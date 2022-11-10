<!-- Descrizione:
Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone. -->
<script>
export default {
    name: "SiteHeader",
    data() {
        return {
            navbarMenu: [
                {
                    text: 'Characters',
                    href: '#'
                },
                {
                    text: 'Comics',
                    href: '#'
                },
                {
                    text: 'Movies',
                    href: '#'
                },
                {
                    text: 'TV',
                    href: '#'
                },
                {
                    text: 'Games',
                    href: '#'
                },
                {
                    text: 'Collectibles',
                    href: '#'
                },
                {
                    text: 'Videos',
                    href: '#'
                },
                {
                    text: 'Fans',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                },
                {
                    text: 'Shop',
                    href: '#'
                }
            ]
        }
    }
}
</script>

<template>
    <div id="site_header">
        <div class="container">
            <div class="row">
                <div class="col-auto">
                    <div class="logo">
                        <img src="../assets/img/dc-logo.png" alt="">
                    </div>
                </div>
                <div class="col">
                    <nav class="navbar">
                        <a :href="item.href" v-for="item in navbarMenu" :class="item.text === 'Comics' ? 'active' : ''">
                            {{ item.text.toUpperCase() }}
                        </a>
                    </nav>
                </div>
            </div>


        </div>

    </div>

</template>

<style lang="scss" scoped>
#site_header {
    font-size: 12px;
    font-weight: bold;
}

.logo {
    img {
        max-width: 100%;
        height: 80px;
        padding: 1rem;
    }
}

.col {
    display: flex;
    align-items: center;
    justify-content: end;
}

.active {
    color: #0282f9;
    padding-bottom: 30px;
    border-bottom: 4px solid #0282f9;
}

a {
    text-decoration: none;
    color: black;
    margin: 0 8px;

    &:hover {
        color: #0282f9;
    }

    &:focus {
        color: #0282f9;
        padding-bottom: 30px;
        border-bottom: 4px solid #0282f9;
    }
}
</style>

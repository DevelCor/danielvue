<template>
    <div>
        <div class="Navbar Aux">
            <div>
                <h1 class="Logo">CV</h1>
                    <nav class="menu">
                        <ul class="ul">
                            <li class="li"> <router-link to="/" class="link">Home</router-link> </li>
                            <li class="li"> <router-link to="/about" class="link" >About</router-link> </li>
                        </ul>
                    </nav>
                </div>      
            </div>
    </div>
</template>

<script>
export default {
    methods: {    
        handleScroll: function () {
            let sticky = document.getElementsByClassName("Aux");    
            let scroll = window.scrollY;
            if (scroll < 520) {
                sticky[0].classList.add("Navbar");
                sticky[0].classList.remove("sticky");
            }
            else {
                sticky[0].classList.add("sticky");
                sticky[0].classList.remove("Navbar");
            }
        }
    },
    created: function () {
        window.addEventListener('scroll', this.handleScroll);
    },
    destroyed: function () {
        window.removeEventListener('scroll', this.handleScroll);
    }
}
</script>
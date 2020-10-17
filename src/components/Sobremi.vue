<template>
    <section class="about_me">
        <div class="about_me_">
            <div class="historia_tittle">
                <h3 class="sobremi_tittle">
                    <span class="history_span"> Pequeña historia </span>  
                    <span class="sobremi_span">Sobre mí</span>
                </h3>
            </div>
            <div class="habilidades_">
                    <div class="biblio">
                        <p class="historia_p">
                        Estudiante universitario, bachiller en ciencias, del liceo bolivariano Monseñor Sanmiguel, gocho, me gustan los vídeo juegos y todo lo que tenga que ver con tecnología... Una gran fascinación por la programación y todo lo sorprendente que se puede lograr al implementar las herramientas correctas con la preparación adecuada.
                        <br><br>
                        Actualmente estudiante de la UNET, en el 3er semestre de ingeniería en informática. Desarrollador javascript, programador Front-End. Programador de c/c++, java, html, css, sass, y conocimientos en manejo del framework de javascript Vue, con gran apego a los patrones de diseño de software y las buenas practicas de javascript, programador javascript full stack en desarrollo.
                        </p>
                    </div>
                    <div class="skills">
                        <span class="coding">Front-end/back-end</span>
                        <div class="skill">
                            <span>HTML</span>
                            <radial-progress-bar :diameter="60"
                             :startColor= "'#42B983'"
                             :stopColor= "'#5B6E65'"
                             :completed-steps="completedSteps"
                             :total-steps="totalSteps">
                             </radial-progress-bar>
                        </div>
                        <div class="skill">
                            <span>CSS</span>
                            <radial-progress-bar :diameter="60"
                             :startColor= "'#42B983'"
                             :stopColor= "'#5B6E65'"
                             :completed-steps="2"
                             :total-steps="totalSteps">
                             </radial-progress-bar>
                        </div>
                        <div class="skill">
                            <span>javascript</span>
                            <radial-progress-bar :diameter="60"
                             :startColor= "'#42B983'"
                             :stopColor= "'#5B6E65'"
                             :completed-steps="6"
                             :total-steps="totalSteps">
                             </radial-progress-bar>
                        </div>
                        <div class="skill">
                            <span>vue</span>
                            <radial-progress-bar :diameter="60"
                             :startColor= "'#42B983'"
                             :stopColor= "'#5B6E65'"
                             :completed-steps="8"
                             :total-steps="totalSteps">
                             </radial-progress-bar>
                        </div>
                    </div>
            </div>
        </div>
    </section>
</template>

<script>
import RadialProgressBar from 'vue-radial-progress'

    export default {
    data () {
        return {
        completedSteps: 5,
        totalSteps: 10,
       // startColor: '#ffffff',
       // stopColor: '#ffffff'
        }
    },

    components: {
        RadialProgressBar
    }
    }
</script>
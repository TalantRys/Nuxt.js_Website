<template>
    <transition name="fade">
        <div v-if="show" class="preloader">
            <p class="preloader__logo">Hello world!</p>
            <div class="preloader__circles">
                <span class="circles__circle"></span>
                <span class="circles__circle"></span>
                <span class="circles__circle"></span>
                <span class="circles__circle"></span>
            </div>
        </div>
    </transition>
</template>
<style>
 .preloader{
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     background-color: #6D6875;
     display: flex;
     justify-content: center;
     align-items: center;
     z-index: 5;
 }
 .fade-enter-active, .fade-leave-active{
     transition: opacity 1s ease;
 }
 .fade-enter, .fade-leave-to{
     opacity: 0;
 }
 .preloader__logo{
     font-size: 50px;
     font-weight: 600;
     color: #fff;
 }
</style>
<script>
export default {
    name: 'preloader',
    data(){
        return{
            show: true,
        }
    },
    mounted(){
        this.showToggle()
    },
    methods:{
        showToggle(){
            setTimeout(() => {
                this.show = false;
            }, 1000)
        }
    }
}
</script>
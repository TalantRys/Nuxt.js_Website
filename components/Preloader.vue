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
                this.show = false
            }, 1000)
        }
    }
}
</script>
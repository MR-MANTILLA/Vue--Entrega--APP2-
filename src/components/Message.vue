<template>
    <div>
        <h1>{{message}}</h1>
        <app-input :msg="message" @messageChanged="message = $event"></app-input>
    </div>
</template>

<script>
    import Input from './input.vue';

    export default{
        data(){
            return{
                message:''
            }
        },

        components:{
            'app-input':Input
        }
    }
</script>

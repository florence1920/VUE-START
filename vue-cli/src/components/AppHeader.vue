<template>
    <header>
        {{ send }}
        {{ send2 }}
        <button v-on:click="renewStr">
            renew
        </button>
    </header>
</template>

<script>
export default {
    props :[
        'send',
        'send2'
    ],
    methods :{
        renewStr : function(){
            this.$emit('renew');
        }
    }
}
</script>

<style>

</style>
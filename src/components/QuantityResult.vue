<template>
    
    <div>
        
        <div v-bind:key="input.id" v-for="input in inputs">
            <QuantityItem v-bind:input="input"/>
        </div>

    </div>   
    
</template>

<script>

import QuantityItem from '../components/QuantityItem.vue';

export default {

    name: 'QuantityResult',
    components: {
        QuantityItem
    },
    props: ["inputs"]

}

</script>

<style scoped>

</style>
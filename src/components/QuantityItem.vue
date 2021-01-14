<template>
    
    <div>
        <p class="quanInput">{{input.quanInput}}</p>
        <p class="quanResult">{{input.quanResult}}</p>
    
    </div>


</template>

<script>


export default {
    name: 'QuantityItem',
    props: ['input']
}

</script>

<style scoped>

.quanInput {
    text-align: center;
    font-size: 3rem;
}

.quanResult {
    text-align: center;
    margin-top: 2rem;
    font-size: 3rem;

}

</style>
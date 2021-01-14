<template>
    
    <div>

        <form class="form" @submit="addInput">

            <input type="text" v-model="quan1" class="Input1 input" name="Input1" id="Input1" placeholder="Lengde"> <span class="smalltext">+</span> 
            <input type="text" v-model="quan2" class="Input2 input" name="Input2" id="Input2" placeholder="Bredde"> <span class="smalltext">+</span> 
            <input type="text" v-model="quan3" class="Input3 input" name="Input3" id="Input3" placeholder="Tykkelse"> 

            <button class="submitBtn" type="submit">Regn ut:</button> 

            <button class="deleteBtn" >Slett:</button> 

        </form>

    </div>
  
</template>

<script>



export default {
    name: 'QuantityInput',
    data() {
        return {
            quan1: '',
            quan2: '',
            quan3: '',
            quanResult: ''
        }
    },
    methods: {

        addInput(e) {
            e.preventDefault();
        }
    }
}

</script>

<style scoped>

.form {
    display: flex;
    align-items: center;
    justify-content: center;

    height: 30vh;
    width: 100vw;
    flex-direction: row;
}

.input {
    width: 20rem;
    padding: 1rem 1rem;
    font-size: 2rem;

    margin: 2rem;
}

.smalltext {
    font-size: 3rem;

}

.submitBtn {
    padding: 1rem 1rem;
    font-size: 2rem;

    border: #808080 solid .25rem;
    color: #fff;
    background-color: steelblue;
    
    margin-right: 2rem;
}

.deleteBtn {
    padding: 1rem 1rem;
    font-size: 2rem;

    border: #808080 solid .25rem;
    color: #fff;
    background-color: maroon;
    
}

</style>
<template>
    <div>
        <input min="0" type="number" @input="changeAmount($event.target.value)" placeholder="Введите число"><br/>
        <button @click="convert()">Конвертировать</button>
    </div>
</template>

<script>
    export default {
        props: {
            changeAmount: {
                type: Function,
                required: true
            },
            convert: {
                type: Function,
                required: true
            }
        }
    }
</script>

<style  scoped>
input { 
    width: 500px;
    outline: none; 
    border-radius: 3px;
    position: relative;
    top: -50px;
    font-size: 1.25em;
    border: 0;
    padding: 15px 20px;
    background: #fafafa;
    color: #333 ;
}
button {
    position: relative;
    top: -20px;   
    padding: 15px 20px;
    color: white;
    text-transform: uppercase;
    cursor: pointer;
    background: #1A032D;
    border: 0;
    border-radius: 3px;

}
</style>
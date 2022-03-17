<template>
    <div class="div">
        <h1>Refresh the page and get advice ❤</h1>
        <div class="box">
            <ul>
                <p
                    v-for="f of Frase"
                    :key="f.id">
                    {{ f.advice }}
                 </p>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MyHome',
        data(){
            return{
                Frase:[]
            }
        },
        created(){
            fetch('https://api.adviceslip.com/advice')
            .then(response => response.json())
            .then(json => {this.Frase = json;})
        }
    }

</script>

<style scoped>
.div{
    margin-top:10%;
    height: 25vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.box{
    width: 50%;
    height: 100%;
    background-color: rgb(179, 19, 112);
    text-align: center;
    font-family:Comic Sans MS, Comic Sans, cursive;
    border-radius:5px;

    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
p{
    width: 100%;
    color:rgb(255, 255, 255);
    font-size: 20px;
}
</style>

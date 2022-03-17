<template>
    <div class="div">
        <h1>This Page gives you advice,log in to enjoy❤</h1>
        <v-img
            lazy-src="https://picsum.photos/id/11/10/6"
            max-height="1000"
            max-width="500"
            border-radius="5"
            src="https://picsum.photos/id/11/500/300"
        ></v-img>
    </div>
</template>

<script>
    export default {
        name: 'MyHome',
    }

</script>

<style scoped>
.div{
    margin-top:20vh;
    height: 25vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
h1{
    width:100%;
    text-align: center;
}
v-img{
    border-radius: 5px;
}
</style>

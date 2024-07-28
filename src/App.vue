<script>
export default{
    data(){
        return {
            message: 'Click me!'
        }
    },
    methods: {
        changeMessage(){
            this.message = 'Hello World!'
        }
    }
}
</script>

<template>
    <div className="wrapper" @click="changeMessage()">
        <p>{{ message }}</p>
    </div>
</template>

<style scoped>
    .wrapper{
        display: flex;
        justify-content: center;
        align-items: center;
        background: rgb(63, 63, 63);
        width: 30vw;
        height: 20vw;
        color: rgb(199, 199, 199);
        font-size: 3vw;
        border-radius: 15px;
        cursor: pointer;
        transition: transform 0.1s ease;
    }
    .wrapper:active{
        transform: translateY(2px);
    }
    .wrapper p{
        user-select: none;
    }
</style>

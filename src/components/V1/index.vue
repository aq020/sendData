<template>
    <div>
        V1
        <button @click="sendHandler">传数据</button>
        V2
    </div>
</template>

<script>
export default {
    name: "V1",
    data(){
        return{
            msg1: "Hello"
        }
    },
    methods:{
        sendHandler(){
            this.$emit("sendMSG",this.msg1)
        }
    }


}
</script>
<style scoped>

</style>
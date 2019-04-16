<template>
    <center>
        <div>
            <input type="text" v-model="userId">
            <button @click="onLoadUser"> Load User</button>
            <nuxt-child />
        </div>
    </center>
</template>

<script>
export default {
    data(){
        return{
            userId:''
        }
    },
    methods:{
        onLoadUser(){
            this.$router.push('/users/' + this.userId)
        }
    }
}
</script>


<template>
    <center>
        <h1>A single user, with ID: {{$route.params.id}}</h1>
    </center>
    
       

</template>

<script>
export default {
    validate(data){
        console.log(data)
        return /^\d+$/.test(data.params.id)
    }
}
</script>


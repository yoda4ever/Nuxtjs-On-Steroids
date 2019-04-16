<template>
    <center>
            <h1>A Single product (ID:{{$route.params.pid}})</h1>
            <button @click="$router.push('/products/')">Return to Products Link</button>
    </center>
</template>

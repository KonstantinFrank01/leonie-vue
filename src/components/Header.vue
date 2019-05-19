<template>
    <div>
        <nav class="navbar navbar-light bg-white mt-2" style="display: flex; justifyContent: flex-end;">
            <a class="navbar-item mr-5" href="#">Article</a>
            <a class="navbar-item mr-4" href="#">Contact</a>
        </nav>   
        <img src="../assets/heroImage.jpg" id="heroImage"/>
    </div>    
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style>
    #heroImage {
        height: 80vh;
        width: 100%;
    }
</style>

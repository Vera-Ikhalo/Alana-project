<template>
    <nav class="pl-3 pr-6 d-flex justify-content-between">
        <div class="links w-25 d-flex justify-content-between align-items-center">
            <img src="../assets/logo.svg" width="30" height="30" class="pointer" alt="logo">
            <router-link to="" class="text-blue-20 text-sm text-decoration-none">Option1</router-link>
            <router-link to="" class="text-blue-20 text-sm text-decoration-none">Option2</router-link>
            <router-link to="" class="text-blue-20 text-sm text-decoration-none">Option3</router-link>
        </div>
        <div class="btn">
            <button class="text-sm text-white">Sign Out</button>
        </div>
    </nav>
</template>

<script>

export default{
    name: 'NavBar',

}
</script>

<style lang="scss">
nav{
    padding: 0 110px 0 50px;
    font-family: 'Open Sans';
    .links{
        width:50%;
        opacity: 1;
    }
    .btn{
        button{
            background-color:#30313A;
            border-radius:5px;
            padding:6px 32px;
            font-weight:600;
        }
        
    }
}

</style>
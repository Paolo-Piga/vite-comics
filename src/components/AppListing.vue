<script>
    export default{
        name: "AppListing"
    }
</script>

<template>
    <div class="listing-container">
        <div class="container">
            VT Comis and marVUEl
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.component-container {
    background-color: black; 
}
.container {
    @include center(horizontal);
    height: 35vh;
    color: white;
    font-weight: bold;
    font-size: 30px;
}
</style>
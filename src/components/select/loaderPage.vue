<template>
    <div class="loading">
        <div class="text">Loading..</div>
    </div>
</template>

<script>
export default {
    name : "loaderPage"
}
</script>

<style scoped lang="scss">

@import "../../../assets/style/vars.scss";

.loading{
    position: fixed;
    top: 0;
    left: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    background-color: rgb(45, 93, 184);

}

.text {
    text-transform: uppercase;
    letter-spacing: 2px; 
}

</style>
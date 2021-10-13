<template>
  <a class="full_btn">VIEW ALL LATEST NEWS</a>
</template>

<script>
export default {
    name: 'FullBtn',
}
</script>

<style lang='scss' scoped>
@import '../assets/style/variables.scss';
.full_btn{
    text-decoration: none;
    text-align: center;
    display: block;
    width: 100%;
    padding: 3.125rem;
    background-color: $primaryRed;
    color: white;

    &:hover{
        background-color: white;
        color:initial;
    }
}

</style>
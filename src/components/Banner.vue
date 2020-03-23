<template>
    <div class="bannerNav row justify-content-md-center">
        <a href="#">
            <div class="bannerLinks col col-lg-2">
                {{catban.links}}
            </div>
        </a>
    </div>
</template>

<script>
export default {
  name: 'Banner',
  props: ['catban']
}
</script>

<style scoped>
.bannerNav{
    display:inline;
    list-style-type: none;
    text-align: center;
    margin: 0;
    padding: 0;
}
.bannerLinks{
    display: inline-block;
    font-size: 15px;
}
</style>
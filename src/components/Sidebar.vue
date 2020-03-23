<template>
    <div>
        <div id="navcontainer">
            <div class="nav flex-column center fluid meun">
                <a class="navcss nav-link" href="#">Awesome mall</a>
                <a class="navcss nav-link" href="#">Cloths</a>
                <a class="navcss nav-link" href="#">Airtimes and bills</a>
                <a class="navcss nav-link" href="#">Computing</a>
                <a class="navcss nav-link" href="#">Housing</a>
                <a class="navcss nav-link" href="#">Electronics</a>
                <a class="navcss nav-link" href="#">Home & office</a>
                <a class="navcss nav-link" href="#">Fashion</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Sidebar',
}
</script>

<style lang="scss" scoped>
    #navcontainer{
        background-color: rgb(238, 231, 231);
    }
    .navcss{
        font-size: 15px;
    }
</style>
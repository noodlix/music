<template>
    <div class="closed">
        <!-- <div class="menu" :on-click="menuClicked()">=</div> -->
        <div class="menu">=</div>
    </div>
    <div class="menu__container open">
        <div class="menu">X</div>
    </div>
</template>
  
<script>
</script>

<style>
.menu__container{
    width: 400px;
    height: 100vh;
    z-index: 2;
    position: absolute;
    background-color: aliceblue;
}
.menu {
    width: 70px;
    height: 70px;
    position: absolute;
    background-color: white;
    border-radius: 50px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    font-size: 40px;
    margin: 20px;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);

}
.closed{
    display: block;
    width: 400px;
    height: 100vh;
    z-index: 2;
    position: absolute;
}
.open{
    display: none;
}
</style>
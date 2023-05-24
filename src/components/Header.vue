<template>
  <div class="header">
    <div class="pic"><img :src="pfp" alt=""></div>
    <div class="name">{{name}}</div>
  </div>
</template>

<script>
export default {
    name: 'profile-page',
    props:{

    },
    data(){
        return{
            name: 'aaa',
            username: 'aaa111',
            pfp: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/2c/Default_pfp.svg/1200px-Default_pfp.svg.png',
        }
    }
}
</script>
<style>
.header {
  width: 100%;
  height: 100px;
  display: flex;
  flex-direction: row;
}

.pic img{
  width: 70px;
  height: 70px;
  background-color: rgb(255, 255, 255);
  margin: 50px 120px;
  border-radius: 50px;
  display: flex;
  flex-direction: row;
  align-items: center;
  box-shadow: 5px 5px 5px rgb(101, 88, 155);
  justify-content: center;

}

.name {
  font-weight: 800;
  font-size: 30px;
  color: white;
  margin: 60px -90px;
}
</style>
<script setup>
import Header from '../components/Header.vue';
import AlbumPicture from '../components/AlbumPicture.vue';
import Footer from '../components/Footer.vue';
import Menu from '../components/Menu.vue';
// export default{
//   data(){
//     return{
//       current_transform: {
//         category: String
//       }
//     }
//   },
//   methods:{
//     transformBody(_transform){
//       this.current_transform = _transform
//     }
//   }
// }
</script>

<template>
  <div class="main">
      <Menu></Menu>
    <div class="contain">
      <div class="body">
        <!-- <div class="innercontainner" @sendTransformation="transformBody" v-bind:style="{ transform: current_transform }"> -->
        <div class="innercontainner">
          <Header></Header>
          <AlbumPicture></AlbumPicture>
          <Footer></Footer>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.main {
  display: flex;
  flex-direction: row;
  align-items: center;  
}

.contain{
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
}

.innercontainner {
  width: 1000px;
  height: 1200px;
  background-color: rgb(195, 181, 251);
  border-radius: 50px;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  flex-direction: column;
  box-shadow: 5px 5px 5px rgb(101, 88, 155);

}

/* .body :hover{
  transform: translate(10px) rotate(15deg);
} */
.body {
  width: 1500px;
  height: 100vh;
  background-color: rgb(161, 141, 243);
  border-radius: 50px;
}
</style>
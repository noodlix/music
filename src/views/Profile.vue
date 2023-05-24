<template>
    <div class="main">
        <Menu></Menu>
        <div class="contain">
            <div class="body">
                <div class="profilecontainner">
                    <div class="headerProfile">
                        <div class="userpictureContainer">
                            <div class="userPicture"></div>
                        </div>
                        <div class="textContainer">
                            <div class="username">Username</div>
                            <div class="profilename">Name</div>
                            <button class="edit">Edit</button>
                        </div>
                    </div>
                    <LikedSongs></LikedSongs>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import Menu from '../components/Menu.vue';
import LikedSongs from '../components/profileComponents/LikedSongs.vue'

</script>

<style>
.profilecontainner {
    width: 1600px;
    height: 1400px;
    background-color: rgb(195, 181, 251);
    border-radius: 50px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);
}

.headerProfile {
    width: 100%;
    height: 300px;
    display: flex;
    /* background-color: aqua; */
    flex-direction: row;
    padding: 50px;
    gap: 50px;
}

.userPicture {
    width: 200px;
    height: 200px;
    border-radius: 100px;
    background-color: white;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);
}

.username {
    font-weight: 800;
    font-size: 50px;
    color: white;
}

.profilename {
    font-weight: 600;
    font-size: 30px;
    color: white;
}

.edit {
    width: 100px;
    height: 50px;
    border-radius: 15px;
    background-color: rgb(161, 141, 243);
    color: white;
    font-size: 20px;
    font-weight: 700;
    border: none;
    margin-top: 10px;
}
</style>
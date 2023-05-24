<script setup>
</script>

<template>
    <div class="contain">
        <div class="body">
            <div class="containnerReg">
                <div class="titleReg">Log-in</div>
                <div class="iconscontainerReg">
                    <div class="iconReg"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/Spotify_logo_without_text.svg/2048px-Spotify_logo_without_text.svg.png" alt=""></div>
                    <div class="iconReg"><img src="https://cdn0.iconfinder.com/data/icons/internet-2020/1080/Applemusicandroid-512.png" alt=""></div>
                    <div class="iconReg"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e7/Yandex_Music_icon.svg/2048px-Yandex_Music_icon.svg.png" alt=""></div>
                </div>
                <div class="innercontainnerReg">
                    <input class="inputReg" type="text" placeholder="username">
                    <input class="inputReg" type="text" placeholder="password">
                    <button class="buttonReg">Log-in</button>
                </div>
                <div class="orLogin">Register</div>
            </div>
        </div>
    </div>
</template>

<style>
.containnerReg {
    width: 600px;
    height: 650px;
    background-color: rgb(195, 181, 251);
    border-radius: 50px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);
}

.innercontainnerReg {
    display: flex;
    flex-direction: column;
    gap: 50px;
}

.titleReg {
    font-size: 60px;
    font-weight: 800;
    color: white;
    margin: 50px 0px 20px;
    text-align: center;
}

.inputReg {
    width: 400px;
    height: 60px;
    border-radius: 10px;
    color:rgb(161, 141, 243);
    font-size: 20px;
    font-weight: 700;
    padding: 10px;
    border: none;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);

}
.buttonReg{
    width: 400px;
    height: 60px;
    border-radius: 15px;
    background-color: rgb(161, 141, 243);
    color:  white;
    font-size: 20px;
    font-weight: 700;
    border: none;
}
.iconscontainerReg{
    display: flex;
    flex-direction: row;
    margin-bottom: 40px;
    gap: 35px;
}
.iconReg img{
    width: 60px;
    height: 60px;
    /* margin-top: 1px; */
}
.iconReg{
    width: 60px;
    height: 60px;
    background-color: rgb(255, 255, 255);
    border-radius: 60px;
}
.orLogin{
    font-size: 20px;
    font-weight: 800;
    color: white;
    margin: 30px;
    text-align: center;
}
</style>
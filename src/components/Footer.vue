<template>
    <div class="footer" >
        <div class="Like rate" @click="likeSong()">💜</div>
        <div class="Dislike rate" @click="dislikeSong()">💔</div>


    </div>
</template>
  
<script>
export default {
    name: 'profile-page',
    props: {
    },
    data() {
        return {
            transform: 'translate(0px) rotate(0deg)'

        }
    },
    computed: {
        computedTransformation: function () {
            return this.transform;
        }
    },
    emits: ['sendTransformation'],
    methods: {
        likeSong: function (event) {
            this.transform = 'translate(100px) rotate(65deg)';
            this.$emit('sendTransformation', this._transform)

        },
        dislikeSong: function (event) {
            this.transform = 'translate(-100px) rotate(-65deg)';
        }
    }
}
</script>
<style>
.footer {
    /* background-color: forestgreen; */
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    transition: transform 1s;

}

.rate {
    width: 80px;
    height: 80px;
    margin-top: -150px;
    border-radius: 50px;
    display: flex;
    flex-direction: row;
    font-size: 30px;
    align-items: center;
    justify-content: center;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);
}

.Like {
    background-color: rgb(161, 141, 243);
}

.Dislike {
    background-color: rgb(248, 246, 255);
}
</style>
<template>
    <div class="container">
        <div class="alb"></div>
        <div class="text">
            <div class="aboutSong">
                <div class="songName">songName</div>
                <div class="artistName">artistName</div>
            </div>
            <div class="stop">||</div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {

            allsongs: [
                {
                    id: '1',
                    songName: ` On My Way Alan Walker`,
                    poster: "img/1.jpg"
                },
                {
                    id: '2',
                    songName: ` Alan Walker-Fade Alan Walker`,
                    poster: "img/2.jpg"
                },
                {
                    id: "3",
                    songName: `Cartoon - On & On  Daniel Levi`,
                    poster: "img/3.jpg",
                },
                {
                    id: "4",
                    songName: `Warriyo - Mortals Mortals`,
                    poster: "img/4.jpg",
                },
                {
                    id: "5",
                    songName: `Ertugrul Gazi Ertugrul`,
                    poster: "img/5.jpg",
                },
                {
                    id: "6",
                    songName: `Electronic Music Electro</div>`,
                    poster: "img/6.jpg",
                },
                {
                    id: "7",
                    songName: `Agar Tum Sath Ho Tamashaa</div>`,
                    poster: "img/7.jpg",
                },
                {
                    id: "8",
                    songName: `Suna Hai Neha Kakker</div>`,
                    poster: "img/8.jpg",
                },
                {
                    id: "9",
                    songName: `Dilber Satyameva Jayate</div>`,
                    poster: "img/9.jpg",
                },
                {
                    id: "10",
                    songName: `Duniya Luka Chuppi</div>`,
                    poster: "img/10.jpg",
                },
                {
                    id: "11",
                    songName: `Lagdi Lahore Di Street Dancer 3D</div>`,
                    poster: "img/11.jpg",
                },
                {
                    id: "12",
                    songName: `Putt Jatt Da Putt Jatt Da</div>`,
                    poster: "img/12.jpg",
                },
                {
                    id: "13",
                    songName: `Baarishein Atif Aslam</div>`,
                    poster: "img/13.jpg",
                },
                {
                    id: "14",
                    songName: `Vaaste Dhvani Bhanushali</div>`,
                    poster: "img/14.jpg",
                },
                {
                    id: "15",
                    songName: `Lut Gaye Jubin Nautiyal</div>`,
                    poster: "img/15.jpg",
                },
            ],
        }
    },
}

</script>
<style>
.container {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    /* background-color: rgba(95, 158, 160, 0.307); */
    flex-direction: column;
}

.alb {
    width: 750px;
    height: 750px;
    background-color: white;
    margin-top: -100px;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);

}

.text {
    width: 750px;
    margin-top: 10px;
    color: white;
    display: flex;
    flex-direction: row;
    gap: 500px
}

.songName {
    font-weight: 800;
    font-size: 30px;
}

.artistName {
    font-weight: 500;
    font-size: 20px;
}

.stop {
    width: 50px;
    height: 50px;
    margin-top: 10px;
    background-color: white;
    color: black;
    border-radius: 50px;
    display: flex;
    flex-direction: row;
    align-items: center;
    box-shadow: 5px 5px 5px rgb(101, 88, 155);
    justify-content: center;
}
</style>
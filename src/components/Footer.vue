<script>

</script>

<template>
    <div class="outerContainer">
        <div class="innerContainer withBackground">
            <div class="listSpace">

                <div class="leftCol">
                    <h2>dc comics</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>

                    <h2>shop</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>

                <div class="centerCol">
                    <h2>dc</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>

                <div class="rightCol">
                    <h2>sites</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>
            </div>

            <div class="giantLogoBg">
                <figure>
                    <img src="../assets/img/dc-logo-bg.png" alt="DC logo in background">
                </figure>
            </div>
        </div>
        <div class="bottomFollowBar">
            <div class="innerContainer withoutBackground">
                <button>
                    sign-up now!
                </button>
                <div class="followButtons">
                    <h2 id="followTitle">
                        follow us
                    </h2>
                    <ul class="followButtons">
                        <li>
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>


</template>

<style scoped>
li {
    color: #959595;
}

button {
    border: 2px solid #0282f9;
    background-color: #303030;
    color: white;
    margin: auto 10px;
    padding: 8px;
}

ul.followButtons {
    display: flex;
    margin: auto 10px;
}

div.leftCol,
div.centerCol,
div.rightCol {
    padding: 25px 25px 25px 0;
    color: white;
}

div.outerContainer {
    background-image: url('../assets/img/footer-bg.jpg');
}

div.innerContainer.withBackground {
    font-size: 13px;
    padding: 20px;
    height: 300px;
    overflow: hidden;
}

div.innerContainer.withoutBackground {
    display: flex;
    justify-content: space-between;
}

div.giantLogoBg figure img {
    transform: translate(270px, -100px);
    height: 450px;
}

div.listSpace {
    display: flex;
}

div.bottomFollowBar {
    height: 100px;
    background-color: #303030;
    display: flex;
    justify-content: space-between;
}

div.followButtons {
    display: flex;
}

#followTitle {
    font-size: 22px;
    margin: auto 20px;
    color: #0282f9;
}
</style>

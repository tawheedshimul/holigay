<template>
    <div class="similarstays">
        <div>

        </div>
        <div class="cards">
            <div class="card">
                <img src="../assets/Banner.png" alt="">
                <p>Chic</p>
                <p>location</p>
                <p>Price</p>
            </div>
            <div class="card">
                <img src="../assets/Banner.png" alt="">
                <p>Chic</p>
                <p>location</p>
                <p>Price</p>
            </div>
            <div class="card">
                <img src="../assets/Banner.png" alt="">
                <p>Chic</p>
                <p>location</p>
                <p>Price</p>
            </div>
            <div class="card">
                <img src="../assets/Banner.png" alt="">
                <p>Chic</p>
                <p>location</p>
                <p>Price</p>
            </div>
        </div>
    </div>
</template>

<style scoped>

.similarstays{
    width: 1348px;
    height: 441px;
    gap: 20px;
    margin: auto;
}
.cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
}

.card {
    width: 332px;
    height: 441px;

}

.card img {
    width: 322px;
    height: 332px;
    border-radius: 16px;

}
</style>
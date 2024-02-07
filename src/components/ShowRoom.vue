<template>
    <div class="showroom">
        <div class="main-img-section">
            <img class="main-img" src="../assets/showroommain.png" alt="" srcset="">
        </div>
        <div class="right-img">
            <div>
                <img class="side-img" src="../assets/showone.png" alt="">
            </div>
            <div>
                <img class="side-img" src="../assets/showone.png" alt="">
            </div>
            <div>
                <img class="side-img" src="../assets/showone.png" alt="">
            </div>
            <div>
                <img class="side-img" src="../assets/showone.png" alt="">
            </div>
        </div>
    </div>
</template>

<style scoped>
.showroom {
    height: 500px;
    max-width: 1348px;
    margin: auto;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
}

.main-img {
    width: 99%;
    height: 500px;
    object-fit: fill;
    border-radius: 16px;
}

.right-img {
  width: 98%;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  
}

.side-img {
  width: 98%;
  height: 245px;
  object-fit: fill;
  border-radius: 16px;
  gap: 10px;
}
</style>
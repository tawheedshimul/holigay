<template>
    <div class="room">
        <div class="room-top">
            <p class="room-title">
                2Rooms Available
            </p>
            <div>
hello
            </div>
        </div>
        <!-- rooom 1  -->
        <div class="room-card">
            <p class="room-card-title">Double Standard Room</p>
            <div class="room-card-object">
                <div class="room-card-left">
                    <img src="../assets/showone.png" alt="">
                    <p>room</p>

                </div>
                <div class="vertical-line"></div>
                <div class="room-card-middle">
                    <span class="card-text">Wi-fi </span>
                    <span class="card-text">Shower </span>
                    <span class="card-text">City View </span>
                    <span class="card-text">Hair Dryer </span>
                    <span class="card-text">Towel </span>
                    <span class="card-text">Free toiletries </span>
                    <span class="card-text">Kitchen </span>
                    <span class="card-text">Washing machine </span>
                    <span class="card-text">Toilet </span>
                    <span class="card-text">Sofa </span>
                    <span class="card-text">Linen </span>
                    <span class="card-text">Desk </span>
                    <span class="card-text">Seating Area </span>
                    <span class="card-text">Video </span>
                    <span class="card-text">Private entrance </span>
                    <span class="card-text">TV </span>
                    <span class="card-text">internet Facilites </span>
                    <span class="card-text">Refrigerator </span>
                    <span class="card-text">Ironing </span>
                    <span class="card-text">Tea/Coffee maker </span>
                    <span class="card-text">MicroWave </span>
                    <span class="card-text">Heating </span>
                    <span class="card-text">Kitchenware </span>
                    <span class="card-text">Fan </span>
                    <span class="card-text">Outdoor furniture </span>
                </div>
                <div class="vertical-line"></div>
                <div>
                    <div style="display: flex ; align-items: last baseline;">
                        <p
                            style="font-family: 'Plus Jakarta Sans', sans-serif; font-weight: 600; font-size: 32px;  letter-spacing: -2%;margin: 0px; color: #040112;">
                            $86</p>
                        <span class="text-low-opacity">/night</span>
                    </div>

                    <form class="card-pay">
                        <input type="radio" id="paycard" name="paymentMethod">
                        <label class="card-text2" for="paycard">Pay with card</label>
                        <br>
                        <input type="radio" id="payhotel" name="paymentMethod">
                        <label class="card-text2" for="payhotel"><span>Pay at hotel</span></label>
                    </form>
                    <button class="btn">Book Now</button>
                    <p class="text-low-opacity">Free Cancellation before 18 Apr 2024</p>
                </div>
            </div>

        </div>
        <!-- room 2  -->
        <div class="room-card">
            <p class="room-card-title">Twin Room</p>
            <div class="room-card-object">
                <div class="room-card-left">
                    <img src="../assets/showone.png" alt="">
                    <p>room</p>

                </div>
                <div class="vertical-line"></div>
                <div class="room-card-middle">
                    <span class="card-text">Wi-fi </span>
                    <span class="card-text">Shower </span>
                    <span class="card-text">City View </span>
                    <span class="card-text">Hair Dryer </span>
                    <span class="card-text">Towel </span>
                    <span class="card-text">Free toiletries </span>
                    <span class="card-text">Kitchen </span>
                    <span class="card-text">Washing machine </span>
                    <span class="card-text">Toilet </span>
                    <span class="card-text">Sofa </span>
                    <span class="card-text">Linen </span>
                    <span class="card-text">Desk </span>
                    <span class="card-text">Seating Area </span>
                    <span class="card-text">Video </span>
                    <span class="card-text">Private entrance </span>
                    <span class="card-text">TV </span>
                    <span class="card-text">internet Facilites </span>
                    <span class="card-text">Refrigerator </span>
                    <span class="card-text">Ironing </span>
                    <span class="card-text">Tea/Coffee maker </span>
                    <span class="card-text">MicroWave </span>
                    <span class="card-text">Heating </span>
                    <span class="card-text">Kitchenware </span>
                    <span class="card-text">Fan </span>
                    <span class="card-text">Outdoor furniture </span>
                </div>
                <div class="vertical-line"></div>
                <div>
                    <div style="display: flex ; align-items: last baseline;">
                        <p
                            style="font-family: 'Plus Jakarta Sans', sans-serif; font-weight: 600; font-size: 32px;  letter-spacing: -2%;margin: 0px; color: #040112;">
                            $86</p>
                        <span class="text-low-opacity">/night</span>
                    </div>

                    <form class="card-pay">
                        <input type="radio" id="paycard" name="paymentMethod">
                        <label class="card-text2" for="paycard">Pay with card</label>
                        <br>
                        <input type="radio" id="payhotel" name="paymentMethod">
                        <label class="card-text2" for="payhotel"><span>Pay at hotel</span></label>
                    </form>
                    <button class="btn">Book Now</button>
                    <p class="text-low-opacity">Free Cancellation before 18 Apr 2024</p>
                </div>
            </div>

        </div>

    </div>
</template>

<style scoped>
.room {
    max-width: 1120px;
    margin: auto;
}

.room-top{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.room-title {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 600;
    font-size: 24px;
    line-height: 28.8px;
    letter-spacing: -2%;
    color: #040112;
}

.room-card {
    width: 100%;
    background-color: #F7F7F8;
    border-radius: 16px;
    padding: 24px;
    margin-top: 10px;
}

.room-card-title {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 600;
    font-size: 18px;
    line-height: 30.6px;
    color: #040112;
}

.room-card-object {
    display: flex;
    /* align-items: center; */
}

.vertical-line {
    width: 1px;
    height: 350px;
    background-color: #E1DEE9;
    margin: 0px 20px 0px 20px;

}

.room-card-left img {
    width: 274px;
    height: 274px;
    border-radius: 12px;
    background-size: fill;
}

.room-card-middle {
    width: 452px;
    padding: 12px, 0px, 12px, 0px;
}

.card-text {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 400;
    font-size: 14px;
    line-height: 23.8px;
    color: #040112;
    border-radius: 4px;
    padding: 2px 4px;
    margin-right: 10px;
    background-color: #EDEDEF;
}

.card-text2 {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 400;
    font-size: 14px;
    line-height: 23.8px;
    color: #040112;
    border-radius: 4px;
}

.card-pay {
    align-items: center;
    padding: 45px 0px 15px 0px;
}

input[type="radio"] {
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    width: 13px;
    height: 13px;
    border-radius: 50%;
    outline: none;
    transition: 0.1s;
    border: 1px solid #E1DEE9;
}

/* CSS to style radio button icons when checked */
input[type="radio"]:checked {
    border: 4px solid #EB4730;
    /* Orange background when checked */
}

.btn {
    background-color: #EB4730;
    color: white;
}

.text-low-opacity {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 400;
    font-size: 14px;
    line-height: 23.8px;
    color: #040112;
    opacity: 60%;
}</style>
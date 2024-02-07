<template>
    <div class="footer">
        <!-- links 1 -->
        <div class="footer-top">
            <div class="footer-object">
                <p class="footer-link-name">Link 1</p>
                <p class="footer-link">Duis dignissim</p>
                <p class="footer-link">Aliquam quis</p>
                <p class="footer-link">Nullam a scelerisque</p>
                <p class="footer-link">Morbi ornare</p>
                <p class="footer-link">Aliquam porttitor</p>
            </div>
            <div class="footer-object">
                <p class="footer-link-name">Link 1</p>
                <p class="footer-link">Duis dignissim</p>
                <p class="footer-link">Aliquam quis</p>
                <p class="footer-link">Nullam a scelerisque</p>
                <p class="footer-link">Morbi ornare</p>
                <p class="footer-link">Aliquam porttitor</p>
            </div>
            <div class="footer-object">
                <p class="footer-link-name">Link 1</p>
                <p class="footer-link">Duis dignissim</p>
                <p class="footer-link">Aliquam quis</p>
                <p class="footer-link">Nullam a scelerisque</p>
                <p class="footer-link">Morbi ornare</p>
                <p class="footer-link">Aliquam porttitor</p>
            </div>
            <div class="footer-object">
                <p class="footer-link-name">Link 1</p>
                <p class="footer-link">Duis dignissim</p>
                <p class="footer-link">Aliquam quis</p>
                <p class="footer-link">Nullam a scelerisque</p>
                <p class="footer-link">Morbi ornare</p>
                <p class="footer-link">Aliquam porttitor</p>
            </div>
            <div class="footer-object">
                <img src="../assets/flogo1.png" alt="">
                <img src="../assets/flogo2.png" alt="">
            </div>
            <div class="footer-object">
                <img src="../assets/flogo3.png" alt="">
                <img src="../assets/flogo4.png" alt="">
            </div>
        </div>
        <hr>
        <div class="footer-bottom">
            <div class="footer-bottom-left">
                <p class="footer-bottom-text">© 2024 Holigay </p>
                <p class="footer-bottom-text">Terms of service </p>
                <p class="footer-bottom-text">Privacy Policy </p>
            </div>
            <div>
                <img src="../assets/holigay.png" alt="">
            </div>
            <div class="footer-bottom-text">
                <div>
                    currencygdfgdgdfgdfggdfgdffdg
                </div>
                <div>
                    currency
                </div>
                <div>
                    currency
                </div>
                <div>
                    currency
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer {
    max-width: 1440px;
    /* height: 427px; */
    border-radius: 16px 16px 0 0;
    background-color: #0B0721;
    margin: auto;
}

.footer-top {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
}

@media only screen and (max-width: 960px) {
    .footer-top {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
    }
}


.footer-object {
    padding: 30px;

}

.footer-object img {
    width: 100%;
    height: 80px;
    opacity: 40%;
}

.footer-link-name {
    font-weight: 500;
    font-size: 14px;
    line-height: 18.2px;
    letter-spacing: -0.2px;
    color: #FFFFFF;
    opacity: 60%;
}

.footer-link {
    font-weight: 400;
    font-size: 14px;
    line-height: 18.2px;
    letter-spacing: -0.2px;
    color: #FFFFFF;
}

.footer-bottom {
    display: flex;
    justify-content: space-between;
   margin: auto;
}

.footer-bottom-left {
    display: flex;
}

.footer-bottom-text {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 18.2px;
    letter-spacing: -.2px;
    text-align: center;
    color: #FFFFFF;
}
</style>
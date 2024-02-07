<template>
    <div class="similarstays">
        <div class="similar-title">
            <p>Similar Stays</p>
            <div>
                <svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="18" cy="18" r="18" fill="gray" />
                    <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M19.6014 13.6979C19.4749 13.5715 19.3033 13.5005 19.1244 13.5005C18.9455 13.5005 18.774 13.5715 18.6474 13.6979L14.8224 17.5229C14.696 17.6495 14.625 17.821 14.625 17.9999C14.625 18.1788 14.696 18.3503 14.8224 18.4769L18.6474 22.3019C18.7754 22.4211 18.9446 22.486 19.1195 22.483C19.2944 22.4799 19.4612 22.409 19.5849 22.2854C19.7086 22.1617 19.7794 21.9948 19.7825 21.82C19.7856 21.6451 19.7207 21.4759 19.6014 21.3479L16.2534 17.9999L19.6014 14.6519C19.7278 14.5253 19.7988 14.3538 19.7988 14.1749C19.7988 13.996 19.7278 13.8245 19.6014 13.6979Z"
                        fill="#F0EFF3" />
                </svg>

                <svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="18" cy="18" r="18" fill="#F0EFF3" />
                    <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M16.3986 13.6979C16.5251 13.5715 16.6967 13.5005 16.8756 13.5005C17.0545 13.5005 17.226 13.5715 17.3526 13.6979L21.1776 17.5229C21.304 17.6495 21.375 17.821 21.375 17.9999C21.375 18.1788 21.304 18.3503 21.1776 18.4769L17.3526 22.3019C17.2246 22.4211 17.0554 22.486 16.8805 22.483C16.7056 22.4799 16.5388 22.409 16.4151 22.2854C16.2914 22.1617 16.2206 21.9948 16.2175 21.82C16.2144 21.6451 16.2793 21.4759 16.3986 21.3479L19.7466 17.9999L16.3986 14.6519C16.2722 14.5253 16.2012 14.3538 16.2012 14.1749C16.2012 13.996 16.2722 13.8245 16.3986 13.6979Z"
                        fill="#040112" />
                </svg>
            </div>
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
    gap: 20px;
    margin: auto;
}

.similar-title {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.similar-title p{
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 600;
    font-size: 24px;
    line-height: 28.8px;
    letter-spacing: -2%;
    color: #010215;
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
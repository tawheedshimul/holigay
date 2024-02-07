<template>
    <div class="hotelpolicy">
        <div class="hotel-title">
            Hotel Policy
        </div>

        <div class="policy">
            <p class="policy-title">Check In</p>
            <p class="policy-text">From 16:00</p>
        </div>
        <div class="policy">
            <p class="policy-title">Check Out</p>
            <p class="policy-text">Unit 10:00</p>
        </div>
        <div class="policy">
            <p class="policy-title">Cancellation/prepayment</p>
            <p class="policy-text">Cancellation and prepayment policies vary according to accommodation type. Please check
                what <span style="color: #EB4730;">conditions </span>may
                apply to each option when making your selection.</p>
        </div>
        <div class="policy">
            <p class="policy-title">Children and beds</p>
            <div>
                <p class="policy-title">Child policies</p>
                <p class="policy-text">Children of any age are welcome <br> To see correct prices and occupancy information, please add the number of children in your group and their ages to your search</p>
                <p class="policy-title">Cost and extra bed policies</p>
                <span class="policy-text">No costs or extra beds are available</span>
            </div>
        </div>
        <div class="policy">
            <p class="policy-title">Age restriction</p>
            <p class="policy-text">The minimum age for check-in is 25</p>
        </div>
        <div class="policy">
            <p class="policy-title">Pets</p>
            <p class="policy-text">Pets are allowed. No extra charges.</p>
        </div>
        <div class="policy">
            <p class="policy-title">Accepted payment methods</p>
            <div>
                <p class="policy-text">Credit Cards</p>
                <p class="policy-text">Cash</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.hotelpolicy {
    max-width: 1120px;
    margin: auto;
    padding-top: 20px;
}

.hotel-title {
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 600;
    font-size: 24px;
    line-height: 28.8px;
    letter-spacing: -2%;
    color: #010215;
}

.policy {
    display: flex;
    border-bottom: 1px solid #F0EFF3;
}

@media only screen and (max-width: 600px) {
    .policy {
        display: block; /* or inline-block */
        border-bottom: 1px solid #F0EFF3;
        /* Additional styling for small devices */
    }
}

.policy-title {
    min-width: 240px;
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 600;
    font-size: 14px;
    line-height: 23.8px;
    color: #040112;
}

.policy-text {
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 400;
    font-size: 14px;
    line-height: 23.8px;
    color: #040112;
}
</style>
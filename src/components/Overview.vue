<template>
    <div class="overview">
        <div class="left">
            <p>3-star hotel</p>
            <p class="left-title">
                Savor the Sea Breeze: Experience Unrivaled Luxury at Our Seaside Retreat in Malibu
            </p>
            <p class="left-desc">
                Indulge in the epitome of coastal luxury at our Seaside Retreat in Malibu. Nestled along the sun-kissed
                shores of California, this haven promises a harmonious blend of serenity and sophistication. Let the
                rhythmic waves and breathtaking sunsets set the stage for an unforgettable escape.
            </p>
            <p class="left-title">Captivating Amenities Await</p>
            <div class="left-facilities">
                <div class="left-title-desc">
                    <p class="left-fa-title">Private Beach Access:</p>
                    <p class="left-desc">Enjoy exclusive entry to the pristine sands of Malibu, steps away from your
                        accommodation.</p>
                </div>
                <div class="left-title-desc">
                    <p class="left-fa-title">Panoramic Ocean Views:</p>
                    <p class="left-desc">Immerse yourself in the beauty of the Pacific with sweeping views from the comfort
                        of your retreat.</p>
                </div>
                <div class="left-title-desc">
                    <p class="left-fa-title">Private Beach Access:</p>
                    <p class="left-desc">Unwind on your private terrace, perfect for sipping cocktails or stargazing over
                        the tranquil ocean.</p>
                </div>
                <div class="left-title-desc">
                    <p class="left-fa-title">Private Beach Access:</p>
                    <p class="left-desc">Enjoy exclusive entry to the pristine sands of Malibu, steps away from your
                        accommodation.</p>
                </div>
            </div>
            <button class="btn">Show All Facilites</button>
        </div>

        <!-- right side  -->

        <div class="right">
            <div class="rating-overview">
                <div class="rating-avg">
                    <div class="rating-avg-point">
                        4.5
                    </div>
                    <div>
                        <p class="avg-point-condition">Very Good</p>
                        <p class="user-rating">11 User Reviews</p>
                    </div>
                </div>
            </div>
            <div>
                <select>
                    <option value="">date</option>
                </select>
            </div>
            <div>
                <select>
                    <option value="option1">Option 1</option>
                    <option value="option2" selected>Option 2</option>
                    <option value="option3">Option 3</option>
                </select>
            </div>
            <div>
                <p>Check in:</p>
                <div>
                    <p>from</p>
                    <p>date</p>
                </div>
            </div>
            <div>
                <p>Check Out:</p>
                <div>
                    <p>from</p>
                    <p>date</p>
                </div>
            </div>
            <div>
                map
            </div>
            <div>
                <p>Parking</p>
                <p>Availabel</p>
            </div>
            <div>
                <p>Parking</p>
                <p>Availabel</p>
            </div>
            <div>
                <p>Parking</p>
                <p>Availabel</p>
            </div>
            <p>What else is nearby</p>
        </div>
    </div>
</template>

<style scoped>
.overview {
    width: 1120px;
    height: 629px;
    gap: 64px;
    display: flex;
    margin: auto;
    padding-top: 64px;
}

.left {
    width: 734px;
}

.left-title {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 600;
    font-size: 24px;
    line-height: 28.8px;
    letter-spacing: -0.02em;

}

.left-desc {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 400;
    font-size: 14px;
    line-height: 23.8px;
}

.left-facilities {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
}

.left-title-desc {
    width: 347px;
}

.left-fa-title {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 600;
    font-size: 14px;
    line-height: 23.8px;
}

.btn {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 600;
    font-size: 14px;
    line-height: 18.2px;
    letter-spacing: -0.02em;
    text-align: center;
    color: #FFFFFF;
    background-color: #EB4730;
    outline: none;
    border-radius: 8px;
    padding: 12px 16px;
    margin-bottom: 8px;
    cursor: pointer;

}

.right {
    width: 234px;
}

.rating-overview {
    width: 312px;
    height: 76px;
    border-radius: 12px;
    padding: 24px;
    background: #F7F7F8;
    margin-bottom: 10px;
    align-items: center;
    display: flex;
}

.rating-avg {
    height: 42px;
    display: flex;
    align-items: center;
}

.rating-avg-point {
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 700;
    font-size: 42px;
    line-height: 41.6px;
    letter-spacing: -.02em;
    color: #19AA4A;
}
.avg-point-condition{
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 700;
    font-size: 14px;
    margin-bottom: 4px;
    color: #19AA4A;
    padding-left: 20px;
}
.user-rating{
    font-family: 'Plus Jakarta Sans', sans-serif;
    font-weight: 400;
    font-size: 12px;
    color: #040112;
    opacity: 60%;
    padding-left: 20px;
}
</style>
<template>
    <div class="ratings">
        <div>
            <div class="ratings-card-top">
                <div class="rating-left-card">
                    <p class="left-card-p1">HOLIGAY</p>
                    <p class="left-card-p2">4.5</p>
                    <p class="left-card-p3">User Rating</p>
                    <p class="left-card-p4">Based on 12 reviews</p>
                </div>
                <div>
                    <div class="rating-right-card">
                        <p>5</p>
                        <svg width="160" height="4" viewBox="0 0 160 4" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect opacity="0.1" y="0.0012207" width="160" height="4" rx="1" fill="#19AA4A" />
                            <rect y="0.0012207" width="142" height="4" rx="1" fill="#19AA4A" />
                        </svg>
                        <p>32</p>
                    </div>
                    <div class="rating-right-card">
                        <p>5</p>
                        <svg width="160" height="4" viewBox="0 0 160 4" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect opacity="0.1" y="0.0012207" width="160" height="4" rx="1" fill="#19AA4A" />
                            <rect y="0.0012207" width="142" height="4" rx="1" fill="#19AA4A" />
                        </svg>
                        <p>32</p>
                    </div>
                    <div class="rating-right-card">
                        <p>5</p>
                        <svg width="160" height="4" viewBox="0 0 160 4" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect opacity="0.1" y="0.0012207" width="160" height="4" rx="1" fill="#19AA4A" />
                            <rect y="0.0012207" width="142" height="4" rx="1" fill="#19AA4A" />
                        </svg>
                        <p>32</p>
                    </div>
                    <div class="rating-right-card">
                        <p>5</p>
                        <svg width="160" height="4" viewBox="0 0 160 4" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect opacity="0.1" y="0.0012207" width="160" height="4" rx="1" fill="#19AA4A" />
                            <rect y="0.0012207" width="142" height="4" rx="1" fill="#19AA4A" />
                        </svg>
                        <p>32</p>
                    </div>
                    <div class="rating-right-card">
                        <p>5</p>
                        <svg width="160" height="4" viewBox="0 0 160 4" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect opacity="0.1" y="0.0012207" width="160" height="4" rx="1" fill="#19AA4A" />
                            <rect y="0.0012207" width="142" height="4" rx="1" fill="#19AA4A" />
                        </svg>
                        <p>32</p>
                    </div>
                </div>
            </div>
        </div>
        <div v-for="(review, index) in reviews" :key="index">

            <div class="ratings-info">
                <div class="rating-leftside">
                    <div>
                        <div v-for="n in review.rating" :key="n" style="display: inline-block">
                            <svg width="22" height="20" viewBox="0 0 22 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M10.5245 0.465723C10.6741 0.00506783 11.3259 0.00506735 11.4755 0.465723L13.5819 6.9485C13.6488 7.15451 13.8408 7.29399 14.0574 7.29399H20.8738C21.3582 7.29399 21.5596 7.9138 21.1677 8.1985L15.6531 12.2051C15.4779 12.3324 15.4046 12.5581 15.4715 12.7641L17.5779 19.2469C17.7276 19.7075 17.2003 20.0906 16.8085 19.8059L11.2939 15.7993C11.1186 15.672 10.8814 15.672 10.7061 15.7993L5.19153 19.8059C4.79967 20.0906 4.27243 19.7075 4.42211 19.2469L6.52849 12.7641C6.59543 12.5581 6.5221 12.3324 6.34685 12.2051L0.832272 8.1985C0.440415 7.9138 0.641802 7.29399 1.12616 7.29399H7.94256C8.15917 7.29399 8.35115 7.15451 8.41809 6.9485L10.5245 0.465723Z"
                                    fill="#19AA4A" />
                            </svg>
                        </div>
                    </div>
                    <div>
                        <div>{{ review.name }}</div>
                        <div>{{ review.date }}</div>
                    </div>
                </div>
                <div>
                    <div class="rating-title">{{ review.title }}</div>
                    <div class="rating-details">
                        <template v-if="review.message.length <= 350">
                            {{ review.message }}
                        </template>
                        <template v-else>
                            <div v-if="!showFull[index]">{{ review.message.substring(0, 350) }}...</div>
                            <div v-else>{{ review.message }}</div>
                            <button @click="toggleShowMore(index)">
                                {{ showFull[index] ? 'Show Less' : 'Show More' }}
                            </button>
                        </template>
                    </div>
                </div>

            </div>

        </div>
        <button class="btn">More Reviews</button>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            reviews: [
                { name: "Hena", rating: 2, date: 'January 2024', title: "A Coastal Paradies!", message: 'Our stay at the Seaside Retreat in Malibu was nothing short of magical. The private beach access made every morning a delight, and the oceanview suite offered breathtaking views from sunrise to sunset. Impeccable amenities and a serene atmosphere made this escape truly unforgettable. We can not wait to return!' },
                { name: "Hena", rating: 2, date: 'January 2024', title: "Luxury Redefined", message: 'The Sunset Villa exceeded our expectations in every way. The attention to detail, from the spacious living areas to the exclusive terrace, was remarkable. The staff was attentive, ensuring a seamless experience. This retreat redefines luxury, and we will cherish the memories of our stay for a lifetime.' },
                { name: "Tawheed", rating: 3, date: 'January 2024', title: "An Unforgettable Coastal Escape", message: 'From the moment we arrived at the Seaside Retreat in Malibu, it felt like stepping into a dream. The Oceanview Suite, with its floor-to-ceiling windows, provided a continuous spectacle of the mesmerizing Pacific. Each morning, the private beach access allowed us to relish the soft sands and crashing waves in absolute solitude. The meticulous attention to deta' },
                {
                    name: "John", rating: 5, date: 'January 2024', title: "Highly recommended!", message: `Our stay at the Seaside Retreat in Malibu was a symphony of serenity and luxury, leaving us utterly captivated by the coastal charm. The Sunset Villa, with its exclusive terrace overlooking the Pacific, provided an idyllic setting for unwinding amidst breathtaking sunsets.

From the moment we stepped into our coastal haven, the attention to detail was evident. The Cozy Fireplace Lounge became our sanctuary during cooler evenings, creating an intimate ambiance that complemented the rhythmic sound of the waves. The personal touch extended to the staff, who went above and beyond to ensure our every need was met.
The Infinity Pool, with its panoramic views of the ocean, added a touch of glamour to our days. It was the perfect spot to bask in the California sun while enjoying the gentle ocean breeze. The Luxury Spa-Inspired Bathrooms were a true indulgence, offering a retreat within a retreat.

Our Seaside Retreat experience was nothing short of perfection. Every amenity and service contributed to an atmosphere of unparalleled tranquility. We departed with a sense of rejuvenation and gratitude for having discovered this coastal gem. For those seeking an escape where seaside serenity meets refined luxury, this retreat is an absolute masterpiece`
                }
            ]
            , showFull: []
        }
    },
    methods: {
        toggleShowMore(index) {
            this.$set(this.showFull, index, !this.showFull[index]);
        }
    }
}
</script>
  
<style>
.ratings {
    max-width: 1120px;
    margin: auto;
}

.ratings-card-top {
    width: 518px;
    margin: auto;
    padding: 40px;
    display: flex;
    justify-content: space-between; /* Move justify-content to main CSS */
}

@media only screen and (max-width: 720px) {
    .ratings-card-top {
        max-width: 960px;
    }
}

.rating-left-card {
    border-radius: 16px;
    padding: 32px 24px 24px 24px;
    width: 250px;
    background-color: #F7F7F8;
    text-align: center;
    margin-right: 10px;


}

.left-card-p1 {}

.left-card-p2 {
    font-family: 'Plus Jakarta Sans', Arial, sans-serif;
    font-weight: 700;
    font-size: 48px;
    margin: 0px;
    letter-spacing: -0.96px;
    text-align: center;
    color: #19AA4A;
}

.left-card-p3 {
    font-family: 'Plus Jakarta Sans', Arial, sans-serif;
    font-weight: 600;
    font-size: 24px;
    margin: 0px;
    letter-spacing: -0.96px;
    text-align: center;
    color: #010215;

}

.left-card-p4 {
    opacity: 60%;
    color: #040112;
    font-family: 'Plus Jakarta Sans', Arial, sans-serif;
    font-weight: 400;
    font-size: 14px;
    margin: 0px;
    letter-spacing: -0.96px;
    text-align: center;

}

.rating-right-card {
    display: flex;
    align-items: center;
    margin: 0px;
    height: 40px;
}

.ratings-info {
    display: flex;
    margin-bottom: 10px;
    margin-top: 10px;
    border-bottom: 1px solid #F0EFF3;

}

@media only screen and (max-width: 960px) {
    .ratings-info {
        display: flex;
        flex-direction: column-reverse;
        border-bottom: 1px solid #F0EFF3;
        /* Additional styling for small devices */
    }

    .rating-leftside div {
        display: flex;
    }
}

.rating-leftside {
    min-width: 320px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.rating-title {
    font-family: 'Plus Jakarta Sans', Arial, sans-serif;
    font-weight: 600;
    font-size: 16px;
    line-height: 27.2px;
    color: #040112;
}

.rating-details {
    font-family: 'Plus Jakarta Sans', Arial, sans-serif;
    font-weight: 400;
    font-size: 14px;
    line-height: 23.8px;
    color: #040112;
}

.btn {
    border-radius: 8px;
    padding: 12px 32px;
    margin-top: 20px;
    width: 100%;
    background-color: #F0EFF3;
    outline: none;
    font-family: 'Plus Jakarta Sans', Arial, sans-serif;
    font-weight: 600;
    font-size: 14px;
    line-height: 18.2px;
    letter-spacing: -0.2px;
    text-align: center;
    color: #040112;
    cursor: pointer;
}
</style>
  
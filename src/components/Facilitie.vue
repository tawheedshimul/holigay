<template>
    <div class="facilitie">
        <div class="hotel">
            <div class="hotel-features">
                <div v-for="(category, index) in categories" :key="index" class="category">
                    <div class="hotel-name-flex">
                        <div class="facility-name">{{ category.name }}</div>
                        <button class="buttons" @click="toggleShow(index)">
                            {{ showMore[index] ? 'Show less' : 'See more' }}
                        </button>
                    </div>
                    <div>
                        <ul class="facility-features">
                            <li v-for="(feature, idx) in category.features" :key="idx"
                                v-show="showMore[index] || idx < maxFeatures">
                                {{ feature }}
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            categories: [
                { name: "Internet access", features: ["Free Wi-Fi all rooms", "Internet", "Internet services", "Wi-fi public areas"] },
                { name: "Things to do", features: ["Fitness center", "Hot tub", "Sauna", "Wi-Fi in public areas", "Spa", "Spa/Sauna", "Swimming Pool", "Tours"] },
                { name: "Accessibility", features: ["Wheelchair accessible"] },
                { name: "Getting around", features: ["Airport transfer", "Car park"] },
                { name: "Cleanliness and safety", features: ["Anti-viral cleaning products", "Cashless payment service", "Daily disinfection in all rooms", "Daily disinfection in common areas", "Face covering on staff", "First aid kit", "Guest rooms seal after sanitization", "Hand sanitiser", "Hotel room service app", "Hot water linen and Laundry washing", "Hygiene certification", "Physical distancing of at least 1 meter", "Professional-grade sanitizing service", "Protective screens in common areas", "Room sanitization opt-out available", "Rooms sanitized between stays", "Safe dining setup", "Sanitized kitchen and tableware items", "Shared stationery removed"] },
                { name: "Dining, drinking and snacking", features: ["Bar", "Breakfast[buffet]", "Coffee shop", "Poolside bar", "Restaurants", "Room service", "Snack bar"] },
                { name: "Services and conveniences", features: ["Air conditioning in public area", "Contactless check-in/out", "Daily housekeeping", "Dry cleaning", "Elevator", "Facilities for disabled guests", "Food delivery", "Heating in public area", "Laundry service", "Luggage storage", "Meeting/banquet facilities", "Safety deposit boxes", "Smoke-free property", "Terrace", "Xerox/fax in business center"] },
                { name: "Available in all rooms", features: ["Accessible by elevator", "Air conditioning", "Bathroom phone", "Closet", "Clothes rack", "Desk", "Hair dryer", "Heating", "In-room safe", "lines", "Mini bar", "Mirror", "Non-smoking", "Private bathroom", "Satellite/cable channels", "Shower", "Smoke detector", "Socket detector", "Socket near the bed", "Soundproofing", "Telephone"] }
            ],
            showMore: [], // Initialize showMore array
            maxFeatures: 3,
        };
    },
    created() {
        // Initialize showMore array with false for each category
        this.showMore = new Array(this.categories.length).fill(false);
    },
    methods: {
        toggleShow(index) {
            // Toggle the showMore value for the clicked category
            this.$set(this.showMore, index, !this.showMore[index]);
        },
    },
};
</script>
  
<style>
.facilitie{
    max-width: 1120px;
    margin: auto;
    padding-top: 40px;
}
.hotel {
    width: 100%;
}

.hotel-features {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
}

@media(max-width: 560px) {
    .hotel-features {
        grid-template-columns: repeat(1, 1fr);
    }
}

.category {
    border-radius: 8px;
    padding: 16px;
    margin: 8px;
    background-color: #F7F7F8;
}

/* Style the button for better visibility */
.buttons {
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 500;
    font-size: 14px;
    letter-spacing: -0.02em;
    text-align: center;
    color: #040112;
    opacity: 40%;
    background: none;
    border: none;
    padding: 0;
    margin: 0;
}

.facility-features {
    list-style: none;
    padding-left: 0;
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 400;
    font-size: 14px;

}

.hotel-name-flex {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.facility-name {
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 600;
    margin-bottom: 5px;
    font-size: 14px;
}


/* Remove default list styling */
ul {
    list-style: none;
}
</style>
  
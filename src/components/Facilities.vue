<template>
    <div class="facilities">
        <div class="faci-title">
            {{ title }}
        </div>
        <div class="faci-object">
            <div v-for="(group, groupIndex) in facilityGroups" :key="groupIndex" class="group">
                <div v-for="(facility, facilityIndex) in group" :key="facilityIndex" class="facility">
                    <div class="facility-name">{{ facility.name }}</div>
                    <ul class="facility-features">
                        <li v-for="(feature, featureIndex) in facility.features" :key="featureIndex">{{ feature }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script setup>
const title = "Facilities";

const facilityGroups = [
    [
        { name: "Internet access", features: ["Free Wi-Fi all rooms", "Internet", "Internet services", "Wi-fi public areas"] },
        { name: "Things to do", features: ["Fitness center", "Hot tub", "Sauna", "Wi-Fi in public areas", "Spa", "Spa/Sauna", "Swiming Pool", "Tours"] },
        { name: "Accessbility", features: ["Wheelchair accessible"] },
        { name: "Getting around", features: ["Airport transfer", "Car park"] }
    ],
    [
        { name: "Cleanliness and safety", features: ["Anti-viral cleaning products", "Cashless payment service", "Daily disinfection in all rooms", "Daily disfection in common areas", "Face covering on staff", "First aid kit", "Guest rooms seal after sanitization", "Hand sanitiser", "Hotel room service app", "Hot water linen and Laundry washing", "Hygiene certification", "Physical distancing of at least 1 meter", "Professional-grade sanitizing service", "Protective screens in common areas", "Room sanitization opt-out available", "Rooms sanitized between stays", "Safe dining setup", "Sanitized kitchen and tableware items", "Shared stationery removed"] },

    ],
    [
        { name: "Dining,drinking and snacking", features: ["Bar", "Breakfast[buffet]", "Coffe shop", "Poolside bar", "Resturants", "Room service", "Snack bar"] },
        { name: "Services and conveniences", features: ["Air conditionig in public area", "Contactiess check-in/out", "Daily housekeeping", "Dry cleaning", "Elevator", "Facilities for disabled guests", "Food delivery", "Heating in public area", "Laundry service", "Luggage storage", "Meeting/banquet facilities", "Safety deposit boxes", "Smoke-free property", "Terrace", "Xeros/fax in business center"] }
    ],
    [
        { name: "Available in all rooms", features: ["Accessible by elebator", "Air conditioning", "Bathroom phone", "Closet", "Clothes rack", "Desk", "Hair dryer", "Heating", "In-room safe", "lines", "Mini bar", "Mirror", "Non-smoking", "Private bathroom", "Satelite/cable channels", "Shower", "Smoke detector", "Socket detector", "Socket near the bed", "Soundproofing", "Telephone"] }
    ],
];
</script>
  
<style scoped>
.facilities {
    max-width: 1120px;
    margin: auto;
    padding-top: 40px;
}

.faci-title {
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 600;
    font-size: 24px;
    line-height: 28.8px;
    letter-spacing: -2%;
    color: #010215;
}

.faci-object {
    display: flex;
    justify-content: space-between;
}

.group {
    margin-right: 20px;
}

.facility {
    margin-bottom: 20px;
}

.facility-name {
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 600;
    margin-bottom: 5px;
    margin-top: 30px;
    font-size: 14px;
}

.facility-features {
    list-style: none;
    padding-left: 0;
    font-family: "Plus Jakarta Sans", sans-serif;
    font-weight: 400;
    font-size: 14px;

}



.facility-features li {
    padding: 10px 10px 10px 0px;
    margin-bottom: 5px;
    border-bottom: 1px solid #F0EFF3;
}
</style>
   
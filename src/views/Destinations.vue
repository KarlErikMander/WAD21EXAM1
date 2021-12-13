<template>
  <div class="destinations">
    <h1> Our destinations</h1>
    <destination_comp :destinationList="$store.getters.destinationListDiscount" />
  </div>
</template>

<script>
import destination_comp from "@/components/destination_comp.vue";

export default {
  name: "Destinations",
  components: { destination_comp },
  data() {
    return {
      // destinationList: [
      //   { id: 1, from: "Tartu", to: "Tallinn", time: "02:15", distance: 180, price: 12, tickets: 7 },
      //   { id: 2, from: "Tartu", to: "Narva", time: "03:50", distance: 178, price: 13, tickets: 3 },
      //   { id: 3, from: "Tartu", to: "Riga", time: "04:00", distance: 244, price: 20, tickets: 2 },
      //   { id: 4, from: "Tallinn", to: "Tartu", time: "07:15", distance: 180, price: 15, tickets: 12 },
      //   { id: 5, from: "Tartu", to: "Vilnius", time: "09:15", distance: 540, price: 20, tickets: 16 }
      //]
    };
  }
};
</script>

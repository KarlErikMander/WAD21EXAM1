<template>
  <div id="destination-list-one">
    <div v-for="(singleDest, index) in destinationList" :key="index">
      <p>From {{singleDest["from"]}} to
        {{singleDest["to"]}} at {{singleDest["time"]}}
      with distance {{singleDest["distance"]}}km with price of {{singleDest["price"]}}€
      </p>
      <p>Tickets left: {{singleDest["tickets"]}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "destination_comp",
  props: {
    destinationList: {
      type: Array,
      required: true
    }
  },
  data: function() {
    return {};
  },

  computed: {},

  methods: {}

};
</script>


<style scoped>
.item {
  background: rgb(47, 255, 141);
  margin-bottom: 5px;
  padding: 3px 5px;
}

#comp-list-one {
  background: #d9b1ff;
  box-shadow: 1px 2px 3px rgba(0, 0, 0, 0.2);
  margin-bottom: 30px;
  padding: 10px 20px;
}

#comp-list-one ul {
  padding: 0;
}

#comp-list-one li {
  display: inline-block;
  margin-right: 10px;
  margin-top: 10px;
  padding: 20px;
  background: rgba(255, 255, 255, 0.7);
}

.price {
  font-weight: bold;
  color: #E8800C;
}
</style>

<template>
  <q-page padding>
    <div class="q-pa-md row items-stretch">

      <food v-for="food in foods" :key="food" :food="food"></food>


    </div>
  </q-page>
</template>

<script>
import Food from 'components/Food.vue';

export default {
  data() {
    return {
      foods: [
        {
          imageUrl: 'https://i.imgur.com/0umadnY.jpg',
          name: 'Burger',
          description: 'A burger is a sandwich consisting of one or more cooked patties of ground meat, usually beef, placed inside a sliced bread roll or bun.',
          deliciousness: 4
        },
        {
          imageUrl: 'https://i.imgur.com/0umadnY.jpg',
          name: 'Pizza',
          description: 'Pizza is a savory dish of Italian origin, consisting of a usually round, flattened base of leavened wheat-based dough.',
          deliciousness: 5
        },
        {
          imageUrl: 'https://i.imgur.com/0umadnY.jpg',
          name: 'Sprouts',
          description: 'The Brussels sprout is a member of the Gemmifera Group of cabbages, grown for its edible buds.',
          deliciousness: 1
        },
        {
          imageUrl: 'https://i.imgur.com/0umadnY.jpg',
          name: 'Kebab',
          description: 'Kebab turkey is a member lorem update doctor ',
          deliciousness: 4
        },
      ]
    }
  },
  components: {
    Food
  }
}
</script>

<style>
.card {
  flex-basis: 210px;
  border: 1px solid #ccc;
  border-radius: 5px;
  padding: 5px;
  margin-right: 10px;
  margin-bottom: 10px;
}

.card img {
  max-width: 100%;
}

.card-content {
  padding: 0 10px;
}

h1 {
  font-size: 23px;
}

p {
  font-size: 14px;
}
</style>

<template>

  <div id="app">
    <ul>
      <li v-for="(person, index) in people">
        {{ person }} - {{ index }}
      </li>
    </ul>

    <div v-for="(value, key, index) in catStats">
      <div>{{ index }} - {{ key }}: {{ value }}</div>
    </div>

    <div v-for="n in amountOfHorizontalRules">
      {{ n }}: <hr />
    </div>

  </div>
</template>

<script>
  export default {
    data() {
      return {
        people: ['Grace', 'Tim', 'Sergey'],
        catStats: {
          name: 'Opal',
          breed: 'Grey Tortoiseshell',
          favoriteThing: 'sleeping'
        },
        amountOfHorizontalRules: 46
      }
    }
  }
</script>
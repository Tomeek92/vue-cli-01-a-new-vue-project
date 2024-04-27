<template>
  <li>
    <h2>{{ name }}</h2>
    <button @click="toggleDetails">Show details</button>
    <ul v-if="detailsAreVisible">
      <li><strong>Phone:</strong> {{ phoneNumber }}</li>
      <li><strong>Email:</strong> {{ emailAddress }}</li>
    </ul>
  </li>
</template>
<script>
export default {
  props: ["name", "phoneNumber", "emailAddress"],
  data() {
    return {
      detailsAreVisible: false,
      friends: {
        id: "Andrzej",
        name: "Skonieczny",
        phone: "1234567",
        email: "AndrzejSkonczeny@wp.pl",
      },
    };
  },
  methods: {
    toggleDetails() {
      this.detailsAreVisible = !this.detailsAreVisible;
    },
  },
};
</script>

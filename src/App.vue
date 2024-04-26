<template>
  <section>
    <h2>My friends</h2>
    <ul>
      <li></li>
    </ul>
  </section>
</template>
<script>
export default {
  data() {
    return {
      friends: [
        {
          id: "Andrzej",
          name: "Skonieczny",
          phone: "1234567",
          email: "AndrzejSkonczeny@wp.pl",
        },
        {
          id: "Pietrek",
          name: "Skonieczny",
          phone: "1234567",
          email: "PietrekSkonczeny@wp.pl",
        },
      ],
    };
  },
};
</script>

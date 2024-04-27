<template>
  <section>
    <h2>My friends</h2>
    <ul>
      <friend-contact
        name="Andrzej"
        phone-number="123 456 789"
        email-address="wp.pl@pl"
      ></friend-contact>
      <friend-contact
        name="Rafał"
        phone-number="123 456 789"
        email-address="rafal123@wp.pl"
      ></friend-contact>
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

<template>
  <section>
    <h2>My friends</h2>
    <ul>
      <friend-contact
        v-for="friend in friends"
        :key="friend.id"
        :name="friend.name"
        :phone-number="friend.phone"
        :email-address="friend.email"
        :is-favorite="true"
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
          name: "Romano",
          phone: "12345678",
          email: "AndrzejSkonczeny@wp.pl",
        },
        {
          id: "Pietrek",
          name: "Pietrek",
          phone: "123456799999",
          email: "PietrekSkonczeny@wp.pl",
        },
      ],
    };
  },
};
</script>

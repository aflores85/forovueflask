<template>
  <div>
  <ul v-for="(Subject, index) in Subject" :key="index">
    <li>{{ Subject }}</li>
  </ul>
  </div>
</template>

<script>
export default {
  name: "ListaSubject",
  data() {
    return {
      Subject: [],
    };
  },
  methods: {
    getSubject() {
      fetch("http://localhost:5000/api/v1/getsubject")
        .then((response) => response.json())
        .then((data) => {
          this.Subject = data.Subject;
        });
    },
  },
  mounted() {
    this.getSubject();
  },
};
</script>
<style scoped></style>
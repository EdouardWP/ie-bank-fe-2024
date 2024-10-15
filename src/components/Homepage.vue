<template>
  <div class="homepage">
    <div class="jumbotron text-center">
      <div class="container">
        <h1 class="display-3">Welcome to IE Bank Corp</h1>
        <p class="lead">Your trusted partner for financial solutions.</p>
        <hr class="my-4" />
        <p>
          At IE Bank Corp, we offer a range of financial services to meet your needs. 
          Join us today and take control of your financial future.
        </p>
        <b-button variant="success" size="lg" @click="navigateToAccounts">
          Explore Accounts
        </b-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  methods: {
    navigateToAccounts() {
      // You can add navigation logic here
      this.$router.push("/accounts");
    },
  },
};
</script>

<style scoped>
.homepage {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #007bff; /* Bootstrap primary blue */
  color: white;
}

.jumbotron {
  background: rgba(255, 255, 255, 0.1);
  padding: 40px;
  border-radius: 10px;
}

h1 {
  font-size: 4rem;
  font-weight: bold;
}

.lead {
  font-size: 1.5rem;
  margin-bottom: 20px;
}

hr {
  border-top: 2px solid white;
}

b-button {
  font-size: 1.25rem;
}
</style>

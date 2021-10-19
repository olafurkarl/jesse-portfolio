<template>
  <div>
    <form @submit.prevent="handleSubmit(password)">
      <img src="~/assets/lock.svg">
      <br>
      <input
        ref="password"
        v-model="password"
        autofocus
        type="password"
        name="password"
        placeholder="Enter the magic words"
        class="form-control"
      >

      <button class="btn btn-primary">
        Open Sesame
      </button>
    </form>
  </div>
</template>

<script>
export default {
  computed: {
    todos () {
      return this.$store.state.todos.list
    }
  },
  mounted () {
    this.$refs.password.focus()
  },
  methods: {
    handleSubmit (password) {
      if (password === 'dovetail') {
        this.$store.commit('login/login')
      }
    }
  }
}
</script>

<style scoped>
form {
    text-align: center;
    margin-top: 5em;
}

img {
    margin-bottom: 40px;
    margin-top: 3em;
}

button {
    background: #003C72;
    width: 191px;
    height: 60px;
    color: white;
    font-size: 20px;
    font-weight: 600;
    text-indent: 0;
    padding: 0;
    border: none;
    border-radius: 4px;
    font-family: 'Montserrat';
}

input {
    width: 621px;
    height: 60px;
    border: solid 4px #003C72;
    border-radius: 4px;
    font-family: Lato;
    font-size: 20px;
    padding: 18px;
}

::placeholder {
    color: #C4C4C4;
    opacity: 1; /* Firefox */
    font-family: Lato;
    font-size: 20px;
}

</style>

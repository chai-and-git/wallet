<template>
  <div class="modal-overlay">
    <div class="modal">
      <form @submit.prevent="handleSubmit">
        <input v-model="form.name" type="text" name="cardName" placeholder="Enter card name" required />
        <button type="submit">Add Card</button>
      </form>
    </div>
    <div class="close" @click="$emit('close-modal')">
      X
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      form: {
        name: ''
      }
    }
  },
  methods: {
    handleSubmit(e) {
      if (this.form.name) {
        const cardNumber = Math.floor(1000 + Math.random() * 9000);
        localStorage.setItem("cardName", this.form.name)
        localStorage.setItem("cardNumber", cardNumber)
        const expiry = this.generateRandomDate();
        localStorage.setItem("cardExpiry", `${expiry.getMonth}/${expiry.getFullYear}`)
      }
    },
    generateRandomDate: () => {
      const now = new Date();
      const expiry = new Date(new Date().setFullYear(new Date().getFullYear() + 10));
      return new Date(from.getTime() + Math.random() * (to.getTime() - from.getTime()));
    }
  }
}
</script>
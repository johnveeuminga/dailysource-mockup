<template>
  <form action="#" class='newsletter-form'>
    <div class="form-group">
      <input type="text" class="form-control" placeholder='Enter your email'>
    </div>
    <div class="form-group newsletter-form__time d-flex align-items-center justify-content-between">
      <p>Send it at</p>
      <select class="custom-select newsletter-form__time-input form-control">
        <option selected>9AM</option>
      </select>
      <select class="custom-select newsletter-form__time-zone form-control">
        <option selected> GMT -05:00: Eastern Time </option>
      </select>
    </div>
    <div class="btn-container text-right">
      <button class="btn btn-primary text-uppercase">Submit</button>
    </div>
  </form>
</template>

<script>
export default {
  name: 'NewsletterForm'
}
</script>

<style lang='scss' scoped>
.newsletter-form {
  &__time {
    p {
      font-size: 20px;
      margin-bottom: 0;
    }
  }
  &__time-input {
    max-width: 95px;
  }

  &__time-zone {
    max-width: 295px;
  }
}
</style>

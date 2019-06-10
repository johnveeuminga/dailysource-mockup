<template>
  <form action="#" class='newsletter-form'>
    <div class="form-group">
      <input type="text" class="form-control" placeholder='Enter your email'>
    </div>
    <div class="d-flex align-items-center">
      <div class="form-group mb-0 newsletter-form__time d-flex align-items-center justify-content-start">
        <p>Send it at</p>
        <select class="custom-select newsletter-form__time-input form-control">
          <option selected>9AM</option>
        </select>
        <select class="custom-select newsletter-form__time-zone form-control">
          <option selected> GMT -05:00: Eastern Time </option>
        </select>
      </div>
      <div class="btn-container text-right">
        <button class="btn d-block btn-primary text-uppercase">Submit</button>
      </div>
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

  display: block;
  &__time {
    flex-grow: 1;
    flex-shrink: 0;
    p {
      font-size: 20px;
      margin-bottom: 0;
      margin-right: .375em;
    }
  }

  .form-group {
    margin-bottom: 1.25rem;
  }

  &__time-input {
    max-width: 80px;
    margin-right: .375em;
  }

  &__time-zone {
    max-width: 225px;
  }

  .btn-container {
    flex-grow: 1;

    .btn {
      width: 100%;
    }
  }
}
</style>

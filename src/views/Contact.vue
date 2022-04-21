<template>
  <div class="container">
    <div class="row">
      <div class="mb-3 col">
        <label for="firstname" class="form-label">Prénom</label>
        <input
          type="text"
          class="form-control"
          id="firstname"
          placeholder="Votre prénom"
        />
      </div>
      <div class="mb-3 col">
        <label for="lastname" class="form-label">Nom</label>
        <input
          type="text"
          class="form-control"
          id="lastname"
          placeholder="Votre nom"
        />
      </div>
    </div>
    <div class="mb-3 col">
      <label for="email" class="form-label">Email</label>
      <input type="email" class="form-control" id="email" placeholder="Email" />
    </div>
    <div class="mb-3">
      <label for="message" class="form-label">Votre message</label>
      <textarea
        class="form-control"
        id="message"
        rows="5"
        placeholder="Ecrivez votre message"
      ></textarea>
    </div>
    <div class="d-flex justify-content-center">
      <button type="button" class="btn btn-primary btn-lg">Envoyer</button>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    document.body.classList.add('contact-bg');
  },
  unmounted() {
    document.body.classList.remove('contact-bg');
  }
};
</script>

<style>
.container {
  min-height: calc(100vh - 396px);
  margin-top: 140px;
}
.form-label {
    background: #fff;
    border: 2px solid #3E5902;
    color: #3E5902;
    padding: 5px 10px;
    box-shadow: 4px 8px 10px 3px rgb(0 0 0 / 40%);
}
.btn-primary {
  background: #3E5902;
  border: 2px solid #fff;
  color: #fff;
  box-shadow: 4px 8px 10px 3px rgb(0 0 0 / 40%);
}
.btn-primary:hover{
  background-color: #344808;
  border-color: #344808;
}
</style>
<template>
  <div
    class="bg-image"
    style="
      background-image: url('https://mdbcdn.b-cdn.net/img/Photos/Others/images/76.jpg');
      height: 120vh;
    "
  >
    <div class="container text-center" style="text-align: center">
      <h1>Home</h1>

      <center>
        <tr>
          <th>
            <p>My Profile</p>
            <button @click="goProfile()">
              <img
                src="https://uploads.codesandbox.io/uploads/user/761cc845-c457-4b86-a7bf-9179aeba1f52/f8QX-profile.png"
                height="45"
                width="45"
              />
            </button>
          </th>

          <h1>|</h1>

          <th>
            <p>Contact</p>
            <button @click="goContact()">
              <img
                src="https://uploads.codesandbox.io/uploads/user/761cc845-c457-4b86-a7bf-9179aeba1f52/gNE1-contact.png"
                height="45"
                width="45"
              />
            </button>
          </th>
        </tr>
      </center>
      <br />
      <iframe
        src="https://giphy.com/embed/Cmr1OMJ2FN0B2"
        width="300"
        height="300"
        frameBorder="0"
        class="giphy-embed"
        allowFullScreen
      ></iframe>
    </div>
  </div>
</template>


<script>
export default {
  methods: {
    goContact() {
      this.$router.push("/contact");
    },
    goProfile() {
      this.$router.push("/profile");
    },
  },
};
</script>

<style scoped>
h1 {
  font-size: 2em;
  text-align: center;
}
p {
  font-size: 20px;
}
</style>
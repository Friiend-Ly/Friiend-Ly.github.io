<template>
  <div id="app">
    <Header :title="title"/>
    <div class="container d-flex container-box">
      <UserInputElements 
        :formData="formData"
        @changeFormData="changeFormData($event)"
      />
      <GeneratedCard :formData="formData"/>
    </div>
  </div>
</template>
<style> 
@import url('https://fonts.googleapis.com/css2?family=Lato&family=Roboto+Serif:wght@100&display=swap');
</style>

<script>
import Header from "./components/Header.vue";
import UserInputElements from "./components/UserInput.vue";
import GeneratedCard from "./components/GeneratedCard.vue";
export default {
  name: "App",
  components: {
    Header,
    UserInputElements,
    GeneratedCard
  },
  data() {
    return {
      title: 'ID Card Generator',
      formData: {
        fullName: "",
        clubName: "",
        licenceNum:"",
        groupeSanguin:"",
        email:"",
        phoneNum:"",
        locationName:""

      }
    }
  },
  methods: {
    changeFormData(keyObject) {
      this.formData = Object.assign(this.formData, keyObject);
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
:root {
  --bg-official: #4047f0;
  --font-body: "Montserrat", sans-serif;
}
.subtitle-section {
  color: var(--bg-official);
  font-family: var(--font-body);
  font-weight: 600;
  font-size: 25px;
}

.subtitle-card {
  font-family: var(--font-body);
  font-weight: 600;
  font-size: 25px;
}

.text-center {
  text-align: center;
}

.container-general {
  display: flex;
  align-items: center;
}

.section-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  border: 1px solid #c8c8c8;
}

.section-left {
  border-bottom-left-radius: 16px;
}

.section-right {
  border-bottom-right-radius: 16px;
}

.container-box {
  padding-left: 0;
  padding-right: 0;
}

.form-element {
  margin: 5px;
  min-width: 200px;
}

.form-box {
  width: 100%;
  max-width: 285px;
}

.form-label {
  min-width: 150px;
  display: block;
  font-family: var(--font-body);
  font-weight: 600;
}

.form-input {
  display: block;
  border: 1px solid #c4b4b4;
  border-radius: 10px;
  height: 40px;
  padding: 5px 10px 5px 40px;
}

.font-icon {
  position: relati    ve;
}

.font-icon i {
  position: absolute;
  left: 15px;
  top: 45px;
  color: #000;
}

.btn-generate {
  border: none;
  border-radius: 10px;
  background-color: var(--bg-official);
  color: #fff;
  font-family: var(--font-body);
  font-weight: bold;
  padding: 0.5em;
  margin-top: 1em;
}

.id-card-container {
  display: block;
  width: 100%;
  
}

.card-container {
  width: 100%;
  border-radius: 10px;
  font-family: var(--font-body);
  display: flex;
  align-items: center;
  justify-content: center;
  max-width: 450px;
  font-family: 'Lato', sans-serif;
  
}

.card-title {
  font-size: 16px;
  
  font-weight: bold;
}

.card-input {
  font-size: 16px;
  font-weight: bold;
}

.card-wrapper {
  width: 100%;
  background-color: #fff;
  background: linear-gradient(#f8f8f8, #fff);
  box-shadow: 0 8px 16px -8px rgba(0, 0, 0, 0.4);
  border-radius: 10px;
  overflow: hidden;
  position: relative;
  margin: 1.5rem;
  display: flex;
  padding-top: 100px;
  background-image: url('./assets/bg.png');
  background-size: cover;

}

.user-card {
   display: inline-block;
  padding: 8px;
  background: #000;
  margin: auto;
  border-radius: 50%;
  background-size: 200% 200%;
  animation: animated-gradient 2s linear infinite;
}



.user-photo {
  display: block;
  width: 120px;
  height: 120px;
  border-radius: 50%;
  background-image: url('./assets/Chap Blue CV.png');
  background-size: cover;
  
}

.card-element {
  margin-left: 10px;
  margin-bottom: 15px;
}

.card-name {
  font-size: 1.5rem;
}

.college-name {
  font-size: 1.2rem;
  color: #000!;
}







.profile-card{
  width: 400px;
  text-align: center;
  overflow: hidden;
  padding-top: 75PX;
  color: #000;
}

.dafont{
  color: #fff;
  font-size: 1.4rem;
}


</style>



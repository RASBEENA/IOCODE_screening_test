<template>
    <section id="main-section">
      <h1>We make great digital <span style="color: #01F28D">products</span> for innovative brands. </h1>
      <p class="p-style">Get your desired design services from our talented designers, around the world at a reasonable cost</p>
  
      <form action="/" class="inline">
        <div class="input-icons">
          <i class="fa-solid fa-envelope icon input-field-color"></i>
          <input type="email" id="email" v-model="email" name="email" @input="validateEmail" class="textfield-shape input-field input-field-color" placeholder="Your work email">
          <button type="submit" class="btn btn-success btn-style" @click='buttonToCall'>Book a call</button>
        </div>
      </form>
      <p class="para-font-size">4.6/5.0 <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i> 15+ Businesses, 35+ Happy clients</p>
    </section>
  </template>
  
  <script>
  export default {
    name: 'MainSection',

    data() {
      return {
        email: '',
      }
    },
    methods: {
        buttonToCall(){
            const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!this.email) {
            console.log('email required');
        } else if (!emailPattern.test(this.email)){
            console.log('invalid email format');
        } else {
            console.log(this.email);
      }

        },
        
    }
  };
  </script>

 
  
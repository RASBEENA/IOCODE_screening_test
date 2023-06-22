

<template>
    <nav class="navbar navbar-expand-lg navbar-dark">
      <a class="navbar-brand sample-color">Sample</a>
  
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
  
      <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link sample-color" href="#footer">Home</a>
          </li>
          <li class="nav-item dropdown" v-click-outside="closeDropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" @click="toggleDropdown" aria-haspopup="true" :aria-expanded="isDropdownOpen.toString()">
              Case Studies
            </a>
            <div class="dropdown-menu" :class="{ show: isDropdownOpen }">
              <a class="dropdown-item" href="#">Action 1</a>
              <a class="dropdown-item" href="#">Action 2</a>
              <a class="dropdown-item" href="#">Action 3</a>
            </div>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="">Blog</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="">About Us</a>
          </li>
          
          <button type="button" class="btn btn-success" @click='buttonClicked' >Book a call</button>
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavBar',
    data() {
      return {
        isDropdownOpen: false,
      };
    },
    methods: {
      toggleDropdown() {
        this.isDropdownOpen = !this.isDropdownOpen;
      },
      closeDropdown() {
        this.isDropdownOpen = false;
      },
      buttonClicked() {
        console.log("call booked");
      },
    },
    
  };
  </script>
  
 
  
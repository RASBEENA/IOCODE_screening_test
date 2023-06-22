
<template>
  <div class="container-fluid">
    <NavBar />
    <MainSection />
   <FooterSection />

  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import MainSection from './components/MainSection.vue';
import FooterSection from './components/FooterSection.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    MainSection,
    FooterSection,
  },
};
</script>

<style>
body {
    font-family: "Montserrat";
    text-align: center;
    background-color: #1E1E1E;;
}

h1 {
    font-family: 'Darker Grotesque';
    font-weight: 900;
    color: #E8FFF5;
    font-style: normal;
    font-size: 3.5rem;
    text-align: center;
    padding:0% 20% 1%;
  
}
p {
    color:  #D1FFEB;
    font-weight: 300;
    font-size: 15px;
    align-items: center;
    text-align: center;
   
}


.container-fluid {
    padding: 2% 10%;
    
}
#title .container-fluid {
    padding:3% 7% 10%;
    text-align: left;
}
/* nav bar */
.navbar {
    padding-bottom: 4.5rem;
}

.navbar-brand {
    font-family: 'Darker Grotesque';
    font-size: 1rem;
    font-weight: 900;
    font-size: 25px;
}
.nav-item {
    padding: 0 18px;
}
.nav-link {
    font-family: "Montserrat";
    font-size: .8rem;
    font-weight:light;
     color: #E8FFF5;
}
.btn {
    border-radius: 1.5em;
    background-color:  #01F28D;
    ;
}
.textfield-shape {
    border-radius: 1.5em;
}

.big-heading {
    
    font-size: 2.5rem;
    line-height: 1.5;
    font-weight: 900;  
}
.item-color {
    color: #198754;
    font-weight: bold;
    
}
.fa-star {
    color:  #FDB022;
    margin: 3px;

}


.input-icons i {
    position: absolute;
}
  
.input-icons {
    width: 100%;
    margin-bottom: 10px;
}
  
.icon {
    padding: 10px;
    min-width: 40px;
}
  
.input-field {
    width: 20%;
    padding: 10px;
    text-align: center;
}
.sample-color {
    color: #02FF95;

}
.service-color {
    color: #01F38D;

}
.para-font-size {
    font-size: 13px;
}
.description {
margin-left: 50px;
 margin-right: 50px;


}  
.btn-style {
   margin-left: 10px;
}
#main-section {
  padding-left: 20px ;
  padding-right: 20px;
  padding-bottom: 30px;
}
.p-style { 
    
    padding:0% 30% 1%;
}

</style>
<template>
    <nav id="nav">
      <router-link id="logo-url" to="/"><img :src="logo" :alt="alt" id="logo"></router-link>
      <router-link to="/">Home</router-link> 
      <router-link to="/Pedidos">About</router-link>
    </nav>
  </template>
  
  <script>
  export default {
    name: "Navbar",
    props: ["logo", "alt"],
  };
  </script>
  
  <style scoped>
  #nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    
  }
  
  #logo {
    width: 40px;
    height: 40px;
  }

  #nav #logo-url{
    margin: auto;
    margin-left: 0px
  }

  #nav a{
    color: #FCBA03;
    text-decoration: none;
    margin: 12px;
    transition:.5s; 
    }

    #nav a:hover{
        color: #FFF;
    }
  </style>
  
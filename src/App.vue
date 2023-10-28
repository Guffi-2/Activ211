<script setup lang="ts">

</script>

<template>
  <header>
    <img src="./On.PNG" class="logo vue" alt="Vue logo" />
    <h2>Актив школы 211</h2>
    <menu>
      <h4 id="about">О нас</h4>
      <h4 id="news">Новоcти</h4>
      <h4 id="soc-seti">Соц-сети</h4>
    </menu>
  </header>
  <mobileMenu>
      <h4 id="about_m">О нас</h4>
      <h4 id="news_m">Новоcти</h4>
      <h4 id="soc-seti_m">Соц-сети</h4>
  </mobileMenu>
  <news>
    <h2 id="news_p">Новости</h2>
  <news_p>
   
    <div class="post_1">
      
    </div>
  </news_p>
</news>
</template>

<style scoped>
#news_p{
  padding-top: 0px;
  padding-left: 30px;
  font-size: 1.6rem; 
}
#soc-seti{
  padding-left: 20px;
}
#about{
  padding-right: 20px;
}
.logo {
  height: 5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo.vue {
  /* */
  margin: none;
}
menu{
  width: 55%;
  height: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.logo.vue:hover {
  filter: drop-shadow(0 0 0.4em #b90000); /* #a5a5a5*/
}
mobileMenu{
  width: 100%;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: none;
  padding: none;
  background-color: #eeeeee;
  display: none;
}
header{
  width: 100%;
  height: 85px;
  display: flex;
  justify-content: left;
  align-items: center;
  margin: none;
  padding: none;
}

@media (min-width: 1200px) {
  h2 { 
    font-size: 1.5vw;
  }
  h4{
    font-size: 1.3vw;
  }
  .logo {
  height: 5em;
  will-change: filter;
  transition: filter 300ms;
  }
  #about_m{
    visibility: hidden;
  }
  #news_m{
    visibility: hidden;
  }
  #soc-seti_m{
    visibility: hidden;
  }
  mobileMenu{
    visibility: hidden;
    display: none;
  }
}
@media (max-width: 1199px) and (min-width: 900px) {
  h2 { 
    font-size: 1rem; 
  }
  #about_m{
    visibility: hidden;
  }
  #news_m{
    visibility: hidden;
  }
  #soc-seti_m{
    visibility: hidden;
  }
  mobileMenu{
    visibility: hidden;
    display: none;
  }
}

@media (max-width: 899px) {
  h2 { 
    font-size: 1.3rem; 
  }
  mobileMenu{
    display: flex;
  }
  .logo {
  height: 4em;
  will-change: filter;
  transition: filter 300ms;
  }
  header h2{
    width: 55%;
    height: 85px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  #about{
    visibility: hidden;
  }
  #news{
    visibility: hidden;
  }
  #soc-seti{
    visibility: hidden;
    
  }

  #about_m{
    padding-right: 20px;
  }
  #news_m{
    padding-right: 20px;
  }
  menu{
    display: none;
  }
  news{
    padding-top: 20px;
    width: 100%;
    height: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  #news_p{
  padding-top: 0px;
  padding-left: 0px;
  font-size: 1.6rem; 
}
}
</style>

<script  lang="ts">
  import Countdown from "../components/Countdown.svelte";
	import Icons from '../components/Icons.svelte';
</script>

<div class="Main">
  <div class="header">
    <div class="prestDisney">
      <h3 >Disney presenta oooo</h3>
    </div>
    <!-- <img src="../public/images/background4.png"  class="imgMoana" alt=""> -->
    <!-- <div class="principal" >
      <a class="name" href="https://fontmeme.com/disney-font/"><img src="https://fontmeme.com/permalink/220902/13aac854a6aa362f3a276698ec031f69.png" alt="disney-font" border="0"></a>
    </div> -->
  
    <div class="name">
      <img src="../public/images/moana.png"  class="imgMoana" alt="">
    </div>
   
    <!-- <div class="disney">
      <Icons value='disney' />
      <img src="../public/images/icons8-películas-disney-50.png" alt="disney" > 
    </div> -->
     <h3>Mis 7 años</h3> 
  </div>
  <div class="prueba">
    <div>
      <p>Te invita a su fiesta
        de Cumpleaños
        en... 
        <br>
          Destellos Eventos
      </p> 
    </div>
    <div>
      <p>¿Cuando?</p>
      Domingo 23 de octubre de 2022
      <br>
      17:00 hs
    </div>
    
    <div class="Countdown">
      <Countdown/>
    </div>
      
  </div>
</div>
<style>
    .Main {
      margin-top: -0px;
      width: 100%; 
      height: 100%; 
      /* background-color: rgba(17, 61, 208, 0.5); */
      justify-content: center;
      align-items: center;
      text-align: center;
      
    } 
    /* .Main .header{
      margin-top: 50px;
      margin-bottom:200px;
    } */
    .Main .header .prestDisney{
      top: 0px;
      width: 100%;
      text-align: center;
      /* position: absolute; */
      z-index: 1;
    }
    .Main .header .prestDisney h3{
      font-family: Moanas;
        color:var(--secondary-background);
      font-size: 90%;
    }
    .Main .header .imgMoana{
      width: 100%;
    }
    .Main .header .name{
      /* background-color: rgba(191, 245, 253, 0.5); */
      width: 100%;
      text-align: center;
      align-items: center;
      /* position: absolute; */
      top: 500px;
      /* font-size: 60px; */
      /* animation: nameM 5s; */
    }
    /* .disney{
      text-align:center;
      position: absolute;
      top: 0;
      animation: imgM 3s;
      z-index: -1; 
      width:100px;
      margin-top: 45px;
    } */
    /* .disney img{
     
    } */
/* 
    .prueba{
      animation: fade 8s;
    }  */
    .Countdown{
      text-align: center;
      align-items: center;
    }
    @keyframes fade {
    0% {
      opacity: 0;
      
    }
    30% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  } 

  @keyframes nameM {
    0% {
      opacity: 0;
    }
    30% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  } 
  @keyframes imgM {
    0% {
      opacity: 0;
    }
    30% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  } 
    /* .Main-container {
      display: grid;
      grid-template-columns: 3fr 1fr;
      grid-gap: 2em;
      padding: 2em 0;
    } */
</style>

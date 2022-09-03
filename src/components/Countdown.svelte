<script lang="ts">
  export let dateCountdown = "Oct 23, 2022 17:00:00";

  const second = 1000,
      minute = second * 60,
      hour = minute * 60,
      day = hour * 24;

    let countDown = new Date(dateCountdown).getTime(),
    x = setInterval(function() {

      let now = new Date().getTime(),
          distance = countDown - now;

      document.getElementById('dias').innerText = Math.floor(distance / (day)),
        document.getElementById('horas').innerText = Math.floor((distance % (day)) / (hour)),
        document.getElementById('minutos').innerText = Math.floor((distance % (hour)) / (minute)),
        document.getElementById('segundos').innerText = Math.floor((distance % (minute)) / second);

    }, second)
</script>

<div class="contenedor">
      <div class="cartel">
        <div id="dias" />
        <div class="h3"><h3>Días</h3></div>
      </div>
      <div class="cartel">
        <div id="horas" />
        <div class="h3"><h3>Horas</h3></div>
      </div>
      <div class="cartel">
        <div id="minutos" />
        <div class="h3"><h3>Minutos</h3></div>
      </div>
      <div class="cartel">
        <div id="segundos" />
        <div class="h3"><h3>Segundos</h3></div>
      </div>
</div>


<style>
    .contenedor{       
        width: 100%;
        text-align: center;
        align-items: center;
    }
  .cartel {
    width: 16%;
    height: 50px;
    padding-top: 10px;
    text-align: center;
    display: inline-block;
    margin: 0px 2px;
    border: 3px solid var(--secondary-background);
    border-radius: 50%;
  }
  .cartel > div {
    font-size: 15px;
    animation: fade 3s;
    margin-top: 5px;
  }
  .cartel > div > h3 {
    margin-top: 5px;
    font-size: 10px;
    font-weight: normal;
  }
  .h3 {
    bottom: 0;
    margin: 0 auto;
  }
  .contenedor {
    margin-top: 3%;
  }
  
   /* li {
    display: inline-block;
    font-size: 1.5em;
    list-style-type: none;
    padding: 1em;
    text-transform: uppercase;
  }
  li span {
    display: block;
    font-size: 4.5rem;
  }
  .numeros {
    font-family: "Chela one", sans-serif;
    font-size: 60px;
    transition: 0.3s;
    animation-name: fade;
    animation-duration: 3s;
  } .responsivo1 {
  display: inline-block
}
.responsivo2 {
  display: inline-block
}   */
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
</style>

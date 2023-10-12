<script>
  import Saos from "saos";
</script>

<div id="studies">
  <img class="star num1" src="/images/Stars.png" alt="" />
  <div class="container">
    <img
      src="/images/curvy_bottom_arrow.png"
      alt="vertical-arrow-drawing"
      class="arrow"
    />
    <div class="content">
      <Saos
        animation={"tilt-in-fwd-tr 0.6s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
        animation_out={"flip-out-hor-top 0.45s cubic-bezier(0.550, 0.085, 0.680, 0.530) both"}
        top={250}
        bottom={250}
        class="step"
      >
        <p>
          2014-2018 : Psychology studies <br /> Campus Lettres & Sciences
          Humaines <br />1 Boulevard Albert 1er, 54000 Nancy
        </p>
        <h2>2018 : Graduated from Psychology (Master degree)</h2>
      </Saos>
      <Saos
        animation={"tilt-in-fwd-tr 0.6s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
        animation_out={"flip-out-hor-top 0.45s cubic-bezier(0.550, 0.085, 0.680, 0.530) both"}
        top={250}
        bottom={250}
        class="step"
      >
        <p>
          2021-2022 : Web Dev Formation <br /> Alaji <br />6 route de
          l'aviation, 54600 Villers-lès-Nancy
        </p>
        <h2>2022 : Obtainerd my BTEC equivalent</h2>
      </Saos>
      <Saos
        animation={"tilt-in-fwd-tr 0.6s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
        animation_out={"flip-out-hor-top 0.45s cubic-bezier(0.550, 0.085, 0.680, 0.530) both"}
        top={250}
        bottom={250}
        class="step"
      >
        <p>
          2022-2026: Developer Architect Formation <br />Epitech <br />80 rue
          Saint Georges, 54000 Nancy
        </p>
        <h2>More to come...</h2>
      </Saos>
    </div>
  </div>
  <img class="star num2" src="/images/Stars.png" alt="" />
</div>

<style>
  @keyframes -global-flip-out-hor-top {
    0% {
      transform: rotateX(0);
      opacity: 1;
    }
    100% {
      transform: rotateX(70deg);
      opacity: 0;
    }
  }


  @keyframes -global-tilt-in-fwd-tr {
    0% {
      transform: rotateY(20deg) rotateX(35deg) translate(300px, -300px)
        skew(-35deg, 10deg);
      opacity: 0;
    }
    100% {
      transform: rotateY(0) rotateX(0deg) translate(0, 0) skew(0deg, 0deg);
      opacity: 1;
    }
  }

  #studies {
    width: 80%;
    margin: 5em auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .container {
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
  }

  h2 {
    font-size: 1.5em;
    margin: 0;
    padding: 0;
    background: linear-gradient(
      90deg,
      #d355ff 0%,
      #ed7fc0 54.23%,
      #dba6f4 99.17%
    );
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  p {
    font-size: 1.2em;
  }

  .star {
    z-index: 0;
  }

  .num1 {
    align-self: flex-end;
  }

  .num2 {
    align-self: flex-start;
    margin-left: 10em;
  }

  @media(max-width: 800px){
    .num2 {
      margin-left: 0;
    }
    p{
        font-size: 1em;
    }
    h2{
        font-size: 1.2em;
    }
    .arrow{
        height: 60vh;
        width: 5em;
        margin-right: 1em;
    }

    .star{
        height: 6em;
    }
  }
</style>

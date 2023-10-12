<div class="home">
  <img
    class="alien-avatar"
    src="/images/Avatar.jpg"
    alt="avatar-alien"
    srcset=""
  />
  <h1>Hi. I'm Clementine, a web developer, and this is my portfolio.</h1>
  <img class="curly-line" src="/images/curly_line.png" alt="curly_line" />
</div>

<style>
  .home {
    height: calc(100vh - 1rem);
    display: grid;
    grid-template-rows: 1fr 1fr 1fr;
    margin-top: 5em;
    
  }
  .alien-avatar {
    width: 10em;
    height: 10em;
    border-radius: 50%;
    margin: auto;
    display: block;
    z-index: 999;
  }

  h1 {
    background: linear-gradient(180deg, #81f1c9 0%, #eb34a0 100%);
    background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 4em;
    text-align: center;
    z-index: 999;
    margin: 0 4em;
    animation: fade-in 1.5s ease-in-out;
  }

  @keyframes fade-in {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
  .curly-line {
    width: 60%;
    margin: auto;
    z-index: 1;
  }

  @media(max-width : 1300px){
    h1{
      font-size: 3em;
      margin: 0 2em;
    }
  }

  @media(max-width : 1000px){
    h1{
      font-size: 2em;
      margin: 0 1em;
    }
  }
  
</style>

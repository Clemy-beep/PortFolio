<script>
  import emblaCarouselSvelte from "embla-carousel-svelte";

  let srcs = [
    "/images/a_n.jpg",
    "/images/cmdb.png",
    "/images/udr_milestone.png",
  ];

  let descriptions = [
    "Alfred & Nestor is my first project and my first experience of being a develope. I contributed to this project firstly by adding content to the website (React) and mostly by creating the web application with the team already in place and developing the user interface (Flutter).",

    "CMDB is the project I made for my presentation at the end of my web dev formation. <br/> It is a social media all about movies. Largely inspired by The Movie Database and IMDB you can write reviews about movies and share them with other users, follow users and comment other reviews.",

    "Milestone is a project i realized for the Union des Rôlistes association. It is a todo list web-app destined to the users who which to know about the association current projects and streamers who collaborate with the association to see  upcoming streaming events.",
  ];


</script>

<div id="exp">
  <h2>Experiences and projects <img class="arrow" src="/images/scroll_to_arrow.png" alt="" /></h2>
  <p class="subtitle">Slide it !</p>
  <div class="embla__viewport">
    <div class="embla" use:emblaCarouselSvelte>
      <div class="embla__container">
        {#each srcs as src, i}
          <div class="embla__slide">
            <img {src} alt="" />
            <div class="description">
              <p>{descriptions[i]}</p>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
</div>

<style>
  #exp {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 70%;
    margin: auto;
  }
  .embla {
    overflow: hidden;
  }
  .embla__container {
    display: flex;
  }
  .embla__slide {
    flex: 0 0 100%;
    min-width: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  img {
    width: 100%;
    object-fit: cover;
    border-radius: 30px;
  }

  h2 {
    background: linear-gradient(90deg, #ed7fc0 3.25%, #81f1c9 100%);
    background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 2em;
    text-align: center;
  }

  .arrow {
    width: 2em;
    display: inline;
    transform: rotate(90deg);
    vertical-align: middle;
    margin-left: 1em;
  }

  .subtitle{
    text-align: center;
    font-size: 1.2em;
    padding: 0;
    margin: 0;
  }

  @media(max-width: 800px){
    #exp{
      width: 90%;
    }
    .subtitle{
      font-size: 1em;
    }
    h2{
        font-size: 1.5em;
    }
  }

  @media(min-width: 1300px){
    .embla__slide img{
        width: 50%;
    }

    .embla__slide p{
        font-size: 1.3em;
        width: 50%;
        margin: auto;
        padding-top: 0.5em;
    }
  }
</style>


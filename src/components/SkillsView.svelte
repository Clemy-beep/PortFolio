<script>
  import Saos from "saos";
  let skills = [
   {
    name: "UX design",
    link: "https://www.interaction-design.org/literature/topics/ux-design"
   },
    {
        name: "UI design",
        link: "https://www.interaction-design.org/literature/topics/ui-design"
    },
    {
        name: "Dynamic front dev",
        link: "https://www.hughesandco.ca/blog/the-difference-between-dynamic-and-static-websites"
    },
    {
        name: "Static front dev",
        link: "https://www.hughesandco.ca/blog/the-difference-between-dynamic-and-static-websites"
    },
    {
        name: "Database design",
        link: "https://en.wikipedia.org/wiki/Database_design"
    },
    {
        name: "Containerization",
        link: "https://www.redhat.com/en/topics/cloud-native-apps/what-is-containerization"
    },
    {
        name: "Deployment",
        link: "https://www.sumologic.com/glossary/software-deployment/"
    },
    {
        name: "API development",
        link: "https://www.redhat.com/en/topics/api/what-are-application-programming-interfaces"
    },
    {
        name: "Version control",
        link: "https://en.wikipedia.org/wiki/Version_control"
    }
  ];

  let languages = [
    {
        name: "HTML5",
        link: "https://developer.mozilla.org/en-US/docs/Glossary/HTML5"
    },
    {
        name: "CSS3",
        link: "https://developer.mozilla.org/en-US/docs/Web/CSS"
    },
    {
        name: "JavaScript",
        link: "https://developer.mozilla.org/en-US/docs/Glossary/JavaScript"
    },
    {
        name: "TypeScript",
        link: "https://www.typescriptlang.org/"
    },
    {
        name:"Dart",
        link: "https://dart.dev/"
    },
    {
        name: "PHP",
        link: "https://www.php.net/"
    },
    {
        name: "SQL",
        link: "https://www.w3schools.com/sql/"   
    },
    {
        name: "Shell",
        link: "https://www.shellscript.sh/"
    },
    {
        name: "Python",
        link: "https://www.python.org/"
    },
    {
        name: "Java",
        link: "https://www.java.com/en/"
    },
  ];

  let toolsAndFrameworks = [
    {
        name: "Svelte",
        link: "https://svelte.dev/"
    },
    {
        name: "React",
        link: "https://reactjs.org/"
    },
    {
        name: "VueJS",
        link: "https://vuejs.org/"
    },
    {
        name: "NuxtJs",
        link: "https://nuxtjs.org/"
    },
    {
        name: "Flutter",
        link: "https://flutter.dev/"
    },
    {
        name: "Django",
        link: "https://www.djangoproject.com/"
    },
    {
        name: "Symphony",
        link: "https://symfony.com/"
    },
    {
        name: "NodeJS",
        link: "https://nodejs.org/en/"
    },
    {
        name: "Express",
        link: "https://expressjs.com/"
    },
    {
        name: "Prisma",
        link: "https://www.prisma.io/"
    },
    {
        name: "Docker",
        link: "https://www.docker.com/"
    },
    {
        name: "Github",
        link: "https://github.com/"
    },
    {
        name:"Draw.io",
        link: "https://app.diagrams.net/"
    },
    {
        name: "Figma",
        link: "https://www.figma.com/"
    },
    {
        name: "DBeaver",
        link: "https://dbeaver.io/"
    },
    {
        name: "VSCode",
        link: "https://code.visualstudio.com/"
    },
    {
        name: "Android Studio",
        link: "https://developer.android.com/studio"
    },
    {
        name: "Postman",
        link: "https://www.postman.com/"
    },
  ];
</script>

<div id="skills">
  <img src="/images/Stars.png" alt="" class="star1" />
  <div class="skills-container">
    <h2>Skills</h2>
    <div class="skills">
      {#each skills as skill}
        <Saos
          class="skill"
          animation={"slide-in-top 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
          ><span><a href={skill.link} class="skill">{skill.name}</a></span></Saos
        >
      {/each}
    </div>
  </div>
  <div class="skills-container">
    <h2>Languages</h2>
    <div class="skills">
      {#each languages as language}
        <Saos
          class="skill"
          animation={"slide-in-top 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
          ><span class="skill"><a href={language.link}>{language.name}</a></span></Saos
        >
      {/each}
    </div>
  </div>
  <img class="star2" src="/images/Stars.png" alt="" />
  <div class="skills-container">
    <h2>Tools & Frameworks</h2>
    <div class="skills">
      {#each toolsAndFrameworks as tool}
        <Saos
          class="skill"
          animation={"slide-in-top 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both"}
          ><span class="skill"><a href={tool.link}>{tool.name}</a></span></Saos
        >
      {/each}
    </div>
  </div>
</div>

<style>
  h2 {
    background: linear-gradient(90deg, #c0a2ff, #d355ff, #81f1c9);
    background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 2rem;
    font-weight: 700;
  }

  span {
    font-size: 1.2rem;
    background: transparent;
    padding: 0.5rem;
    color: white;
    position: relative;
    z-index: 9999;
    text-align: center;
    background: radial-gradient(
          circle at 100% 100%,
          #1b1c1f 0,
          #1b1c1f 25px,
          transparent 25px
        )
        0% 0%/30px 30px no-repeat,
      radial-gradient(
          circle at 0 100%,
          #1b1c1f 0,
          #1b1c1f 25px,
          transparent 25px
        )
        100% 0%/30px 30px no-repeat,
      radial-gradient(
          circle at 100% 0,
          #1b1c1f 0,
          #1b1c1f 25px,
          transparent 25px
        )
        0% 100%/30px 30px no-repeat,
      radial-gradient(circle at 0 0, #1b1c1f 0, #1b1c1f 25px, transparent 25px)
        100% 100%/30px 30px no-repeat,
      linear-gradient(#1b1c1f, #1b1c1f) 50% 50% / calc(100% - 10px)
        calc(100% - 60px) no-repeat,
      linear-gradient(#1b1c1f, #1b1c1f) 50% 50% / calc(100% - 60px)
        calc(100% - 10px) no-repeat,
      linear-gradient(#dba6f4 0%, rgba(142, 255, 214, 0.55) 57%, #00ffa3 100%);
    border-radius: 50em;
    padding: 0.7em;
  }

  .skills {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 2em;
    margin: auto;
  }

  #skills {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 2rem;
  }

  .skills-container {
    width: 60%;
    margin: auto;
    display: block;
  }

  img {
    width: 8em;
  }

  .star1 {
    position: absolute;
    align-self: flex-start;
    margin-left: 2em;
    margin-bottom: 35em;
  }

  .star2 {
   position: absolute;
    align-self: flex-end;
    margin-right: 6em;
    margin-top: 25em;
    background-color: transparent;

    /* write the css rules so that the content car go on top of the image*/
  }

  @keyframes -global-slide-in-top {
    0% {
      transform: translateY(-1000px);
      opacity: 0;
    }
    100% {
      transform: translateY(0);
      opacity: 1;
    }
  }

  a{
    text-decoration: none;
  }

  a:hover{
    text-decoration: underline;
    padding: 0.7em;
    background: none;
  }

    @media screen and (max-width: 768px) {
        .skills-container {
        width: 80%;
        }
        span{
            font-size: 1rem;
            padding: 0.9em;
        }
    }
</style>

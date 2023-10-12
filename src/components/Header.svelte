<header class="header">
    <nav class="wide-scrren-header">
        <li>
            <ul><a href="#about" class="about">About</a></ul>
            <ul><a href="#skills" class="skills">Skills</a></ul>
            <ul class="studies"><a href="#studies" class="studies">Studies</a></ul>
            <ul class="exp"><a href="#exp" class="exp">Experiences</a></ul>
            <ul class="contact"><a href="#contact" class="contact">Contact me</a></ul>
        </li>
    </nav>
    <nav class="small-screen-header">
        <li>
            <ul><a href="#about" class="about"><span class="material-symbols-outlined">
                person
                </span></a></ul>
            <ul><a href="#skills" class="skills"><span class="material-symbols-outlined">
                engineering
                </span></a></ul>
            <ul class="studies"><a href="#studies" class="studies"><span class="material-symbols-outlined">
                school
                </span></a></ul>
            <ul class="exp"><a href="#exp" class="exp"><span class="material-symbols-outlined">
                code
                </span></a></ul>
            <ul class="contact"><a href="#contact" class="contact"><span class="material-symbols-outlined">
                contact_page
                </span></a></ul>
        </li>
    </nav>
</header>

<style>
    .header{
        background-color: #1B1C1F;
        height: 3rem;
        display: block;
        transform: rotate(-2deg);
        width: 100vw;
        position: fixed;
        top: 0;
        margin-bottom: 3em;
        margin-top: 0.5em;
        z-index: 9999;
    }
    .small-screen-header{
        display: none;
    }
    li{
        list-style: none;
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 100%;
    }

    ul{
        font-size: 1.5em;
    }

    a{
        text-decoration: none;
    }

    a:hover{
        font-weight: bold;
        text-decoration: line-through;
    }

    .about, .about span{
        color: #EB34A0;
    }

    .skills, .skills span{
        color: #81F1C9;
    }

    .studies, .studies span{
        color: #DBA6F4;
    }

    .exp, .exp span{
        color: #ED7FC0;
    }

    .contact, .contact span{
        color: #07A3A3;
    }

    @media(max-width : 1300px){
        .header{
            height: 2rem;
        }
        li{
            font-size: 1em;
        }
    }

    @media(max-width : 800px){
        .wide-scrren-header{
            display: none;
        }
        .small-screen-header{
            display: block;
        }
        .header{
            bottom: 0;
        }

        span{
            font-size: 1.5em;
        }
        span:hover{
            font-size: 2em;
        }
    }
</style>
<script>
    import Header from '../components/Header.svelte';
    import Home from '../components/HomeView.svelte';
    import About from '../components/AboutView.svelte';
    import Skills from '../components/SkillsView.svelte';
    import Studies from '../components/StudiesView.svelte';
    import Experiences from '../components/ExperiencesView.svelte';
    import Contact from '../components/ContactView.svelte';
</script>


<Header />
<Home />
<About />
<Skills />
<Studies />
<Experiences />
<Contact />

<style>
    :global(*) {
        background-color: #1B1C1F;
        color: white;
        font-family: 'Space Mono', monospace;
    }
</style>

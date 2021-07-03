<script lang="ts">
	import Profile from './components/profile.svelte'
	import Header from './components/header.svelte'
	import Tabbed from './components/tabbed.svelte'
	import Article from './components/article.svelte'
	import Project from './components/project.svelte'
	import Contact from './components/contact.svelte'

	let items = [
	{ 
		label: "Projects",
		value: 1,
		component: Project
	},
    { 
		label: "Articles",
		value: 2,
		component: Article
	},
    { 
		label: "Contact",
		value: 3,
		component: Contact
	}
  ];
</script>
<header>
	<Header />
</header>
<main>
	<aside>
		<Profile />
	</aside>
	<section>
		<Tabbed {items} />
	</section>
</main>
<style>
main {
	display: grid;
	grid-template-columns: 1fr;
	grid-gap: 1rem;
}
@media (min-width:768px) {
	main {
		grid-template-columns: 1fr 3fr;
		grid-gap: 3rem;
		padding: 1rem 0;
	}
}
</style>
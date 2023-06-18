<nav>
	<div class="nav-container">
		<a href="/" class="nav-logo">Uncnown</a>
		<div class="nav-links">
			{#each nav as link}
				<a href={link.href} class="link">{link.title}</a>
			{/each}
		</div>
	</div>
</nav>
<div class="container">
	<!--Pages will be injected below-->
	<slot></slot>
</div>

<script>
	const nav = [
		{ 
			title: 'About me',
			href: '/about'
		},
		{
			title: 'Blog',
			href: '/blog'
		},
		{
			title: 'Project',
			href: '/projects'
		},
		{
			title: 'Contact',
			href: '/contact'
		},
		{
			title: 'Settings',
			href: '/temp'
		}
	]
</script>

<style>
	.container {
		max-width: 1400px;
		margin: 50px auto;
	}
</style>
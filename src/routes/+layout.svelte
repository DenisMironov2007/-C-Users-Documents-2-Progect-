<nav>
	<div class="nav-container">
		<a href="/" class="nav-logo">Uncnown</a>
		<div class="nav-links">
			{#each nav as link}
			{#if link.isShow}
				<a href={link.href} class="link">{link.title}</a>
			{/if}
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
			href: '/about',
			isShow: true
		},
		{
			title: 'Blog',
			href: '/blog',
			isShow: true
		},
		{
			title: 'Project',
			href: '/projects',
			isShow: true
		},
		{
			title: 'Contact',
			href: '/contact',
			isShow: true
		},
		{
			title: 'Settings',
			href: '/temp',
			isShow: true
		},
		{
			title: 'Problems_500',
			href: '/ohibka',
			isShow: false
		}
	]
</script>

<style>
	.container {
		max-width: 1400px;
		margin: 50px auto;
	}
</style>
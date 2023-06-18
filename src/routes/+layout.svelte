<nav>
	<div class="nav-container">
		<a href="/" class="nav-logo">Uncnown</a>
		<div class="nav-links">
			<a href="/about" class="link">About Me</a>
			<a href="/blog" class="link">Blog</a>
			<a href="/projects" class="link">Project</a>
			<a href="/contact" class="link">Contacts</a>
		</div>
	</div>
</nav>
<div class="container">
	<!--Pages will be injected below-->
	<slot></slot>
</div>

<style>
	.container {
		max-width: 1400px;
		margin: 50px auto;
	}
</style>
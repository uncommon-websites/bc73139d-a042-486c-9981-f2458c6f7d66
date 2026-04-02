<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="page">
	<h1>Error {page.status}</h1>
	<p>{page.error?.message ?? "Something went wrong. Your digital mind is still intact."}</p>
	<a href="/">Go back home</a>
</main>

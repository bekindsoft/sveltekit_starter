<script>
	import { enhance } from "$app/forms";

	export let data
</script>

<h1 class="font-bold text-2xl">Hi, {data.user.username}!</h1>
<p>Your user ID is {data.user.id}.</p>
<form method="post" use:enhance>
<button class="btn btn-primary">Sign out</button>
</form>

<script>
	import { enhance } from '$app/forms';
	export let form;
</script>

<div class="hero min-h-screen bg-base-200">
	<div class="hero-content text-center">
		<div class="max-w-md">
			<h1 class="text-3xl font-bold">Sign in</h1>
			<form method="post" class="form space-y-2" use:enhance>
				<label class="form-control w-full max-w-xs" for="username">
					<div class="label">
						<span class="label-text">Username</span>
					</div>
					<input
						name="username"
						id="username"
						type="text"
						placeholder="username"
						class="input input-bordered w-full max-w-xs"
					/>
				</label>

				<label class="form-control w-full max-w-xs" for="password">
					<div class="label">
						<span class="label-text">Password</span>
					</div>
					<input
						type="password"
						name="password"
						id="password"
						placeholder="password"
						class="input input-bordered w-full max-w-xs"
					/>
				</label>

				<button class="btn w-full btn-primary">Continue</button>
				<p>{form?.message ?? ''}</p>
			</form>
			<a href="/signup">Create an account</a>
		</div>
	</div>
</div>

<script>
import LoginSlider from "../../Components/LoginSlider"


export default {
	components: {
		LoginSlider,
	},
	
};

</script>

<template>
	<div class="grid grid-cols-12">
		<div class="col-span-6 slider-bg">
			<div class="col-start-2 col-span-4">
				<LoginSlider />
			</div>
		</div>

		<div class="login-form col-span-6">
			<div class="login-bg ">
				<div class="xl:container mx-auto grid grid-cols-6">

					<div class="col-start-2 col-span-4">
						<div class="w-full max-w-md space-y-8 login-wrap bg-white">
							<div class=" flex flex-col justify-between h-full min-h-screen py-12">
								<NuxtLink to="/" class="site-logo">
									<img class="max-w-[160px] w-full" src="../../assets/img/login-2-logo.svg"
										alt="Company logo" />
								</NuxtLink>

								<div class="">
									<h2 class="mt-6 text-4xl font-bold tracking-tight text-dark1">Sign in</h2>
									<form class="mt-8 space-y-6" action="#" method="POST">
										<input type="hidden" name="remember" value="true" />
										<div class="-space-y-px rounded-md gap-6 grid">
											<div>
												<label for="email-address"
													class="text-base font-medium text-dark1 pb-2.5 inline-block">Email</label>
												<input id="email-address" name="email" type="email" autocomplete="email"
													required=""
													class="relative block w-full appearance-none rounded-lg border-2 border-dark5 px-3 py-2 text-dark1 placeholder-dark4 focus:z-10 focus:border-indigo-500 focus:outline-none focus:ring-indigo-500 font-medium" placeholder="Email address" />
											</div>
											<div>
												<label for="password"
													class="text-base font-medium text-dark1 pb-2.5 inline-block">Password</label>
												<input id="password" name="password" type="password"
													autocomplete="current-password" required=""
													class="relative block w-full appearance-none rounded-lg border-2 border-dark5 px-3 py-2 text-dark1 placeholder-dark4 focus:z-10 focus:border-indigo-500 focus:outline-none focus:ring-indigo-500 font-medium" placeholder="Password" />
											</div>
										</div>

										<div class="flex items-center justify-between">
											<div class="flex items-center">
												<input id="remember-me" name="remember-me" type="checkbox" class="h-4 w-4 rounded border-gray-300 text-indigo-600 focus:ring-indigo-500" />
												<label for="remember-me" class="ml-2 block text-sm text-dark2 font-normal">Remember me</label>
											</div>

											<div class="">
												<NuxtLink class="text-sm text-main_purple font-medium"
													to="/forgot-password2">Forgot password?</NuxtLink>
											</div>
										</div>

										<NuxtLink to="/login">
											<button type="submit"
												class="group relative flex w-full justify-center rounded-md bg-main_purple text-lg py-2 px-4 font-semibold text-white hover:bg-indigo-700 focus:outline-none mt-7">
												Sign in
											</button>
										</NuxtLink>
									</form>
								</div>

								<p class="mt-12 font-medium text-dark2">
									Don't have an account yet ? <NuxtLink class="text-main_purple" to="/registration">Create an account</NuxtLink>
								</p>
							</div>
						</div>
					</div>

				</div>
			</div>
		</div>
	</div>
</template>

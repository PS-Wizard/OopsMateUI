<script>
    import Fade from "$lib/components/Fade.svelte";

    let email = $state("");
    let password = $state("");
</script>

<Fade>
    <div class="flex min-h-screen">
        <!-- Left side -->
        <div
            class="w-1/2 flex flex-col justify-between p-8 text-white bg-cover bg-center"
            style="background-image: url('https://i.pinimg.com/1200x/83/e1/e5/83e1e5fb29f27513bfe1507d193919b1.jpg');"
        >
            <div class="text-2xl clash">Oops! Mate</div>
            <div class="mt-auto text-sm opacity-80">
                This is totally the strongest bot you will ever play against…
                totally <br />
                Source: Trust Me Bro.
            </div>
        </div>

        <!-- Right side -->
        <div
            class="w-1/2 flex items-center justify-center bg-neutral-100 archivo text-black"
        >
            <form class="w-3/4 max-w-sm space-y-4">
                <h2 class="text-4xl text-center">Log In To Your Account</h2>
                <p class="text-center text-gray-400 text-sm">
                    Enter your email & password below to log in to your account
                </p>

                <input
                    type="email"
                    placeholder="name@example.com"
                    bind:value={email}
                    class="w-full px-4 py-2 rounded-md bg-neutral-200 border border-neutral-300 focus:outline-none focus:ring-2 focus:ring-indigo-500"
                />

                <input
                    type="password"
                    placeholder="superdupersecret123"
                    bind:value={password}
                    class="w-full px-4 py-2 rounded-md bg-neutral-200 border border-neutral-300 focus:outline-none focus:ring-2 focus:ring-indigo-500"
                />

                <button
                    type="submit"
                    class="w-full bg-neutral-900 text-white py-2 rounded-md hover:bg-neutral-800 transition-all cursor-pointer"
                >
                    Log In with Email
                </button>

                <div
                    class="flex items-center justify-center text-gray-400 text-sm"
                >
                    <span class="mx-2">Don't Have An Account?</span>
                </div>

                <a
                    href="/signup"
                    type="button"
                    class="underline text-center block"
                >
                    Sign Up
                </a>
            </form>
        </div>
    </div>
</Fade>

<script>
    import Fade from "$lib/components/Fade.svelte";

    let email = $state("");
    let password = $state("");
</script>

<Fade>
    <div class="flex min-h-screen">
        <!-- Left side -->

        <!-- Right side -->
        <div
            class="w-1/2 flex items-center justify-center bg-neutral-100 archivo text-black"
        >
            <form class="w-3/4 max-w-sm space-y-4">
                <h2 class="text-4xl text-center">Create an account</h2>
                <p class="text-center text-gray-400 text-sm">
                    Enter your email & password below to create your account
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
                    Sign In with Email
                </button>

                <div class="flex items-center justify-center text-gray-400 text-sm">
                    <span class="mx-2">Already Have An Account?</span>
                </div>

                <a href="/login" type="button" class="underline text-center block">
                    Log In
                </a>
            </form>
        </div>
        <div class="w-1/2 flex flex-col justify-between p-8 text-white bg-cover bg-center" 
             style="background-image: url('https://i.pinimg.com/736x/40/08/bc/4008bcb0e26a3e955f09418cf1683758.jpg');">
            <div class="text-2xl clash">Oops! Mate</div>
            <div class="mt-auto text-sm opacity-80">
                This is totally the strongest bot you will ever play against… totally <br />
                Source: Trust Me Bro.
            </div>
        </div>
    </div>
</Fade>

<script>
    import Fade from "$lib/components/Fade.svelte";
    import Navbar from "$lib/components/Navbar.svelte";
</script>

<Navbar />
<Fade>
    <div class="flex justify-between p-16">
        <div class="flex flex-col gap-8 w-2/3">
            <h1 class="text-[4xl~8xl] clash leading-[1]">
                An engine so strong, <br /> it regins for you. <br />
            </h1>
            <p class="max-w-3xl archivo tracking-wide text-neutral-600">
                This is an ongoing Final Year Project — a chess engine website
                still in progress. You can login or signup; except that you
                can't because it doesnt do anything yet ╚(″⚈ᴗ⚈)╗ .
            </p>

            <div class="flex gap-2">
                <a
                    href="/login"
                    class="archivo uppercase text-sm bg-neutral-900 text-white px-5 py-2 rounded-lg font-medium hover:bg-neutral-800 transition"
                >
                    GitHub &nearr;
                </a>
                <a
                    href="/signup"
                    class="archivo uppercase text-sm bg-neutral-100 text-neutral-900 px-5 py-2 rounded-lg font-medium border border-neutral-300 hover:bg-neutral-200 transition"
                >
                    Linkedin &nearr;
                </a>
            </div>
        </div>
        <div class="w-1/3 flex justify-center">
            <img src="/logo.png" alt="logo" class="object-contain" />
        </div>
    </div>
</Fade>

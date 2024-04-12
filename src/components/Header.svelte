<script>
    import { base } from '$app/paths';
    let tabs = [
        {name: 'Projects', href: 'projects'},
        {name: 'About Me', href: 'about'}
    ]
</script>

<header class="sticky z-[10] duration-200 top-0 px-6 flex justify-between bg-slate-950/75">
    <h1 class="m-4 p-2 font-medium">
        <b>Ashay</b> Srivastava
    </h1>
    <div class="m-4">
        {#each tabs as tab,index}
            <a class="duration-400 hover:text-violet-400 m-2" href={`${base}/${tab.href}`}>{tab.name}</a>
        {/each}
        <button class="p-2 px-3 bg-white text-slate-950 rounded-full hover:bg-slate-200">Let's Connect</button>
    </div>
</header>


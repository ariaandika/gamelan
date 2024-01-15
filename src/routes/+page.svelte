<script>

import { RefreshCw, Gauge, Home, SeparatorHorizontal, ArrowLeftCircle, ArrowRightCircle } from "lucide-svelte";
import * as Separator from "$lib/components/ui/separator"
import { Button } from "$lib/components/ui/button"

const sizeBtn = 87
const sizeMed = 50



</script>

<section class="flex h-screen">

    <aside class="p-2 woot">
        <Home size={sizeMed}/>
        <div class="border-t-black border-t-4">
            <Home class="homee" size={66 / 113}/>
        </div>
    </aside>


    <section class="w-full h-screen flex flex-col bg-red-600">
        <aside class="bg-blue-800 text-white p-4 flex gap-4">
            <RefreshCw/>
            <Gauge/>
        </aside>

        <section class="grid grid-cols-2 my-auto border-b-black flex-grow">
            <section class="bg-neutral-200 h-full flex flex-col p-4 gap-4 overflow-x-hidden overflow-y-scroll">
                {#each Array(2) as _}
                <div class="bg-neutral-400 p-8 rounded-sm">Woo</div>
                {/each}
                <div class="bg-blue-400">a</div>
            </section>

            <section class="bg-white p-8">
                <div class="bg-neutral-400 rounded-lg h-full p-4 flex flex-col">
                    <div class="bg-white rounded-lg flex-grow">{"a"}</div>
                    <div class="p-2 flex justify-between">
                        <ArrowLeftCircle size={sizeBtn}/>
                        <ArrowRightCircle size={sizeBtn}/>
                    </div>
                </div>
            </section>

        </section>
    </section>


</section>

<style>
    .woot {
          width: calc((113 / 1440) * 100vw);
    }
    /* :global(.homee) { */
    /*     width: calc((66 / 113) * 100vw); */
    /*     height: calc((66 / 960) * 100vh); */
    /* } */
</style>



<script lang="ts">
  import { ScrollArea } from "$lib/components/ui/scroll-area/index.js";
  import { Maximize2, Minus, X } from "lucide-svelte";
  import Coding from "../coding/Coding.svelte";
  import FunFacts from "../funFacts/FunFacts.svelte";
  import Hobbies from "../hobbies/Hobbies.svelte";

  let intro = `Hi! I'm Jéssica ^_^

I’m just a girl from moz running on coffee and trying to make sense of
life one Google search at a time (send help T_T)

Make yourself at home! Just don't come in with dirty shoes...`;
</script>

<main class="min-h-screen flex flex-col items-center justify-center">
  <div class="grid grid-cols-5">
    <h1 class="col-start-3 text-center">Jéssica 101</h1>
  </div>

  <div class="bg-white shadow-md rounded-lg p-3 m-4 w-7xl grid grid-cols-4">
    <div class="col-span-1 bg-purple-100">
      <h2 class="text-center">Welcome</h2>
      <img
        src="https://media.giphy.com/media/v1.Y2lkPWVjZjA1ZTQ3bnpxYW1wNGc0b25sd3Zsem9iYzMzeXU1MjRndjM1MzJsYm84emJxcyZlcD12MV9naWZzX3JlbGF0ZWQmY3Q9Zw/dn12b0TGWufPpdoSTv/giphy.gif"
        alt="flower"
        height="500px"
        width="400px"
      />
    </div>

    <div
      class="pixel-scrollbar col-span-2 border-2 border-purple-800 overflow-y-auto h-[500px]"
    >
      <div class=" bg-purple-300 flex"><X /> <Minus /><Maximize2 /></div>
      <p class="text-center p-4 whitespace-pre-line pb-10">{intro}</p>
      <Coding />
      <Hobbies />
    </div>

    <div class="col-span-1 bg-purple-100"><FunFacts /></div>
  </div>
</main>

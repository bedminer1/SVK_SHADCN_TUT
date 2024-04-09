<script lang="ts">
  import Sun from "svelte-radix/Sun.svelte";
  import Moon from "svelte-radix/Moon.svelte";
  import { toggleMode } from "mode-watcher";
  import { Button } from "$lib/components/ui/button/index.js";
</script>

<nav class="flex justify-end w-full p-2">
  <Button on:click={toggleMode} variant="outline" size="icon" class="active:scale-90">
      <Moon
        class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100"
      />
      <Sun
        class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0"
      />
      <span class="sr-only">Toggle theme</span>
    </Button>
</nav>
<div class="flex items-center justify-center w-full h-screen">
  <div>
    <a href="/library">The Library</a>
  </div>
</div>
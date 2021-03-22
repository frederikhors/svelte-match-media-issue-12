<script lang="ts">
  import { createMedia } from "svelte-match-media";

  export let name: string;

  const breakpoints = {
    sm: "screen and (max-width: 767px)",
    lg: "screen and (min-width: 1024px)",
  };

  const { media } = createMedia(breakpoints);

  console.log("media:", media);
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
</main>

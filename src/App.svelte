<script>
  import { Button } from "sveltestrap";
  import Toggler from "./Mode.svelte";
</script>

<main class="body">
  <div class="text-center container">
    <h1 class="title">GoFed</h1>
    <br />
    <h3>A game, made using deno_sdl2!</h3>
    <h4>
      Gofed, meaning Go Feed is a 2D platformer game made using deno and SDL2.
      <br />It has a lot of levels and each level you pass, the harder it gets.
    </h4>

    <Toggler>
      <Button
        color="primary"
        class="btnc"
        href="https://github.com/dhairy-online/platformer-deno"
        >Check it out here</Button
      >
      Toggleasd
    </Toggler>
  </div>
</main>

<style>
  :global(body) {
    background-color: #f2eee2;
    color: #0084f6;
    transition: background-color 0.3s;
  }
  :global(body.dark-mode) div {
    color: white;
  }
  :global(body.dark-mode) {
    background-color: #071013;
    color: #bfc2c7;
  }
  @import url("https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@700&display=swap");
  :global(body) {
    background-color: #f2eee2;
  }
  .title {
    font-size: 90px;
    font-family: "JetBrains Mono", monospace;
    color: #a2aebb;
  }
  div {
    font-family: "JetBrains Mono", monospace;
    color: #dfe0e2;
  }
  .btnc {
    color: #071013;
    background-color: #a2aebb;
  }
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

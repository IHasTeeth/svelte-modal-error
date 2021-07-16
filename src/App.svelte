<script>
  import Tailwind from "./components/Tailwind.svelte";
  import Modal from "svelte-simple-modal";
  import Button from "./Button.svelte";

  export let name;
</script>

<Tailwind />

<Modal>
  <main class="text-center p-4 max-w-xs mx-auto sm:max-w-none">
    <h1 class="text-red-500 text-6xl uppercase leading-loose font-thin">
      Hello {name}!
    </h1>
    <p class="text-gray-700">
      Visit the <a
        class="text-blue-600 hover:underline"
        href="https://svelte.dev/tutorial">Svelte tutorial</a
      > to learn how to build Svelte apps.
    </p>
    <Button />
  </main>
</Modal>

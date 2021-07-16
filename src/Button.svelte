<script>
  import { getContext } from "svelte";
  import TestModal from "./modals/testModal.svelte";
  const { open } = getContext("simple-modal");
  const showSurprise = () => {
    open(TestModal);
  };
</script>

<button
  on:click={showSurprise}
  class="modal-open bg-transparent border border-gray-500 hover:border-indigo-500 text-gray-500 hover:text-indigo-500 font-bold py-2 px-4 rounded-full"
  >Open Modal</button
>

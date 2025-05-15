<script lang="ts">
  import { IconBrandAmazon } from "@tabler/icons-svelte";
  export let livro: any = null;
</script>

{#if livro}
  <a
    href={livro.link}
    target="_blank"
    class="flex flex-col text-center justify-between rounded-md bg-zinc-900 overflow-hidden"
  >
    <img src={livro.imagem} alt="Imagem do Livro" class="rounded-md" />
    <div class="flex flex-1 flex-col">
      <span class="flex-1 text-[10px] text-center sm:text-[20px] sm:font-bold"
        >{livro.titulo}</span
      ><br />
      <button
        class="flex flex-col items-center button-perso text-[12px] sm:text-[16px] sm:w-36"
      >
        <IconBrandAmazon />
        <span>Book Link</span></button
      >
    </div>
  </a>
{/if}

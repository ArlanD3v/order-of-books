<script lang="ts">
  export let serie: any = null;
</script>

{#if serie}
  <div
    class="flex flex-col rounded-md overflow-hidden border border-zinc-800
   "
  >
    <a
      class="text-center bg-white/10 hover:bg-[#89f2ff] hover:text-black hover:font-bold duration-1000"
      href="/series/{serie.id}"
    >
      {serie.titulo}
      <img
        src={serie.imagem}
        alt="Imagem da Serie"
        class="h-full object-cover brightness-60 hover:brightness-105 duration-1000"
      />
    </a>

    <div class="flex flex-col gap-2 p-5">
      <span class="text-2xl font-black text-center">{serie.titulo}</span>
      <span class="text-sm text-zinc-400 text-justify">{serie.descricao}</span>

      <a href="/series/{serie.id}" class="button-perso w-32">
        <button class="cursor-pointer rounded-md">Read more</button>
      </a>
    </div>
  </div>
{/if}

<script lang="ts">
  export let autor: any = null;
</script>

{#if autor}
  <a
    href="/autores/{autor.id}"
    class="flex flex-col rounded-md relative overflow-hidden
	 
	 "
  >
    <img src={autor.imagem} alt="Foto do Autor" class="h-96 object-cover" />

    <div
      class="absolute w-full flex
		bottom-0 px-6 py-4
		bg-black/50 hover:bg-[#33CCCC]/70
		hover:font-semibold hover:text-black
		transform translate-x-0 hover:translate-x-1/2
		transition-transform duration-1500"
    >
      <span class="text-2xl">{autor.nome}</span>
    </div>
  </a>
{/if}

<script>
  import ItemAutor from "../../components/autor/ItemAutor.svelte";
  import Titulo from "../../components/shared/Titulo.svelte";
  import autores from "../../constants/autores";
</script>

<div class="flex flex-col gap-10">
  <div class="hover:text-[#33CCCC] duration-1000">
    <Titulo
      principal="Authores"
      secundario="Get to know the faces, smiles and looks of those who make you happy through reading"
    />
  </div>
  <div class="grid grid-cols-2 gap-5">
    {#each autores as autor}
      <div class="grayscale hover:grayscale-0 transition duration-1500">
        <ItemAutor {autor} />
      </div>
    {/each}
  </div>
</div>

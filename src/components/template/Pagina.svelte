<script>
  import AreaLateral from "./AreaLateral.svelte";
  import Cabecalho from "./Cabecalho.svelte";
  import Rodape from "./Rodape.svelte";
</script>

<div
  class="flex flex-col min-h-screen
	bg-black text-white
	"
>
  <Cabecalho />
  <div class="flex flex-1 gap-5 max-w-7xl mx-auto w-full p-5">
    <main class="flex-1 max-h-[120vh] overflow-hidden hover:overflow-y-auto">
      <slot></slot>
    </main>
    <AreaLateral />
  </div>

  <Rodape />
</div>

<!--#33CCCC azul da pena -->

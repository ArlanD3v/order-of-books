<script>
  import { page } from "$app/state";
  import ConteudoAutor from "../../../components/autor/ConteudoAutor.svelte";
</script>

<ConteudoAutor autor={page.data.autor} />

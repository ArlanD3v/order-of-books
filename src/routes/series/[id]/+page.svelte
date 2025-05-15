<script>
  import { page } from "$app/state";
  import ConteudoSerie from "../../../components/serie/ConteudoSerie.svelte";
</script>

<ConteudoSerie serie={page.data.serie} />

<script>
  import {
    IconBook,
    IconBrandFacebook,
    IconBrandInstagram,
    IconBrandLinkedin,
    IconBrandYoutube,
    IconFriends,
    IconHome,
    IconSquare1,
    IconSquare2,
    IconSquare3,
    IconSquare4,
    IconSquare5,
    IconStar,
    IconUser,
  } from "@tabler/icons-svelte";
  import Menu from "./Menu.svelte";
  import MenuItem from "./MenuItem.svelte";
</script>

<aside
  class="flex flex-col self-start

 text-center
 sm:text-left
 rounded-md border border-zinc-800
 p-2 sm:p-4
 gap-10
 w-22
 sm:w-55"
>
  <Menu titulo="Navigation">
    <MenuItem texto="Start" href="/">
      <IconHome size={20} />
    </MenuItem>
    <MenuItem texto="Characters" href="/">
      <IconFriends size={20} />
    </MenuItem>
    <MenuItem texto="Authores" href="/autores">
      <IconUser size={20} />
    </MenuItem>
    <MenuItem texto="Series" href="/">
      <IconBook size={20} />
    </MenuItem>
  </Menu>
  <Menu titulo="Main Authors">
    <MenuItem texto="Arlan S.L" href="/autores/arlan-s-lima">
      <IconSquare1 size={20} />
    </MenuItem>
    <MenuItem
      texto="Marcele V.Q. Oliveira"
      href="/autores/marcele-v-q-oliveira"
    >
      <IconSquare2 size={20} />
    </MenuItem>
    <MenuItem texto="J.K. Rowling" href="/autores/j-k-rowling">
      <IconSquare3 size={20} />
    </MenuItem>
    <MenuItem texto="J.R.R Tolkien" href="/autores/j-r-r-tolkien">
      <IconSquare4 size={20} />
    </MenuItem>
    <MenuItem texto="George R.R Martin" href="/autores/george-r-r-martin">
      <IconSquare5 size={20} />
    </MenuItem>
  </Menu>
  <Menu titulo="Other categories">
    <MenuItem texto="Popular Series">
      <IconStar size={20} />
    </MenuItem>
  </Menu>
  <Menu titulo="Website creator's social networks">
    <MenuItem
      texto="Instagram"
      href="https://www.instagram.com/arl.an/"
      target="_blank"
    >
      <IconBrandInstagram size={20} />
    </MenuItem>
    <MenuItem
      texto="Facebook"
      href="https://www.facebook.com/arlansl/?locale=pt_BR"
      target="_blank"
    >
      <IconBrandFacebook size={20} />
    </MenuItem>
    <MenuItem
      texto="Linkeedin"
      href="https://www.linkedin.com/in/arlandev/"
      target="_blank"
    >
      <IconBrandLinkedin size={20} />
    </MenuItem>
    <MenuItem
      texto="Youtube"
      href="https://www.youtube.com/@Arlan_Suuang"
      target="_blank"
    >
      <IconBrandYoutube size={20} />
    </MenuItem>
  </Menu>
</aside>

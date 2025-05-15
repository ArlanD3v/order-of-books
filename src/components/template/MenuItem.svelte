<script>
  export let href = "/";
  export let texto = "";
  export let target = "";
</script>

<li>
  <a
    {href}
    {target}
    class="
	relative inline-block
	cursor-pointer
	px-4
	py-2
	text-zinc-300
	hover: hover:text-white hover:bg-white/10
	after:block after:h-[2px] after:w-full after:bg-[#33CCCC] after:scale-x-0
	after:origin-left after:transition-transform
	after:duration-500 hover:after:scale-x-100
	"
  >
    <div class="flex items-center gap-2">
      <slot></slot>
      <span>{texto}</span>
    </div>
  </a>
</li>

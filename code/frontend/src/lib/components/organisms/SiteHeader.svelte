<script lang="ts">
  //import all the data from navLinks data in data.ts
  import { navLinks } from '$lib/data';
  import ButtonComponent from "../atoms/ButtonComponent.svelte";
	import NavLink from "../atoms/NavLink.svelte";
</script>


<ButtonComponent backgroundColor="bg-red-50" label="book"  />

<nav>
  {#each navLinks as link (link.href)}
    <NavLink href={link.href} label={link.label} />
  {/each}
</nav>

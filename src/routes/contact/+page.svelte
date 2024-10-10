<script lang="ts">
	import { Fa } from "svelte-fa";
	import {  faGithub, faFacebook, faInstagram } from "@fortawesome/free-brands-svg-icons";
    import { faEnvelope } from "@fortawesome/free-solid-svg-icons"

	const socials = [
		{ site: "https://github.com/Pauline0306", text: "GitHub", icon: faGithub },
		{ site: "https://www.facebook.com/pauline.astorga", text: "Facebook", icon: faFacebook },
		{ site: "https://www.instagram.com/paawwiii_", text: "Instagram", icon: faInstagram },
	];
</script>

<h1 class="text-4xl">Contact</h1>
<p>Follow me on my socials and get to know me more.</p>
<div class="w-full max-w-sm grid grid-cols-2 md:grid-cols-3 gap-4">
    {#each socials as link}
        <a href={link.site} target="_blank" class="text-lg text-white"><Fa icon={link.icon} class="mr-2 inline" size="lg" />{link.text}</a>
    {/each}
</div>
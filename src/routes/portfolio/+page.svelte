<script lang="ts">
	const colImages1 = [
	
		{
			alt: "Bowling",
			src: "Images/bowling.jpg",
			description: "Bowling Silver Awardee",
		},
		{
			alt: "Vroom",
			src: "Images/Vroom 1.jpg",
			description: "Vroom Reservation System",
		},
		
	];

	const colImages2 = [
		{
			alt: "blog",
			src: "Images/blogproject.jpg",
			description: "Blogging System homepage",
		},
		{
			alt: "blog-1",
			src: "Images/blogproject1",
			description: "Blogging System login",
		},
	

	];


</script>

<h1 class="text-6xl">Portfolio</h1>
<p>Here are my projects and activities.</p>


<div class="w-full">
    <div class="grid gap-4 grid-cols-1 sm:grid-cols-2 lg:grid-cols-4">
        <div class="flex flex-col gap-4">
            {#each colImages1 as colImage}
           <div class="w-full h-fit overflow-hidden rounded-lg">
                <img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
                <p class="text-center text-white mt-2">{colImage.description}</p>
            </div>
            {/each}
        </div>
        <div class="flex flex-col gap-4">
            {#each colImages2 as colImage}
            <div class="w-full h-fit overflow-hidden rounded-lg">
                <img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
                <p class="text-center text-white mt-2">{colImage.description}</p>
            </div>
            {/each}
        </div>
    </div>
</div>
<script lang="ts">
	const books = [
		{ title: 'The Whisper of Shadows', author: 'Eliza Blackwood' },
		{ title: 'Quantum Echoes', author: 'Dr. Aiden Frost' },
		{ title: 'The Last Serenade', author: 'Sophia Nightingale' },
		{ title: 'Neon Dreams in Tokyo', author: 'Hiro Tanaka' },
		{ title: 'The Alchemy of Starlight', author: 'Luna Silverstone' },
		{ title: 'Echoes from the Void', author: 'Commander Jack Nova' },
		{ title: 'Whispers of the Ancient Forest', author: 'Aria Greenleaf' },
		{ title: 'The Clockwork Conspiracy', author: 'Professor Thaddeus Gearhart' },
		{ title: 'Sands of Time: A Desert Odyssey', author: 'Zara Dune' },
		{ title: 'The Quantum Tailor', author: 'Dr. Evelyn Threadcraft' },
		{ title: 'Melodies of the Heart', author: 'Maestro Giovanni Allegro' },
		{ title: 'The Cybernetic Sonata', author: 'Ada Lovelace II' },
		{ title: 'Secrets of the Celestial Sea', author: 'Captain Orion Stardust' },
		{ title: 'The Whimsical Watchmaker', author: 'Horatio Ticktock' }
	];
</script>

<ul>
	{#each books as book}
		<li>
			<span class="title">{book.title}</span>
			<span class="author">by {book.author}</span>
		</li>
	{/each}
</ul>

<style>
	ul {
		display: flex;
		flex-direction: column;
		gap: 1rem;

		width: fit-content;
		max-height: 300px;
		margin: 0;
		padding: 1rem;
		border: 2px solid black;
		border-radius: 24px;

		overflow-y: auto;
		scrollbar-color: black lightgray;
	}

	li {
		display: flex;
		flex-direction: column;
	}

	.title {
		font-weight: bold;
	}

	.author {
		font-style: italic;
	}
</style>

<script lang="ts">
	import quizzes from "../data.json";
	import Card from "../components/Card.svelte";
</script>

<div class="quizzes-container w-[700px] m-auto flex justify-center h-screen items-center">
	{#each quizzes as quiz (quiz.id)}
		<Card {quiz} />
	{/each}
</div>

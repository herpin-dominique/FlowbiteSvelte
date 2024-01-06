<script>
	import {
		Section,
		ArticleAuthor,
		ArticleBody,
		ArticleHead,
		ArticleWrapper,
		BlogHead,
		BlogBodyWrapper
	} from 'flowbite-svelte-blocks';
	import { VideoSolid, ArrowRightOutline, NewspaperSolid } from 'flowbite-svelte-icons';
	import { Datepicker } from 'flowbite-svelte';
</script>

<h1>choix-sejour</h1>
<Section name="blog">
	<BlogHead>
		<svelte:fragment slot="h2">Our Blog</svelte:fragment>
		<svelte:fragment slot="paragraph">
			<p class="font-light text-gray-500 dark:text-gray-400 sm:text-xl">
				We use an agile approach to test assumptions and connect with the needs of your audience
				early and often.
			</p>
		</svelte:fragment>
		<Datepicker range />
	</BlogHead>
	<BlogBodyWrapper>
		<ArticleWrapper>
			<ArticleHead>
				<span
					class="bg-primary-100 text-primary-800 dark:bg-primary-200 dark:text-primary-800 inline-flex items-center rounded px-2.5 py-0.5 text-xs font-medium"
				>
					<VideoSolid size="xs" class="mr-1" />
					Tutorial
				</span>
				<span class="text-sm">14 days ago</span>
			</ArticleHead>
			<ArticleBody>
				<svelte:fragment slot="h2"><a href="/">retour aux choix</a></svelte:fragment>
				<svelte:fragment slot="paragraph">
					<p class="mb-5 font-light text-gray-500 dark:text-gray-400">
						Static websites are now used to bootstrap lots of websites and are becoming the basis
						for a variety of tools that even influence both web designers and developers influence
						both web designers and developers.
					</p>
				</svelte:fragment>
			</ArticleBody>
			<ArticleAuthor>
				<svelte:fragment slot="author">
					<img
						class="h-7 w-7 rounded-full"
						src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/jese-leos.png"
						alt="Jese Leos avatar"
					/>
					<span class="font-medium dark:text-white"> Jese Leos </span>
				</svelte:fragment>
				<a
					href="/"
					class="text-primary-600 dark:text-primary-500 inline-flex items-center font-medium hover:underline"
				>
					Read more
					<ArrowRightOutline size="sm" class="ml-2" />
				</a>
			</ArticleAuthor>
		</ArticleWrapper>

		<ArticleWrapper>
			<ArticleHead>
				<span
					class="bg-primary-100 text-primary-800 dark:bg-primary-200 dark:text-primary-800 inline-flex items-center rounded px-2.5 py-0.5 text-xs font-medium"
				>
					<NewspaperSolid size="xs" class="mr-1" />
					Article
				</span>
				<span class="text-sm">14 days ago</span>
			</ArticleHead>
			<ArticleBody>
				<svelte:fragment slot="h2"><a href="/">retour aux choix</a></svelte:fragment>
				<svelte:fragment slot="paragraph">
					<p class="mb-5 font-light text-gray-500 dark:text-gray-400">
						Static websites are now used to bootstrap lots of websites and are becoming the basis
						for a variety of tools that even influence both web designers and developers influence
						both web designers and developers.
					</p>
				</svelte:fragment>
			</ArticleBody>
			<ArticleAuthor>
				<svelte:fragment slot="author">
					<img
						class="h-7 w-7 rounded-full"
						src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/bonnie-green.png"
						alt="Bonnie Green avatar"
					/>
					<span class="font-medium dark:text-white"> Dominique </span>
				</svelte:fragment>
				<a
					href="/"
					class="text-primary-600 dark:text-primary-500 inline-flex items-center font-medium hover:underline"
				>
					En savoir plus
					<ArrowRightOutline size="sm" class="ml-2" />
				</a>
			</ArticleAuthor>
		</ArticleWrapper>
	</BlogBodyWrapper>
</Section>

<script lang="ts">
	import { mdiGithub, mdiOpenInNew, mdiLinkedin, mdiFileDocument } from "@mdi/js"
	import Icon from "$components/Icon.svelte"
	import Logo from "$components/Logo.svelte"
</script>

<section class="landing">
	<h1>
		Hi, I'm <br /> JD van Staden
		<!-- <Logo size="0.9em" color="var(--color-primary-400)" /> -->
	</h1>
	<p>
		I'm a junior software engineer at Old Mutual Investment Group based in Cape Town, South Africa working .
		My interests lie within Artificial Intelligence, Educational Tecnology and Cybersecurity. Send me a message on LinkedIn if you're up for a chat 😊
	</p>
	<hr class="bold" />
	<ul class="links">
		<li>
			<a
				href="https://github.com/jaleel-vs"
				title="GitHub profile"
				target="_blank"
				rel="noopener"
			>
				<Icon title="GitHub Icon" path={mdiGithub} size="1.5em" />
				<span>GitHub</span>
				<Icon path={mdiOpenInNew} />
			</a>
		</li>
		<li>
			<a
				href="https://www.linkedin.com/in/jd-van-staden/"
				title="LinkedIn profile"
				target="_blank"
				rel="noopener"
			>
				<Icon title="GitHub Icon" path={mdiLinkedin} size="1.5em" />
				<span>LinkedIn</span>
				<Icon path={mdiOpenInNew} />
			</a>
		</li>
		<li>
			<a
				href="https://rxresu.me/eusebio77/jaleel2024"
				title="CV"
				target="_blank"
				rel="noopener"
			>
				<Icon title="GitHub Icon" path={mdiFileDocument} size="1.5em" />
				<span>CV</span>
				<Icon path={mdiOpenInNew} />
			</a>
		</li>
	</ul>
</section>

<style>
	.landing {
		grid-area: landing;
	}

	h1 :global(.svg-icon) {
		top: 0.15em; /* visual balance */
	}

	hr {
		width: 4em;
		margin: calc(1.5 * var(--line-space)) 0;
	}

	ul.links {
		display: flex;
		flex-direction: row;
		gap: 1em;
		list-style-type: none;
		margin-bottom: var(--line-space);
	}

	ul.links li {
		float: left;
		margin-bottom: var(--line-space);
	}

	ul.links a {
		display: flex;
		align-items: center;
		float: left;
	}

	ul.links a:hover {
		text-decoration: underline;
	}

	ul.links span {
		padding-left: 0.75em;
		padding-right: 0.6em;
	}
</style>

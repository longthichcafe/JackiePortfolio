<footer>
	<p class="company">
		<a target="_blank" href="https://www.linkedin.com/in/longhaiho/">My LinkedIn 🤙</a>
	</p>

	<p class="details">
		<a target="_blank" href="https://drive.google.com/file/d/1PGIHf-Jqjw0E5ukfRM3oYATAAUi7kuNy/view?usp=sharing">My Resume 📮</a> 

		<small>Generated at {new Date().toISOString()}</small>
	</p>

	<p class="source">
		<a target="_blank" href="https://github.com/longthichcafe">👨‍💻 Projects</a>
	</p>
</footer>

<style>
	footer {
		display: grid;
		grid-template-columns: 1fr 1fr;
		align-items: center;
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		text-align: center;
		padding: 2.5rem;
		box-sizing: border-box;
		font-size: 16px;
	}

	p {
		margin: 0.5em 0;
	}

	a {
		color: var(--fg);
		text-decoration: none;
	}

	a:hover {
		text-decoration: hover;
		scale: 1.1;
		transition: ease-in-out;
		transition-duration: 0.2s;
	}

	.details {
		order: 3;
		grid-column: 1/3;
		white-space: nowrap;
		font-weight: 600;
	}

	.source,
	.company {
		display: flex;
		align-items: center;
		font-weight: 600;
	}

	.source {
		gap: 0.5rem;
		align-items: center;
		justify-content: flex-end;
	}

	.company {
		font-weight: 600;
		white-space: nowrap;
		justify-content: start;
	}

	.company svg {
		height: 1em;
		position: relative;
		top: 0.2em;
	}

	.source a,
	.company a {
		color: var(--fg);
	}

	small {
		position: absolute;
		left: 0;
		bottom: 20px;
		text-align: center;
		width: 100%;
		font-size: 11px;
		color: #999;
	}

	@media (min-width: 800px) {
		footer {
			display: flex;
			justify-content: space-around;
		}

		.source,
		.company {
			width: 10em;
		}

		.details {
			order: 0;
			grid-column: 1/3;
		}
	}
</style>

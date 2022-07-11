<main>
	<div class="wrapper">
		<div class="row">
			<div class="col span10 content">
				<h2 class="textbox1">
					I am <span id="underlined"
						>Innopolis University student</span
					>
					keen on <span class="wave_underlined">ML engenering</span>
					and wish for creating cost-effective and proficient
					<span class="wave_underlined">neural networks</span>
				</h2>
				<div class="contactbox">
					<h3>My contacts:</h3>
					<ul>
						<li>
							<a href="mailto:a.rusin@innopolis.university"
								><img src="outlook.png" alt="email" />
								Email</a
							>
						</li>
						<li>
							<a href="https://github.com/FurryLord"
								><img src="github.png" alt="github" />
								Github</a
							>
						</li>
						<li>
							<a href="https://t.me/Furry_Lord"
								><img src="telegram.png" alt="img" /> Telegram</a
							>
						</li>
						<li>
							<a href="https://vk.com/arseniruss"
								><img src="vk.png" alt="vk" /> VK</a
							>
						</li>
					</ul>
				</div>
				<br />
				<div class="textbox2">
					<h3>Looking forward for you messages!</h3>
				</div>
			</div>
			<div class="col span5 offset-by-one">
				<div class="image_container">
					<img src="mascot.jpg" alt="mascot" />
					<div class="top-left_image">
						<h3>My mascot - InnoFox ^^</h3>
					</div>
				</div>
			</div>
		</div>
	</div>
</main>

<style>
	/* Сhanging some heading styles */
	.textbox2 h3 {
		margin-block-start: 0em;
		margin-block-end: 0em;
	}

	/* Containers for main content */
	.textbox1 {
		background-color: #7f55db;
		padding-top: 2%;
		padding-bottom: 3%;
		border-radius: 15px;
		word-break: break-word;
		overflow: auto;
		margin-block-start: 0em;
		padding: 5% 5% 5% 5%;
	}

	.contactbox {
		background-color: #7f55db;
		padding: 1% 5% 1% 5%;
		border-radius: 15px;
		word-break: break-word;
		overflow: auto;
		margin-top: 4%;
	}

	.textbox2 {
		background-color: #7f55db;
		padding: 1% 5% 1% 5%;
		border-radius: 15px;
		word-break: break-word;
		overflow: auto;
	}

	.content {
		margin-left: 4%;
	}

	/* Some decorators for text */

	#underlined {
		text-decoration: underline;
	}

	.wave_underlined {
		text-decoration: underline;
		text-decoration-style: dotted;
		color: aliceblue;
	}

	/* Styles for pictures included in list
   They are clicable too
*/

	li img {
		width: 16px;
		height: 16px;
		display: inline;
	}

	/* Animation for image (scales it inside container block) */

	img:hover {
		transform: scale(1.2);
	}

	ul img:hover {
		transform: scale(1.4);
		transition: 0.3s;
	}

	.image_container {
		border-radius: 15px;
		position: relative;
		text-align: center;
		overflow: hidden;
	}

	/* Container for text at top-left angle of image */
	.top-left_image {
		position: absolute;
		top: 0%;
		left: 0%;
		background: hsla(21, 37%, 15%, 0.2);
		padding-left: 2%;
		padding-right: 2%;
	}

	/* Styles for list elements notation */

	ul {
		padding-left: 1rem;
		list-style-type: none;
	}

	li {
		font-size: 1.2rem;
	}

	/* Animation for links */

	a {
		color: white;
	}
	a:hover {
		color: #53359f;
	}

	a:focus {
		background: #53359f;
	}

	.row a {
		font-family: "Trebuchet MS";
		text-decoration: none;
	}

	img {
		width: 100%;
		height: auto;
		transition: 1s;
		display: block;
	}
</style>

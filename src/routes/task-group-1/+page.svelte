<script>
	// [Task 1]
	// Create any type of greeting and save it into a variable as a String
	let greeting = 'hola mundo';

	// [Task 2]
	// Create a JSON Object representing a video game. The game should have the following fields:
	// 1) gameName: String
	// 2) gameGenre: String
	// 3) gamePrice: Float
	let game = {
		gameName: 'Elden Ring',
		gameGenre: 'RPG',
		gamePrice: 60.0
	};

	// [Task 3]
	// Create a function that returns the speed of light in "Miles" as a plain Integer
	function speedOfLight() {
		return 186000;
	}

	// [Task 4]
	// Create a function that takes an argument `x`
	// The function should multiple `x` by 4 and return the result
	function calc(x) {
		return x * 4;
	}
</script>

<!-- Take the greeting variable you made in [Task 1] and put it below (replace the String Literal) -->
<h1>{greeting}!!!!</h1>

<!-- Take the JSON Object from [Task 2] and fill in the paragraph element below -->
<p>
	The video game {game.gameName} is part of the {game.gameGenre} genre. It is priced at {game.gamePrice}
	US Dollars
</p>

<!-- Using the JSON Object from [Task 2] fill out the paragraph below -->
<!-- Subtract a members discount of 10 dollars from the price in side the paragraph -->
<!-- NOTE: Do NOT subtract 10 from the variable it's self, just do it inside the {}'s in order to render it  -->
<p>With your member discount {game.gameName} is now {game.gamePrice - 10} US Dollars</p>

<!-- Use [Task 3] to fill out the header 2 below  -->
<h2>The Speed of Light: {speedOfLight()} Miles per Second</h2>

<!-- Use the function from [Task 4] to fill out the header 2 below -->
<h2>10 * 4 = {calc(10)}</h2>

<!-- Change the String Literal below back to it's original state (Lowercase instead of uppercase) -->
<!-- The Challenge: You must do this without altering the existing code. You may only add code instead the {}'s -->
<h1>{'abc'.toUpperCase().toLowerCase()}!!!!</h1>

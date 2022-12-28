<script>
	let html_string = `here's some <strong>HTML!!!</strong>`

	// [Task 1]
	// Create a JSON Object named `person` with the following fields:
	// 1) firstName: String
	// 2) lastName: String
	let person = {
		firstName: "Juan",
		lastName: "Pérez"
	}
	
	// [Task 2]
	// Create a String literal. It can contain any message, however, insert the firstName and lastName fields into the String
	// Be creative on how you use these 2 variables to create a message
	let message = `We know the suspect is called ${person.firstName}, but we are missing the last name. It could be either López or ${person.lastName}`

	// [Task 3]
	// Insert the String Literal made in [Task 2] into another String Literal. 
	// Use this new variable to wrap your original message in html. Specificity make your message have a strike through it
	// Example Of A Strike: https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_s
	let message2 = `<s>Police Report: ${message}</s>`

</script>

<!-- Fix this header 2 so it displays as HTML and not as a raw String -->
<h2>{@html html_string }</h2>

<!-- Display the message made in [Task 3] as html -->

<p>{@html message2 }</p>
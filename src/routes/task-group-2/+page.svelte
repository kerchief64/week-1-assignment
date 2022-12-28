<script>
	// [Task 1]
	// Find an image or gif online. Take the full URL and save it into a variable
	let gif = 'https://media.tenor.com/JMzBeLgNaSoAAAAj/banana-dance.gif';

	// [Task 2]
	// Create an "alt"erative name for the image in case it fails to load. Save it into a variable
	let gifAlt = 'Dancing Banana';

	// [Task 3]
	// Create a JSON Object that represents an image with the following fields
	// Note: Be sure to make the width 100, the height is up to you
	// 1) Image Src: String
	// 2) Image Alt: String
	// 3) Width: Integer
	// 4) Height: Integer
    let image = {
        src: "https://toppng.com/uploads/preview/ok-oki-emotions-ftstickers-emoji-emojistickers-yelowfac-smiley-face-thumbs-u-11562910345kljbwmanw5.png",
				alt: "cool",
				width: 100,
				height: 100,
    }

	// [Task 4]
	// Create a function that returns 75
	function return_75() {
		return 75;
	}

	// [Task 5]
	// Create a function that takes `x` as an argument
	// Return `x` minus 30
	function calc(x) {
		return x - 30;
	}
</script>

<!-- Create an image with the src and alt defined in the variables created in [Task 1] and [Task 2] -->
<img src={gif} alt={gifAlt} />

<br /><br />

<!-- Create an image using the Object created in [Task 3] -->
<!-- Challenge: Subtract 50 from the width without changing the variable itself. It should be done within the {}'s -->
<img src={image.src} alt={image.alt}/>

<br /><br />

<!-- Create an image using the Object created in [Task 3]. However, this time do the following -->
<!-- 
    1) The width should be the default width in the Object, minus the returned value of the function created in [Task 4] 
    2) The height from the image Object should be used as the argument in the function created in [Task 5]. What ever value is returned should be the final height
    3) Add "!!!" to the normal alt value without altering the value itself. This should happen inside the {}'s
-->

<img src={image.src} alt={image.alt + "!!!"} width={image.width - return_75()} height={calc(image.height)}>

<br /><br />

<!-- Create an image with all the default values in the image Object. -->
<!-- 
    Challenge: Make the image always span across the whole screen by changing the unit of the width
    Notes:
    1) Normally the default unit for an image width is "px", even if you don't specify it
    2) The value inside the image Object itself does NOT need to be altered in anyway to make this work
-->
<img src={image.src} alt={image.alt} style="width: {image.width}vw;"/>

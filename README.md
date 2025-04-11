# bikram
<!DOCTYPE html>
<html>
<head>
<title>Image Collage</title>
<style>
  .collage-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); /* Responsive columns */
    grid-gap: 10px; /* Spacing between images */
    padding: 20px; /* Padding around the collage */
  }

  .collage-item {
    overflow: hidden; /* To contain images within their bounds */
    border-radius: 5px; /* Optional: Rounded corners */
    box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1); /* Optional: Subtle shadow */
  }

  .collage-item img {
    width: 100%; /* Make images fill their container */
    height: auto; /* Maintain aspect ratio */
    display: block; /* Remove extra space below inline images */
    transition: transform 0.3s ease-in-out; /* Optional: Smooth hover effect */
  }

  .collage-item img:hover {
    transform: scale(1.05); /* Optional: Slight zoom on hover */
  }

  /* You can add more specific styles for different image sizes or layouts */
  /* For example, to make some images span two columns: */
  /*.collage-item:nth-child(3n) {
    grid-column: span 2;
  }*/
</style>
</head>
<body>

  <h1>My Image Collage</h1>

  <div class="collage-container">
    <div class="collage-item">
      <img src="image1.jpg" alt="Image 1">
    </div>
    <div class="collage-item">
      <img src="image2.png" alt="Image 2">
    </div>
    <div class="collage-item">
      <img src="image3.gif" alt="Image 3">
    </div>
    <div class="collage-item">
      <img src="image4.jpeg" alt="Image 4">
    </div>
    <div class="collage-item">
      <img src="image5.webp" alt="Image 5">
    </div>
    <div class="collage-item">
      <img src="image6.svg" alt="Image 6">
    </div>
    </div>

</body>
</html>
---
layout: page
title:  Artists
permalink: /gallery
---
<br>

<!-- The expanding image container -->
<div class="container-2">
  <!-- Close the image -->
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>

  <!-- Expanded image -->
  <img id="expandedImg" style="width:100%">

  <!-- Image text -->
  <div id="imgtext"></div>
</div>
<div class="row">
  <div class="column">
    <img src="/hadriana/img/IAMD-002.jpg" alt="Nature" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="/hadriana/img/IAMD-005.jpg" alt="Snow" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="/hadriana/img/IAMD-003.jpg" alt="Mountains" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="/hadriana/img/tapestry.jpg" alt="Lights" onclick="myFunction(this);">
  </div>
</div>
<script>
function myFunction(imgs) {
  // Get the expanded image
  var expandImg = document.getElementById("expandedImg");
  // Get the image text
  var imgText = document.getElementById("imgtext");
  // Use the same src in the expanded image as the image being clicked on from the grid
  expandImg.src = imgs.src;
  // Use the value of the alt attribute of the clickable image as text inside the expanded image
  imgText.innerHTML = imgs.alt;
  // Show the container element (hidden with CSS)
  expandImg.parentElement.style.display = "block";
}
</script>
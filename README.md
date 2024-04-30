<OWAOWA>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
p {
  text-align: center;
  font-size: 60px;
  margin-top: 0px;
}
</style>
</head>
<body>

<p id="demo"></p>

<script>
// Set the date we're counting down to
var countDate = new Date(" Aug 30, 2023 00:21:07:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distance = now - countDate;
    
  // Time calculations for days, hours, minutes and seconds
  var years = Math.floor(distance / (1000 * 60 * 60 * 24));
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
  
  // Output the result in an element with id="demo"
  document.getElementById("demo").innerHTML = years + "y" + days + "d " + hours + "h "
  + minutes + "m " + seconds + "s";
    
}, 1000);
</script>

</body>
</html>

<div class="wrapper">
$color-text: #525252;
$color-link: #525252;
$color-link-hover: #525252;

body {
  font-family: "ArcadePix",Helvetica,Arial,sans-serif;
  // Fallback for old browsers
  background: #16222A;

  background: -webkit-linear-gradient(to left, #16222A , #3A6073);
  background: linear-gradient(to left, #16222A , #3A6073);
  
  color: #525252;
}

a {
  color: $color-link;
  
  &:hover {
    color: $color-link-hover;
  }
}

h1 {
  text-align: center;
}

.timer {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 128px;  
  font-family: "ArcadePix","ArcadePix",Gadget,sans-serif;
}

html, body {
  margin: 0;
  height: 100%;
}

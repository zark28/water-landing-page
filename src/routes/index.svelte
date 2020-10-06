<script>

</script>
<style>
  
  h1{
    position:absolute;
    font-size: 20em;
    font-weight: 600;
    top: 25%;
    left: 50%;
    transform: translate(-50%,-50%);
    color: rgba(0, 0, 0, 0.459);
      }

  .icons{
    position:absolute;
    top: 90%;
    left: 70%;
    transform: translate(-50%,-50%);
    width: 18em;
    height: 3em;
    border-radius: 2em;
    background-color:#00000057;
    display: flex;
    justify-content: space-evenly;
  }
   .icons img{
     width: 2em;
     padding: .5em;
     filter: invert(0%) sepia(100%) saturate(0%) hue-rotate(13deg) brightness(95%) contrast(105%);
   }
  
</style>

<svelte:head>
  <title>Sapper project template</title>
</svelte:head>

<main class='content'>
  <h1>BEACH</h1>
  <div class='icons'>
    <a href> <img src="logo-facebook.svg" alt="facebook-link">    </a>
    <a href> <img src="logo-instagram.svg" alt="instagram-link">    </a>
    <a href> <img src="logo-youtube.svg" alt="youtube-link">    </a>
  </div>
</main>

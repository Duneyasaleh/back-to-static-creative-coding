<script>
    import bier from '$lib/pop-art-image/png/bier-time.png'
    import telefoon from '$lib/pop-art-image/png/telefoon.png'
    import bierMeid from '$lib/pop-art-image/png/bier-meid1.png'
    import bierboard from '$lib/pop-art-image/png/save-bier.png'
    import biertje from '$lib/pop-art-image/png/biertje.png'
</script>
<section id="section2">
<img class="telefoon" src="{telefoon}" alt="">  
<img class="bier-img" src="{bier}" alt="" width="500">
<img class="bier-meid" alt="" src="{bierMeid}">
<img class="biertje" src="{biertje}" alt="" width="300">
<img class="bier-board" src="{bierboard}" alt="" width="500" height="500" >


</section>

<style>
section{
    position: relative;
    width: 100vw;
    height: 100vh;
    background-color: red;
    border: 1.5rem solid black;
}
.telefoon{
    position: absolute;
    top: 0;
    right: 20%;
    animation: telefoontje 2s infinite;
}
.bier-img{
    position: absolute;
    bottom: 0;
}
.bier-meid{
    position: absolute;
    bottom: 0;
    right: 10%;
    animation: shake 5s infinite;
}
.bier-board{
    position: absolute;
    top: 20%;
    left: 35%;
 
}
.biertje{
    position: absolute;
    top: 0;
    left: 42%;
    animation: biertje 2s infinite;
}
@keyframes shake {
  10%, 90% {
    transform: translate3d(-1px, 0, 0);
  }
  
  20%, 80% {
    transform: translate3d(2px, 0, 0);
  }

  30%, 50%, 70% {
    transform: translate3d(-4px, 0, 0);
  }

  40%, 60% {
    transform: translate3d(4px, 0, 0);
  }
}

@keyframes telefoontje {
    0% {
        top: -7rem;
    }
 
    100% {
        top: 0;
    }
}
@keyframes biertje {
    0% {
        top: 7rem;
    }
 
    100% {
        top: 0;
    }
}
</style>
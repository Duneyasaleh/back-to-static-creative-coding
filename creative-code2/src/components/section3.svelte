<script>
    import bride from '$lib/pop-art-image/png/bride.png';
   import huilen from '$lib/pop-art-image/huilen.jpg';
   import fluister from '$lib/pop-art-image/fluister.webp';
   import kijken from '$lib/pop-art-image/kijken.webp';
   import stress from '$lib/pop-art-image/stress.jpg';
   import cute from '$lib/pop-art-image/cute.jpg';
   import gefeliciteerd1 from '$lib/pop-art-image/png/gefeliciteerd-meisje.png';
   import gefeliciteerd2 from '$lib/pop-art-image/png/gefeliciteerd.png';

</script>
<section id="section3">
<img class="bride" src="{bride}" alt="" >
<img src="{gefeliciteerd1}" alt="" class="gefeliciteerd1">
<div class="memories-img">
<img src="{huilen}" alt="" width="200">
<img src="{stress}" alt="" width="200">
<img src="{kijken}" alt="" width="200">
<img src="{fluister}" alt="" width="200">
<img src="{cute}" alt="" width="200">
</div>
<img src="{gefeliciteerd2}" alt="" class="gefeliciteerd2" width="300">
</section>

<style>
section{
    position: relative;
    width: 100vw;
    height: 100vh;
    background-color: hotpink;
    border: 1.5rem solid black;
    
}

.bride{
    position: absolute;
    left: 30%;
    bottom: 0;
}
.memories-img {
    position: relative;
}
.memories-img img{
    position: absolute;
    border: 1rem solid black;
    box-shadow: 10px 5px 5px hwb(0 0% 100% / 0.404);
}
.memories-img img:nth-child(2){
    right: 20%;
    top: 3em;
}
.memories-img img:nth-child(3){
    right: 40%;
    top: 3em;
}
.memories-img img:nth-child(4){
    right: 10%;
    top: 30em;
}
.memories-img img:nth-child(5){
    left: 10%;
    top: 20em;
}
.memories-img img:nth-child(1){
    left: 20%;
    top: 3em;
}
.gefeliciteerd1{
    position: absolute;
    top: 0;
    left: 34%;
    animation: gefeliciteerd1 2s infinite;
}
.gefeliciteerd2{
    position: absolute;
    bottom: 0;
    right: 20%;
    animation: gefeliciteerd2 2s infinite;
}
@keyframes gefeliciteerd1 {
    0% {
        top: -3rem;
    }
    100% {
        top: 0;
    }
}
@keyframes gefeliciteerd2 {
    0% {
        bottom: -3rem;
    }
    100% {
        bottom: 0;
    }
}
</style>
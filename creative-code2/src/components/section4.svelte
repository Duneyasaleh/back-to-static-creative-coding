<script>
    import wolk from '$lib/pop-art-image/png/bubbeltje2.png'
    import wolkBubble from '$lib/pop-art-image/png/wolk-bubble.png'
    import santaBier from '$lib/pop-art-image/png/santa-bier.png'
    import santaMeid from '$lib/pop-art-image/png/santa-meid.png'
    import santaParaplu from '$lib/pop-art-image/png/santa-paraplu.png'
</script>
<section id="section4">
    <div class="wolkje">
        <img src="{wolkBubble}" alt="" width="800">
        <img src="{wolk}" alt="" width="800" height="800">
        <h2>Merry christmas</h2>
    </div>
    <img src="{santaBier}" alt="" class="santaBier">
    <img src="{santaMeid}" alt="" class="santaMeid" width="400">
    <img src="{santaParaplu}" alt="" class="santaParaplu" width="300">
</section>

<style>
section{
    position: relative;
    width: 100vw;
    height: 100vh;
    background-color: green;
    border: 1.5rem solid black;
    
    
}
.wolkje{
    position: relative;
}
.wolkje img, h2 {
    position: absolute;
    left: 25%;
}
.wolkje img:nth-child(1) {
    top: 3.5rem;
    animation: wolk-bubble 2s infinite;
}
h2{
    font-family: 'Martian Mono', monospace;
    width: 500px;
    left: 34%;
    top: 21rem;
    font-size: 70px;
    text-align: center;
    text-shadow: red 1px 0 10px;
}
section > img{
    position: absolute;
}
.santaMeid{
    bottom: 0;
}
.santaBier{
    bottom: 0;
    right: 0;
}
@keyframes wolk-bubble {
    0%{
        width: 45%;

    }
    100%{
        width: 50%;
        left: 23%;
        top: 3em;
    }
}

</style>
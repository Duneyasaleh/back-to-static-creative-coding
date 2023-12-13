<script>
    import hondje from '$lib/pop-art-image/png/fit.png'
    import bubble from '$lib/pop-art-image/png/bubbeltje2.png'
    import stertjeLeft from '$lib/pop-art-image/png/ster-left.png'
    import stertjeRight from '$lib/pop-art-image/png/ster-right.png'
</script>
<section>
    <article>
        <img src="{stertjeLeft}" alt="" class="ster-left">
        <img src="{stertjeRight}" alt="" class="ster-right">
        <div class="bubbletje">
            <img src="{bubble}" alt="" srcset="" width="900" height="800" >
            <h1>Welkom op mijn kleurrijke kunstfeestje!</h1>
        </div>
    </article>
   
    <img src="{hondje}" alt="hondje" class="hondje" width="500" height="500">
</section>

<style>
section{
    width: 100vw;
    height: 100vh;
    background-color: #2BCBDC;
    border: 1.5rem solid black;
    
}
.hondje{
    position: absolute;
    bottom: 0;
    animation: naarboven 2s ease-out ;
}
article{
    position: absolute;
    right: 15%;
}
h1{
font-size: 45px;
font-family: 'Martian Mono', monospace;
width: 33rem;
 margin-top: -28rem;
 margin-left: 16rem;
 color: white;
 text-shadow: black 1px 0 10px;

}
.bubbletje {
  animation: shaking 2s infinite;
}
.ster-left{
    position: absolute;
    top: 0;
    animation: Ster 2s infinite;
    left:5rem;
}
.ster-right{
    position: absolute;
    top: 0;
    right: 0%;
    animation: Ster-right 2s infinite;
}
@keyframes naarboven {
  from {bottom: -15rem;}
  to {bottom: 0;}
}
@keyframes shaking {
  0% { transform: rotate(0deg); }
  25% { transform: rotate(5deg); }
  50% { transform: rotate(0eg); }
  75% { transform: rotate(-5deg); }
  100% { transform: rotate(0deg); }
}
@keyframes Ster {
  0% {
    transform: scale(0.5) translate(-100%, -100%);
    top: 10rem;
  }
  100% {
    top: 8rem;
    transform: scale(1.5) translate(-100%, -100%);
  }
}
@keyframes Ster-right {
  0% {
    transform: scale(0.5) translate(100%, -100%);
    top: 10rem;
  }
  100% {
    transform: scale(1.5) translate(100%, -100%);
    top: 8rem;
  }
}

</style>
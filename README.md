# <div id="flower"></div>

<script src="script.js"></script>
body{
    margin:0;
    background:black;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    overflow:hidden;
}

#flower{
    position:relative;
    width:500px;
    height:500px;
}

.petal{
    position:absolute;
    left:50%;
    top:50%;

    transform-origin:center center;

    opacity:.18;
    mix-blend-mode:screen;

    animation:bloom 6s ease-in-out infinite;
}

@keyframes bloom{

0%{
transform:translate(-50%,-50%)
scale(.2)
rotate(0deg);
opacity:0;
}

50%{
opacity:.3;
}

100%{
transform:translate(-50%,-50%)
scale(1.3)
rotate(360deg);
opacity:0;
}
const flower = document.getElementById("flower");

for(let i=0;i<220;i++){

    confor(let i=0;i<250;i++){

    push();

    rotate(i*0.02+t);

    scale(1+i*0.002);

    tint(255,12);

    image(flower,0,0);

    pop();

}st petal=document.createElement("img");

    petal.src="petals/petal.png";

    petal.className="petal";

    const angle=Math.random()*360;

    const size=150+Math.random()*120;

    const delay=Math.random()*6;

    petal.style.width=size+"px";

    petal.style.transform=
        `translate(-50%,-50%) rotate(${angle}deg)`;

    petal.style.animationDelay=`-${delay}s`;

    flower.appendChild(petal);

}

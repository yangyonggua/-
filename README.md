# -html{

background:linear-gradient(to right, #bb313e25, #bb313e25, #d7222925, #dd4a1625, #e4761525, #f5c50025, #f0e92725, #b1ce2425, #48a93525, #03944525, #157c4f25, #176a5825, #1b556325, #1d386f25, #1d386f25, #20277825, #52266325, #8a244b25);

/*background:linear-gradient(#FF6666 0%,#336699 20%);背景渐变颜色*/

    height: 100%;

    color:#99cc33;/*文字颜色*/

}



/*最外层容器样式*/

.wrap{

width: 200px;

height: 200px;

/*改变左右上下,图片方块移动*/

margin: 150px auto;

position: relative;

}

/*包裹所有容器样式*/

.cube{

width: 200px;

height: 200px;

margin: 0 auto;

transform-style: preserve-3d;

transform: rotateX(-30deg) rotateY(-80deg);

-webkit-animation: rotate 20s infinite;

/*匀速*/

animation-timing-function: linear;

}

@-webkit-keyframes rotate{

from{transform: rotateX(0deg) rotateY(0deg);}

to{transform: rotateX(360deg) rotateY(360deg);}

}

.cube div{

position: absolute;

width: 200px;

height: 200px;

opacity: 0.8;

transition: all .4s;

}

/*定义所有图片样式*/

.pic{

width: 200px;

height: 200px;

}

.cube .out_front{

transform: rotateY(0deg) translateZ(100px);

}

.cube .out_back{

transform: translateZ(-100px) rotateY(180deg);

}

.cube .out_left{

transform: rotateY(90deg) translateZ(100px);

}

.cube .out_right{

transform: rotateY(-90deg) translateZ(100px);

}

.cube .out_top{

transform: rotateX(90deg) translateZ(100px);

}

.cube .out_bottom{

transform: rotateX(-90deg) translateZ(100px);

}

/*定义小正方体样式

*/

.cube span{

display: bloack;

width: 100px;

height: 100px;

position: absolute;

top: 50px;

left: 50px;

}

.cube .in_pic{

width: 100px;

height: 100px;

}

.cube .in_front{

transform: rotateY(0deg) translateZ(50px);

}

.cube .in_back{

transform: translateZ(-50px) rotateY(180deg);

}

.cube .in_left{

transform: rotateY(90deg) translateZ(50px);

}

.cube .in_right{

transform: rotateY(-90deg) translateZ(50px);

}

.cube .in_top{

transform: rotateX(90deg) translateZ(50px);

}

.cube .in_bottom{

transform: rotateX(-90deg) translateZ(50px);

}

/*鼠标移入后样式*/

.cube:hover .out_front{

transform: rotateY(0deg) translateZ(200px);

}

.cube:hover .out_back{

transform: translateZ(-200px) rotateY(180deg);

}

.cube:hover .out_left{

transform: rotateY(90deg) translateZ(200px);

}

.cube:hover .out_right{

transform: rotateY(-90deg) translateZ(200px);

}

.cube:hover .out_top{

transform: rotateX(90deg) translateZ(200px);

}

.cube:hover .out_bottom{

transform: rotateX(-90deg) translateZ(200px);

}

.hovertreeinfo{text-align:center;}

.hovertreeinfo a{color:white}


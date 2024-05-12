.coin {
    width: 80px;
    height: 80px;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    position: relative;
}

.coin div {
    width: 100%;
    height: 100%;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}

.coin img {
    width: 100%;
    height:100%;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}

.coin {
  transition: -webkit-transform 1s ease-in;
  -webkit-transform-style: preserve-3d;
}
.coin div {
  position: absolute;
  -webkit-backface-visibility: hidden;
}
.coin .blue {
  z-index: 100;
}
.coin .red {
  -webkit-transform: rotateY(-180deg);
}

.coin.red {
    -webkit-transform: rotateY(-180deg);
}

.coin.flipblue {
  -webkit-animation: flipBlue 5s ease-out forwards;
  -moz-animation: flipBlue 5s ease-out forwards;
    -o-animation: flipBlue 5s ease-out forwards;
       animation: flipBlue 5s ease-out forwards;
}
.coin.flipred {
  -webkit-animation: flipRed 5s ease-out forwards;
  -moz-animation: flipRed 5s ease-out forwards;
    -o-animation: flipRed 5s ease-out forwards;
       animation: flipRed 5s ease-out forwards;
}

@-webkit-keyframes flipBlue {
  from { -webkit-transform: rotateY(0); -moz-transform: rotateY(0); transform: rotateY(0); }
  to { -webkit-transform: rotateY(2880deg); -moz-transform: rotateY(2880deg); transform: rotateY(2880deg); }
}
@-webkit-keyframes flipRed {
  from { -webkit-transform: rotateY(0); -moz-transform: rotateY(0); transform: rotateY(0); }
  to { -webkit-transform: rotateY(3060deg); -moz-transform: rotateY(3060deg); transform: rotateY(3060deg); }
}

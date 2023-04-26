
- body{
  margin: 0;
  padding: 0;
  background-color: #0c0b0c;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.heart{
  height: 70px;
  width: 70px;
  background-color: #f20044;
  position: relative;
  box-shadow: 10px 10px 90px #f20044;
  animation: animHeart .6s linear infinite;
}

@keyframes animHeart{
  0%{
       transform: rotate(-45deg) scale(1.07);
  }

  80%{
        transform: rotate(-45deg) scale(1);
  }

  100%{
        transform: rotate(-45deg) scale(.8);
  }
}

.heart::before{
  content: '';
  position: absolute;
  height: 70px;
  width: 70px;
  background-color: #f20044;
  box-shadow: -10px 10px 90px #f20044;
  top: -50%;
  border-radius: 50%;
}

.heart::after{
  content: '';
  position: absolute;
  box-shadow: 10px -10px 90px #f20044;
  height: 70px;
  width: 70px;
  background-color: #f20044;
  right: -50%;
  border-radius: 50%;
}

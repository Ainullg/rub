# <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>rubiks-cube</title>
</head>
<body>
   <h1>moh ainul yakin 
   </h1>
 
   <div class="container">
     <span></span>
     <span></span>
     <span></span>
     <span></span>
   </div><div><style>/* From Uiverse.io by terenceodonoghue */ 
    .container {
      position: absolute;
      top: 50%;
      left: 50%;
      border-radius: 50%;
      height: 96px;
      width: 96px;
      animation: rotate_3922 1.2s linear infinite;
      background-color: #9b59b6;
      background-image: linear-gradient(#9b59b6, #84cdfa, #5ad1cd);
    }
    
    .container span {
      position: absolute;
      border-radius: 50%;
      height: 100%;
      width: 100%;
      background-color: #9b59b6;
      background-image: linear-gradient(#9b59b6, #84cdfa, #5ad1cd);
    }
    
    .container span:nth-of-type(1) {
      filter: blur(5px);
    }
    
    .container span:nth-of-type(2) {
      filter: blur(10px);
    }
    
    .container span:nth-of-type(3) {
      filter: blur(25px);
    }
    
    .container span:nth-of-type(4) {
      filter: blur(50px);
    }
    
    .container::after {
      content: "";
      position: absolute;
      top: 10px;
      left: 10px;
      right: 10px;
      bottom: 10px;
      background-color: #fff;
      border: solid 5px #ffffff;
      border-radius: 50%;
    }
    
    @keyframes rotate_3922 {
      from {
        transform: translate(-50%, -50%) rotate(0deg);
      }
    
      to {
        transform: translate(-50%, -50%) rotate(360deg);
      }
    }
    </style></div>
<style> ::-ms-backdrop</style>
   <div class="loader">
     <span class="loader-text">loading</span>
       <span class="load"></span>
   </div><div>
    <style>/
        .loader {
          width: 80px;
          height: 50px;
          position: relative;
        }
        
        .loader-text {
          position: absolute;
          top: 0;
          padding: 0;
          margin: 0;
          color: #C8B6FF;
          animation: text_713 3.5s ease both infinite;
          font-size: .8rem;
          letter-spacing: 1px;
        }
        
        .load {
          background-color: hsl(255, 44%, 39%);
          border-radius: 50px;
          display: block;
          height: 16px;
          width: 16px;
          bottom: 0;
          position: absolute;
          transform: translateX(64px);
          animation: loading_713 3.5s ease both infinite;
        }
        
        .load::before {
          position: absolute;
          content: "";
          width: 100%;
          height: 100%;
          background-color: #D1C2FF;
          border-radius: inherit;
          animation: loading2_713 3.5s ease both infinite;
        }
        
        @keyframes text_713 {
          0% {
            letter-spacing: 1px;
            transform: translateX(0px);
          }
        
          40% {
            letter-spacing: 2px;
            transform: translateX(26px);
          }
        
          80% {
            letter-spacing: 1px;
            transform: translateX(32px);
          }
        
          90% {
            letter-spacing: 2px;
            transform: translateX(0px);
          }
        
          100% {
            letter-spacing: 1px;
            transform: translateX(0px);
          }
        }
        
        @keyframes loading_713 {
          0% {
            width: 16px;
            transform: translateX(0px);
          }
        
          40% {
            width: 100%;
            transform: translateX(0px);
          }
        
          80% {
            width: 16px;
            transform: translateX(64px);
          }
        
          90% {
            width: 100%;
            transform: translateX(0px);
          }
        
          100% {
            width: 16px;
            transform: translateX(0px);
          }
        }
        
        @keyframes loading2_713 {
          0% {
            transform: translateX(0px);
            width: 16px;
          }
        
          40% {
            transform: translateX(0%);
            width: 80%;
          }
        
          80% {
            width: 100%;
            transform: translateX(0px);
          }
        
          90% {
            width: 80%;
            transform: translateX(15px);
          }
        
          100% {
            transform: translateX(0px);
            width: 16px;
          }
        }
         
         
        
        </style>
   </div>
 

<div class="cube-loader">
  <div class="cube-top"></div>
  <div class="cube-wrapper">
    <span style="--i:0" class="cube-span"></span>
    <span style="--i:1" class="cube-span"></span>
    <span style="--i:2" class="cube-span"></span>
    <span style="--i:3" class="cube-span"></span>
  </div>
  <style>/* From Uiverse.io by andrew-demchenk0 */ 
    .cube-loader {
      position: relative;
    /* u can choose any size */
      width: 75px;
      height: 75px;
      transform-style: preserve-3d;
      transform: rotateX(-30deg);
      animation: animate 4s linear infinite;
    }
    
    @keyframes animate {
      0% {
        transform: rotateX(-30deg) rotateY(0);
      }
    
      100% {
        transform: rotateX(-30deg) rotateY(360deg);
      }
    }
    
    .cube-loader .cube-wrapper {
      position: absolute;
      width: 100%;
      height: 100%;
      /* top: 0;
      left: 0; */
      transform-style: preserve-3d;
    }
    
    .cube-loader .cube-wrapper .cube-span {
      position: absolute;
      width: 100%;
      height: 100%;
      /* top: 0;
      left: 0; */
                                         /* width 75px / 2 = 37.5px */
      transform: rotateY(calc(90deg * var(--i))) translateZ(37.5px);
      background: linear-gradient(
        to bottom,
        hsl(330, 3.13%, 25.1%) 0%,
        hsl(177.27, 21.71%, 32.06%) 5.5%,
        hsl(176.67, 34.1%, 36.88%) 12.1%,
        hsl(176.61, 42.28%, 40.7%) 19.6%,
        hsl(176.63, 48.32%, 43.88%) 27.9%,
        hsl(176.66, 53.07%, 46.58%) 36.6%,
        hsl(176.7, 56.94%, 48.91%) 45.6%,
        hsl(176.74, 62.39%, 50.91%) 54.6%,
        hsl(176.77, 69.86%, 52.62%) 63.4%,
        hsl(176.8, 76.78%, 54.08%) 71.7%,
        hsl(176.83, 83.02%, 55.29%) 79.4%,
        hsl(176.85, 88.44%, 56.28%) 86.2%,
        hsl(176.86, 92.9%, 57.04%) 91.9%,
        hsl(176.88, 96.24%, 57.59%) 96.3%,
        hsl(176.88, 98.34%, 57.93%) 99%,
        hsl(176.89, 99.07%, 58.04%) 100%
      );
    }
    
    .cube-top {
      position: absolute;
      width: 75px;
      height: 75px;
      background: hsl(330, 3.13%, 25.1%) 0%;
                          /* width 75px / 2 = 37.5px */
      transform: rotateX(90deg) translateZ(37.5px);
      transform-style: preserve-3d;
    }
    
    .cube-top::before {
      content: '';
      position: absolute;
    /* u can choose any size */
      width: 75px;
      height: 75px;
      background: hsl(176.61, 42.28%, 40.7%) 19.6%;
      transform: translateZ(-90px);
      filter: blur(10px);
      box-shadow: 0 0 10px #323232,
                  0 0 20px hsl(176.61, 42.28%, 40.7%) 19.6%,
                  0 0 30px #323232,
                  0 0 40px hsl(176.61, 42.28%, 40.7%) 19.6%;
    }
    </style>
</div>
<div class="my-loader">
  <div class="rubiks-cube">
    <div class="face front">
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
    </div>

    <div class="face back">
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #050201;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
    </div>
    <div class="face left">
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
    </div>
    <div class="face right">
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
    </div>
    <div class="face top">
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
    </div>
    <div class="face bottom">
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
      <div style="background: #ffeb3b;" class="cube"></div>
      <div style="background: #4caf50;" class="cube"></div>
      <div style="background: #2196f3;" class="cube"></div>
      <div style="background: #ffffff;" class="cube"></div>
      <div style="background: #ff3d00;" class="cube"></div>
    </div>
  </div>
</div>
<style>
    .my-loader {
      width: 200px;
      height: 200px;
      perspective: 1000px;
      margin: 100px auto;
    }
    
    .rubiks-cube {
      width: 100%;
      height: 100%;
      position: relative;
      transform-style: preserve-3d;
      animation: my-rotateCube 5s infinite linear;
    }
    
    .my-loader .face {
      position: absolute;
      display: flex;
      flex-wrap: wrap;
      width: 100%;
      height: 100%;
    }
    
    .my-loader .face.front {
      transform: translateZ(100px);
    }
    .my-loader .face.back {
      transform: rotateY(180deg) translateZ(100px);
    }
    .my-loader .face.left {
      transform: rotateY(-90deg) translateZ(100px);
    }
    .my-loader .face.right {
      transform: rotateY(90deg) translateZ(100px);
    }
    .my-loader .face.top {
      transform: rotateX(90deg) translateZ(100px);
    }
    .my-loader .face.bottom {
      transform: rotateX(-90deg) translateZ(100px);
    }
    
    .my-loader .cube {
      width: calc(100% / 3);
      height: calc(100% / 3);
      box-sizing: border-box;
      border: 1px solid #000;
    }
    
    @keyframes my-rotateCube {
      0% {
        transform: rotateX(0deg) rotateY(0deg);
      }
      100% {
        transform: rotateX(360deg) rotateY(360deg);
      }
    }
    </style>
</body>
</html>

</html>


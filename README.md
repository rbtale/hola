/* reset css */

* {
    min-width: 0;
    font: inherit;
  }
  
  *,
  *::before,
  *::after {
    box-sizing: border-box;
  }
  
  img,
  video,
  svg {
    display: block;
    height: auto;
    max-width: 100%;
  }
  
  body {
    margin: 0;
    min-height: 100dvh;
  }
  
  h1,
  h2,
  h3 {
    text-wrap: balance;
  }
  
  p {
    text-wrap: pretty;
  }
  
  /* styles */
  /* TODO: Cambiar la fuente
  
  * {
    font-family: comic-sans;
  } */
  
  body {
    background-color: #fab0f4;
  }
  
  main {
    display: flex;
    flex-direction: column;
  
    gap: 3rem;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  .container-letter {
    position: relative;
  }
  
  .cover {
    position: absolute;
    border-left: 200px solid transparent;
    border-right: 200px solid transparent;
    border-top: 100px solid #fe3334;
    border-bottom: 100px solid transparent;
  
    /*  */
    transition: transform .75s;
    transform-origin: top;
  }
  
  .paper {
    position: absolute;
    padding: 1.5rem;
    line-height: 1rem;
    right: 5px;
    /*  */
    z-index: -1;
    background: white;
    width: 390px;
    height: 180px;
  
    transition: all .75s;
  }
  
  .letter {
    border-left: 200px solid #ff989e;
    border-right: 200px solid #ff989e;
    border-top: 100px solid transparent;
    border-bottom: 100px solid #ff858a;
  }
  
  .options {
    display: flex;
    gap: 5rem;
  
    & button {
      color: #ff3234;
      font-weight: 600;
      border-radius: 3px;
      background: #fad7df;
      padding: 0.5rem 1rem;
      border: 1px solid #fe3334;
      cursor: pointer;
    }
  
    & button:hover {
      background: #ff989e;
      color: white;
    }
  }
  
  .open-cover {
    transform: rotatex(180deg);
  }
  
  .open-paper {
    animation: openPaper .5s forwards;
  }
  
  @keyframes openPaper {
    0% {
      top: 0;
    }
    100% {
      top: -120px;
    }
  }
  
  .close-paper {
    animation: closePaper .5s forwards;
  }
  
  @keyframes closePaper {
    0% {
      top: -120px;
    }
    100% {
      top: 0;
    }
  }
  
  
  .heart {
    display: none;
    position: absolute;
    top: 25%;
    left: 46.5%;
    margin: auto;
    font-size: 3rem;
  
    color: #fe3334;
  
    animation: crecer 1s forwards ;
  }
  
  @keyframes crecer {
    0% {
      scale: 1;
      opacity: 1;
    }
    100% {
      scale: 3;
      opacity: 0;
  
    }
  }

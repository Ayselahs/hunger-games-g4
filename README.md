# hunger-games-g4

#ayselahSmith


  @media screen and (max-width: 1100px) {
    body {
    grid-template-areas: 
    'header'
    'nav'
    'main'
    'footer';
    grid-template-columns: 1fr;
    grid-template-rows: repeat (4, 120px);
    }
  
  .header__title {
      font-size: 2rem;
    }
  
    .nav {
      padding: 0 20px 40px;
  
    }
    .nav__container {
      width: 80vw;
      min-width: 300px;
      grid-template-columns: repeat(4, 1fr);
      grid-auto-rows: initial;
      grid-auto-flow: column;
      justify-items: center;
      align-items: center;
    }
    .nav__link, .nav__link--active {
      text-decoration: underline;
    }
    .nav__link--active {
      padding: 0;
    }
    .nav__link::after, .nav__link--active::after {
      display: none;
    }
  }












  :root {
    --primary:red;
    --gray: hsl(217, 11%, 64%);
    --white: hsl(216, 100%, 95%);
    --highlight: yellow;
  }
  
  body {
    font-size: 1.2rem;
    margin: 0;
    box-sizing: border-box;
    min-height: 100vh;
    background-color: black;
    display: grid;
    grid-template-areas: 
    'header header'
    'jumbotron jumbotron'
    'nav main'
    'footer footer';
    grid-template-columns: 300px auto;
    grid-template-rows: repeat (4, auto);
  }
  
  .header__home {
    background-color: var(--primary);
    color: var(--white);
    padding: 20px;
    display: grid;
    align-items: center;
    justify-items: center;
    grid-area: header;
  }

.nav {
    grid-area: nav;
  }
  
.jumbotron {
    display: grid;
    grid-area: jumbotron;
    background-color: orange;
    padding: 20px;
  }

 .jumbotron__heading {
    font-size: 3rem;
    margin: 0;
  }
  
  .header__nav {
    grid-area: nav;
    justify-self: center;
    box-shadow: var(--gray) 4px 4px 10px 2px;
    row-gap: 24px;
    grid-template-columns: 1fr;
    min-width: 200px;
    justify-items: center;
    padding: 12px 0 24px;
  }

.header__home .nav__link  {
    text-decoration: none;
    color: var(--primary);
    position: relative;
  }

  .nav__link::after, .nav__link--active::after {
    position: absolute;
    content: "";
    bottom: 0;
    left: 50%;
    margin-left: -90px;
    border-bottom: var(--primary) 1px solid;
    width: 180px;
  }
  
  .nav__link--active {
    box-shadow: inset var(--highlight) 200px 0px 0px 1px;
    padding: 0 70px;
  }
  
.main {
    grid-area: main;
    max-width: 600px;
    background-color: white;
    justify-items: center;
}

.main__heading .main__subheading {
    background-image: url("jumbotron_img.jpg");
}

  .footer {
    display: grid;
    align-items: center;
    justify-items: center;
    grid-area: footer;
    background-color: var(--primary);
  }
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Forum');
:root {
  --black: #000000;
  --darkgray: #4e463d;
  --light-gray:#4f4a3b;
  --green: #414914;
  --red: #bf412a;
  --orange: #c86203;
  --white: #ffffff;
}

/* flexbox structure */
.main__column {
  -webkit-flex: 2;
  -ms-flex: 2;
  flex: 2;
}

.column__side {
  -webkit-flex: 1;
  -ms-flex: 1;
  flex: 1;
}

.body {
    margin: 0;
    min-height: 100vh;
    font-family: 'Montserrat', sans-serif;
    font-size: 1em;
    display: float;
    background-image: url("https://www.toptal.com/designers/subtlepatterns/uploads/grey_wash_wall.png");
}

.header {
    background-color: #c86203;
    display: flex; 
    align-items: flex-end;
    color: black;
    align-items: center;
    justify-items: space-around;
    font-size: 1em;
    height: 60px;
}

.nav__container {
  min-height: 60px;
  display: flex; 
  justify-content: space-between;
  align-items: center;
  width: 100%;
  flex-direction: row;
  padding-left: 15px;
  padding-right: 15px; 
  font-size: .75em; 
}

.nav__home {
  float: left;
}

.nav__link {
  float: right;
}

.nav__link, .nav__home {
  color: white;
  text-decoration: none;
  font-size: 1em;
  padding: 10px;
  margin-right: auto;
}

.nav__link:hover, .nav__home:hover {
  background-color: white;
  color: #bf412a;
}

.nav__container .nav__icon {
  display: none;
}

.nav__icon {
  color: #ffffff;
  padding: 10px;
}

.nav__icon:hover {
  color: #c86203;
  background-color: white;
  padding: 10px;
}

.jumbotron {
  background-image: url("images/jumbotron_img.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  border-top: solid #bf412a 10px;
  border-bottom: solid #bf412a 10px;
  display: flex; 
  flex-direction: column;
  justify-items: center;
  align-items: center;
  text-align: center; 
  padding: 20px;
}

.jumbotron__text {
  font-size: 3.5em;
  align-self: center;
  background-color: black;
  color: white;
  margin: 20; 
  padding: 20px 40px;
}

.jumbotron__btn {
  background-color: #bf412a;
  color: #ffffff;
  font-weight: bold;
  font-size: 1em;
  border-radius: 12px;
  border: none;
  cursor: pointer;
  padding: 12px;
  text-transform: uppercase;
}

.jumbotron__btn:hover {
  background-color: white; 
  border: solid 2px #bf412a;
  color: #bf412a;
}

.sidebar {
  background-color: white;
  width: 200px;
  height: auto;
  position: fixed;
  z-index: 1;
  right: 0;
  display: inline-block;
  padding: 10px;
  margin-right: 50px;
  overflow-x: hidden;
  text-align: center;
}

.nav__sidebar {
  width: 180px;
  text-align: center;
}

.sidebar__header {
  color:#4e463d;
  font-size: 1.25em;
}

.sidebar__link {
  text-decoration: none;
  color: #c86203;
  padding: 10px;
  font-size: .75em;
}

.sidebar__link:hover {
  background-color: #c86203;
  color: white;
  transition: 450ms;
}

.main {
  display: inline-block;
  width: 70%;
  background-color: white;
  box-shadow: gray 4px 4px 10px 2px;
  padding: 20px;
  margin: 30px;
  color: #4f4a3b
}

.main__heading {
  text-align: center;
}

.cast__gallery {
  padding: 5px;
  float: left;
  width: 180px;
}

.cast__gallery_list {
  list-style-type: none;
}

.cast__gallery img {
  width: 100%;
  height: auto;
}

.cast__gallery a {
  text-decoration: none;
  color: #bf412a;
  text-align: center;
  font-size: .8em;
}

.clearfix:after {
  content: "";
  display: table;
  clear: both;
}

.plot {
  display: flexbox;
  flex-direction: row; 
  flex-wrap: wrap;
}

/* Image Grid */
.cast__img_container {
  display: grid;
	grid-template-columns: repeat(3, 1fr);
	grid-gap: 20px;
  align-items: center;
}

.cast__img_grid {
  display: flex;
	flex-direction: column;
	align-items: center;
	text-align: center;
}

.cast__img_grid img {
  width: 50%;
	height: auto;
  border-top-left-radius: 3px;
  border-top-right-radius: 3px;
}

.cast__caption {
  margin-top: 10px;
	font-size: 1rem;
}

/* Trailer */
.trailer {
  margin-top: 50px;
}

/* Responsive Video */
.vid-wrapper {
  position: relative;
	padding-bottom: 56.25%;
	height: 0;
	overflow: hidden;
	max-width: 100%;
}

.vid-wrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.plot__image1 {
  width: 30%;
  float: left;
  padding-right: 10px;
}

.plot__image2 {
  width: 30%;
  float: right;
  padding-left: 10px;
}

.plot__image3 {
  width: 50%;
  float: left; 
  padding-right: 10px;
}

.plot__image4 {
  width: 50%;
  float: right; 
  padding-right: 10px;
}

h1, h2, h3 {
  font-family: 'Forum', cursive;
  text-transform: uppercase;
}

h1 {
  font-size: 3em;
}

h2 {
  font-size: 2em;
}

h3 {
  font-size: 1.5em;
}

.footer {
  text-align: center;
  background-color: #c86203;
  padding: 20px;
  font-size: 0.75em;
}

/* responsive layout */
@media screen and (max-width: 400px) {
  .nav__container a {display: none;}
  .nav__container a.nav__icon {
    float: left;
    display: block;
  }

  .nav__container.responsive {position: relative;}
  .nav__container.responsive .nav__icon {
    position: absolute;
    right: 0;
    top: 0;
  }
  .nav__container.responsive a {
    float: none;
    display: block;
    text-align: left;
  }

  .sidebar {
    display: none;
  }

  .jumbotron {
    max-width: 100%;
  }
  
  .main__row {
  -webkit-flex-direction: column;
  flex-direction: column;
  }

  .cast__gallery.responsive {
    width: 49.99999%;
    margin: 6px 0;
  }

  .cast__img_grid img {
    width: 100%;
    height: auto;
    border-top-left-radius: 3px;
    border-top-right-radius: 3px;
  }

}

@media screen and (max-width: 1112px) {
  .sidebar {
  display: none;
  }

  .cast__img_grid img {
    width: 100%;
    height: auto;
    border-top-left-radius: 3px;
    border-top-right-radius: 3px;
  }
}


<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>The Hunger Games Movie Quadrilogy Fan Page</title>
        <link rel="stylesheet" href="style.css" />
        <link
            rel="stylesheet"
            href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
        />
    </head>
    <body class="body">
        <header class="header">
            <div class="nav__container">
                <a href="index.html" class="nav__home">HOME</a>
                <nav class="nav">
                    <a href="mockj-2.html" class="nav__link"
                        >Mockingjay Part 2</a
                    >
                    <a href="mockj-1.html" class="nav__link"
                        >Mockingjay Part 1</a
                    >
                    <a href="#" class="nav__link">Catching Fire</a>
                    <a href="hungergames.html" class="nav__link"
                        >The Hunger Games</a
                    >
                    <a
                        href="javascript:void(0);"
                        class="nav__icon"
                        onclick="myFunction()"
                    >
                        <i class="fa fa-bars"></i
                    ></a>
                </nav>
            </div>
        </header>
        <section class="jumbotron">
            <p class="jumbotron__text">The World Will Be Watching</p>
            <button class="jumbotron__btn">Explore</button>
        </section>
        <main class="main">
            <div class="column__side">
                <div class="sidebar">
                    <h3 class="sidebar__header">The Quadrilogy</h3>
                    <nav class="nav__sidebar">
                        <a href="hungergames.html" class="sidebar__link"
                            >The Hunger Games</a
                        >
                        <a href="#" class="sidebar__link">Catching Fire</a>
                        <a href="mockj-1.html" class="sidebar__link"
                            >Mockingjay Part 1</a
                        >
                        <a href="mockj-2.html" class="sidebar__link"
                            >Mockingjay Part 2</a
                        >
                    </nav>
                </div>
            </div>
            <div class="main__column">
                <section class="info">
                    <h2 class="main__heading">Welcome</h2>
                    <p class="info__text">
                        This is a website celebrating "The Hunger Games" movie
                        series. The Hunger Games is a film directed by Gary
                        Ross, based on the 2008 novel of the same name written
                        by Suzanne Collins. The Hunger Games is the first
                        installment of the film series. While the book is a
                        trilogy, the film series is a quadrilogy (4 parts).
                    </p>
                    <p class="info__text">
                        On this site, you will find interest facts and tidbits
                        about the four films, The Hunger Games, The Hunger
                        Games: Catching Fire, The Hunger Games: Mockingjay -
                        Part 1, and The Hunger Games: Mockingjay - Part 2.
                    </p>
                    <p class="info__text">
                        Lorem ipsum dolor, sit amet consectetur adipisicing
                        elit. Explicabo dolore pariatur similique, facilis a
                        tempora placeat fuga amet maxime perspiciatis dolorem
                        vero vitae deserunt laudantium eaque. Accusantium earum
                        possimus numquam!
                    </p>
                    <p class="info__text">
                        Lorem, ipsum dolor sit amet consectetur adipisicing
                        elit. Minima numquam perferendis saepe quaerat non
                        maxime nesciunt cum tenetur voluptatibus. Fuga, quam
                        quaerat! Quisquam ea magnam nisi temporibus ex
                        voluptatibus rem? Lorem ipsum dolor sit amet consectetur
                        adipisicing elit. Sit temporibus perferendis eius quam,
                        dolor magni non dolore, veniam voluptatibus velit sint
                        nesciunt officia vitae quidem, ipsam iste libero ad et!
                    </p>
                </section>
            </div>
        </main>
        <footer class="footer">
            <p class="footer__text">
                <span id="year"></span>This website was created by Ayselah
                Smith, Jayce McHargue, Patrick Wright & Sophie Schnaper solely
                for educational purposes.
            </p>
        </footer>
        <script>
            document.getElementById("year").textContent =
                new Date().getFullYear;
            function myFunction() {
                var x = document.getElementById("nav__container");
                if (x.className === "nav__container") {
                    x.className += " responsive";
                } else {
                    x.className = "nav__container";
                }
            }
        </script>
    </body>
</html>



 <img class="movie-poster" src="hunger_games_poster_home.jpg" alt="Hunger Games Movie Poster">
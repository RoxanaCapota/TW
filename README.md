<!DOCTYPE html>
<html>
<head>
<title>Movie Time!</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="icon" href="cinema.png">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Karma">
<link rel="stylesheet" href="styles.css" />
<link rel="stylesheet" href="script.js" />
<style>
* {box-sizing: border-box}


body, html {
  height: 100%;
  margin: 0;
  font-family: Arial;
}

/* tab links */
.tablink {
  background-color: #555;
  color: black; /* color title */
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  font-size: 17px;
  width: 25%;
}

.tablink:hover {
  background-color: #777;
}


.tabcontent {
  color: black; /*text color */
  display: none;
  padding: 100px 20px;
  height: 100%;
}


h3 {
  text-align: center;
}
p {
  text-align: center;
}


#Home {background-color: lightpink;}
#Movies {background-color: mistyrose;}
#Series {background-color: seashell;}
#Cartoon {background-color: lavenderblush;}
</style>
</head>
<body>

<button class="tablink" onclick="openPage('Home', this, ' white')">Home</button>
<button class="tablink" onclick="openPage('Movies', this, 'white')" id="defaultOpen">Movies</button>
<button class="tablink" onclick="openPage('Series', this, 'white')">Series</button>
<button class="tablink" onclick="openPage('Cartoon', this, 'white')">Cartoon</button>

<div id="Home" class="tabcontent">
  <h3>MOVIES TIME!!</h3>
  <p>Hello! This page is to help those who are undecided on which movies or series to choose to watch. </p>
</div>

<div id="Movies" class="tabcontent">
  <h3>Movies</h3>
  <img src="dangerouslies.jpg" alt="" style="width:12%" class="center>
      <h3>Dangerous Lies</h3>
      <p>Thriller | 2020 | 1h 37min </p>
  <img src="rednotice.jpg" alt="" style="width:12%">
      <h3>Red Notice</h3>
      <p>Action and adventure, Comedy, Police movie | 2021 | 1h 57min </p>
  <img src="6underground.jpg" alt="" style="width:12%">
      <h3>6 Underground</h3>
      <p>Action and adventure | 2019 | 2h 8min </p>
  <img src="lovedrugs.jpg" alt="" style="width:12%">
      <h3>Love & Other Drugs</h3>
      <p>Comedy, Romance, Drama | 2010 | 1h 52min </p>
  <img src="intern.jpg" alt="" style="width:12%">
      <h3>The Intern</h3>
      <p>Comedy | 2015 | 2h 1min </p>
  <img src="tourist.jpg" alt="" style="width:12%">
      <h3>The Tourist</h3>
      <p>Mystery, Action and adventure, Police movie, Romance | 2010 | 1h 43min </p>
  <img src="murdermystery.jpg" alt="" style="width:12%">
      <h3>Murder Mystery</h3>
      <p>Mystery, Comedy | 2019 | 1h 37min </p>
  <img src="dirtygrandpa.jpg" alt="" style="width:12%">
      <h3>Dirty Grandpa</h3>
      <p>Comedy | 2016 | 1h 41min </p>
  <img src="badmoms.jpg" alt="" style="width:12%">
      <h3>Bad Moms</h3>
      <p>Comedy | 2016 | 1h 40min </p>
  <img src="badmoms2.jpg" alt="" style="width:12%">
      <h3>Bad Moms 2</h3>
      <p>Comedy | 2016 | 1h 40min </p>
    </div>


<div id="Series" class="tabcontent">
  <h3>Series</h3>
  <img src="gossipgirl.jpg" alt="" style="width:12%">
      <h3>Gossip Girl</h3>
      <p>Drama, Romance | 2007 | 6 seasons | 121 episodes</p>
  <img src="prettylittleliar.jpg" alt="" style="width:12%">
      <h3>Pretty Little Liars</h3>
      <p>Thriller, Mistery, Drama | 2010 | 7 seasons | 160 episodes</p>
  <img src="theoriginals.jpg" alt="" style="width:12%">
      <h3>The Originals</h3>
      <p>Drama, Action, Romance | 2013 | 5 seasons | 92 episodes</p>
  <img src="vampirediaries.jpg" alt="" style="width:12%">
      <h3>The Vampire Diaries</h3>
      <p>Drama, Action, Romance | 2009 | 8 seasons| 171 episodes</p>
  <img src="teenwolf.jpg" alt="" style="width:12%">
      <h3>Teen Wolf</h3>
      <p>Drama, Action, Romance | 2011 | 6 seasons | 100 episodes</p>
  <img src="beautyandbeast.jpg" alt="" style="width:12%">
      <h3>Beauty and the Beast</h3>
      <p>Drama, Action, Romance | 2012 | 4 seasons | 70 episodes</p>
  <img src="reign.jpg" alt="" style="width:12%">
      <h3>Reign</h3>
      <p>History Drama | 2013 | 4 seasons | 78 episodes</p>
  <img src="sexandthecity.jpg" alt="" style="width:12%">
      <h3>***** and the City</h3>
      <p>Comedy, Romance, Drama | 1998 | 6 seasons | 94 episodes</p>
  <img src="gilmoregirls.jpg" alt="" style="width:12%">
      <h3>Gilmore Girls</h3>
      <p>Comedy, Romance, Drama | 2000 | 7 seasons | 153 episodes</p>
  <img src="ggayearinthelife.jpg" alt="" style="width:12%">
      <h3>Gilmore Girls: A Year in the Life</h3>
      <p>Comedy, Romance, Drama | 2016 | 1 seasons | 4 episodes</p>
    </div>


<div id="Cartoon" class="tabcontent">
  <h3>Cartoon</h3>
  <p>SOON!! </p>
  
</div>

<script>
function openPage(pageName,elmnt,color) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].style.backgroundColor = "";
  }
  document.getElementById(pageName).style.display = "block";
  elmnt.style.backgroundColor = color;
}


document.getElementById("defaultOpen").click();
</script>
   
</body>
</html> 

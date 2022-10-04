# BlitzAudio Player 🎵

Hi! Thanks for checking out my **Audio Player**. 
If you need a simple audio player with modern UI for your web app, I got you!
No frameworks used, just good ol' HTML, CSS & vanilla JavaScript.
The component is part of the open source project webblocks2022 by ZTM, a library of HTML/CSS/JS components made for [Hackoctober 2022](https://hacktoberfest.com/).
The music used to showcase the component is by [me](https://www.blitzaudio.it/), hope you enjoy it!

![blitzaudio-player](https://i.ibb.co/ySQw6Yk/icon.jpg)

# Getting Started 🛠

If you want to test this component standalone, all you need to do is download the repo and open the index.html file in your favourite browser. 
If you want to integrate it in your web app, include this code inside the `<head>` tag of your index.html:

       <link rel="icon" type="image/x-icon" href="./assets/images/favicon.ico">
       <link rel="stylesheet" href="./styles.css"/>
       <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"/>


Include the audio tag at the top of the body:

    <audio src="" id="audio"></audio>

All the HTML code for the component is in the `<div  class="player">`
Don't forget to include the js files before closing the `<body>` tag and keep them in this order:

    <script  src="./data.js"></script>  
    <script  src="./app.js"></script>


## What you can do 📀

Press play and the first song of database will start playing. Press again to pause. 
Pressing skip next or skip previous will change song and autoplay it. 
The timebar will follow the progression of the current music playing, showing the remaining part of the song in a lighter color. If you want to skip to a different part of the song click anywhere on the timebar.
Under the timebar you can read current time of the song and total duration.

## Adding your own songs 🎶 

If you want to test the player with your own music, add your tracks in .mp3 format inside the directory ./assets/music and also include them in the data.js file. Just follow the model schema:

     { 
        id:  id_number, 
        songTitle:  "Song Title", 
        artist:  "Artist Name",
        source:  "./assets/music/file-name.mp3", 
        cover:  "source link for cover image", 
    },


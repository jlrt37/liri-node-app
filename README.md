Liri is a node.js command line application that takes in parameters and gives back data. 'Node liri.js' must be typed into the command line followed by a command and then a search parameter.

THe commands for Liri are: 
  'concert-this'
  'spotify-this-song'
  'movie-this'
  'do-what-it-says'.

'concert-this' uses the Bandsintown API to retrieve all upcoming concerts for an artist. Each venue name, location, and date is provided for all results. Moment.js is used to format the date from the Bandsintown API. (At this time, this command does not work. Still waiting on API key to come back.

'spotify-this-song' uses the Spotify API to retrieve data about the song entered. It removes 80% of results. All song titles that contain the search parameter or parts of it are returned. The user will receive the artist, song name, a link to preview the song, and the album name for each result.

'movie-this' uses the OMDb API to retreive data about the movie entered. The result will include the title, release year, IMDb rating, Rotten Tomatoes rating, country or countries it was filmed in, langauge(s), plot, and actors/actresses in the film.

'do-what-it-says' is a command that reads the random.txt file and executes the parameters inside of it. By default it is set to 'spotify-this-song,I Want It That Way'.

For this app to be successful, the following commands and installs may need to be performed:
  "npm init -y"
  "npm install dotenv"
  "npm install moment"
  "npm install node-spotify-api"

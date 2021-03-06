# LIRI-NODE-APP
LIRI is like iPhone's SIRI. However, while SIRI is a Speech Interpretation and Recognition Interface, LIRI is a _Language_ Interpretation and Recognition Interface. LIRI is a command line node app that takes in parameters and returns relevant data.

## HOW-T0:
* `CLONE` or `DOWNLOAD ZIP` of this repository to your local machine
* `UNZIP` the folder (if applicable) --> run your terminal/bash in the root of the folder
* `RUN` command `'npm install'` in your terminal/bash to install packages
* `WRITE` an `.env` file replacing the following with your unique spotify + twitter keys:

    ```
    # Spotify API keys

    SPOTIFY_ID=paste-here
    SPOTIFY_SECRET=paste-here

    # Twitter API keys

    TWITTER_CONSUMER_KEY=paste-here
    TWITTER_CONSUMER_SECRET=paste-here
    TWITTER_ACCESS_TOKEN_KEY=paste-here
    TWITTER_ACCESS_TOKEN_SECRET=paste-here

    ```
* `RUN` file `main.js` in your terminal/bash window ( `node main.js` )
* `LIRI` will then prompt four commands to choose from. Use `ARROW KEYS` and press `ENTER` to select one of the following:

##### (a) `'get-tweets'`

   * LIRI will prompt you to enter a twitter screen name.
   
     * LIRI will display the previous 20 tweets from that account as well as the timestamp for each.

   * If no screen name is provided, LIRI will default to `@AlYankovic` ...

##### (b) `'spotify-this-song'`

   * LIRI will prompt you to enter a song name.

   * LIRI will then display the following information about the song in your terminal/bash window

      ```
       * Artist(s)
       * The song's name
       * A preview link of the song from Spotify
       * The album that the song is from

      ```
      
   * If no song is provided then your program will default to `"Amish Paradise"`

##### (c) `'movie-this'`

   * LIRI will prompt you to enter a movie title.

   * LIRI will output the following information to your terminal/bash window:

     ```
       * Title of the movie.
       * Year the movie came out.
       * IMDB Rating of the movie.
       * Rotten Tomatoes Rating of the movie.
       * Country where the movie was produced.
       * Language of the movie.
       * Plot of the movie.
       * Actors in the movie.
     ```

  * If you do not provide a movie name, LIRI will default to `"Mr.Nobody"`

##### (d) `'do-what-it-says'`

* Using the `fs` Node package, LIRI will take the text inside of local file `random.txt` to call one of LIRI's commands according to the file content.


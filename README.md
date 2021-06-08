# Automate-Spotify-Playlist
SPOTIFY PLAYLIST

To create a new playlist function: 
- Got the user id and the OAuth token from spotify web api.
- Added them to another .py file called secrets and then used that to import other functions into the code
- Used python’s “request” library - that helps in making https request
-Spotify’s documentation tells us how to figure out how to create a playlist using Spotify. In the documentation, we were given information on the type of http method to use and the method in this case was a POST method

Search for the song: 
- How to search for a song using artist and track name using spotify web api
- Format query string to take in the song of the artist, send the information using the request library

Getting the liked videos:
- Using youtube data api documentation, 
- Has the code that we need to get the liked videos
- Limitations with this API: It would be hard to parse out the song’s/artist’s name where youtube’s DL library would come into the picture. We would be able to provide that library with a youtube url. This is going to give us song name and the artist stored in spotify_uri variable

Add this song into new Spotify Playlist:
- Which we append into a list giving us a list of songs
- Add songs into a new playlist using json.dumps(uris)
- Send over all of the uris to the specified endpoint
- Test with response.json()

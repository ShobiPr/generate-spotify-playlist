# generate-spotify-playlist

Generate a Spotify playlist based on videoes liked on Youtube. 

(Created based on tutorial: https://github.com/TheComeUpCode/SpotifyGeneratePlaylist)

## Build with
[Youtube Data API v3](https://developers.google.com/youtube/v3) - 

[Spotify Web Api](https://developer.spotify.com/documentation/web-api/) - 

[Youtube_dl](https://github.com/ytdl-org/youtube-dl/) - 

## Getting Started 

### Prerequisites
Install all dependencies 

```
pip3 install -r requirements.txt
```

### Tokens
Collect your Spotify User ID and Oauth Token from Spotify and add the configure credentials in [secrets.py](generate-spotify-playlist/secrets.py) 

* To Collect your User ID use your Spotify **username** 
* To Collect your Oauth Token, visit this [url](https://developer.spotify.com/console/post-playlists/) (using Chrome) and click the **Get Token** button. 

```
spotify_token = ""
spotify_user_id = ""
```

Enable Oauth for Youtube and download the client_secrets.json following this [guide](https://developers.google.com/youtube/v3/getting-started/).
```
{
	"installed":{
		"client_id":"",
		"project_id":"",
		"auth_uri":"",
		"token_uri":"",
		"auth_provider_x509_cert_url":"",
		"client_secret":"",
		"redirect_uris":["",""]
	}
}
```

## Running 
Run the file 

```
python3 create_playlist.py
```
* You will see ```Please visit this URL to authorize this application: <some long url```
* Click on the link and log into your Google Account to collect the authorization code


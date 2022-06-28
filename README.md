# youtube-upload
uploading video to youtube and put it into your playlist.


## instruction
1. Register your project with Google and get the OAuth2.0 credentials, then put your client_id & client_secret into `client_secrets.json` in this project.
2. Open your project's dashboard, search `youtube data api v3` in the library and just enable it.
3. `pip3 install google-api-python-client oauth2client`
4. upload via command line
   ```shell
   python3 youtube-upload.py --file="/tmp/test_video_file.flv" 
                            --title="Summer vacation in California"
                            --description="Had fun surfing in Santa Cruz"
                            --keywords="surfing,Santa Cruz"
                            --category="22"
                            --privacyStatus="private"
                            --playlist="your playlist id"
   ```
   
## reference
- https://developers.google.com/youtube/v3/guides/uploading_a_video
- https://developers.google.com/youtube/v3/docs/playlistItems/insert

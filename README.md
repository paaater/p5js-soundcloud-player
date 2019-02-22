# p5js-soundcloud-player

#### Example

https://joepdooper.github.io/p5js-soundcloud-player

## Built With

[P5.js](https://p5js.org/reference/#/libraries/p5.sound) - p5.sound extends p5 with Web Audio functionality including audio input, playback, analysis and synthesis.
[SoundCloud API](https://developers.soundcloud.com/docs/api/guide) - Using the SoundCloud API, you can build applications that take sound on the web to the next level.

## How it works

### user/tracks
```javascript
var PLAYLIST_URL = 'https://soundcloud.com/user/tracks';
```
```javascript
for(var i=0;i<playlist.length;i++) {
  urlList.push(playlist[i].stream_url + '?client_id=' + CLIENT_ID);
  nameList.push(playlist[i].title);
}
```

### user/sets
```javascript
var PLAYLIST_URL = 'https://soundcloud.com/user/sets/classics';
```
```javascript
for(var i=0;i<playlist.tracks.length;i++) {
  urlList.push(playlist.tracks[i].stream_url + '?client_id=' + CLIENT_ID);
  nameList.push(playlist.tracks[i].title);
}
```
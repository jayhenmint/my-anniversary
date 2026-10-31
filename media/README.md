# Your anniversary media

Place your audio and video files in this folder, beside this README:

| Choice | Exact filename | Path from index.html |
| --- | --- | --- |
| Hear me sing | sing.mp3 | media/sing.mp3 |
| A voice message | voice-message.mp3 | media/voice-message.mp3 |
| Surprise me | surprise.mp4 | media/surprise.mp4 |

Project layout:

```text
my-anniversary/
  index.html
  media/
    README.md
    sing.mp3
    voice-message.mp3
    surprise.mp4
    game/
      photo-1.jpg
      photo-2.jpg
      photo-3.jpg
      photo-4.jpg
```

Use actual MP3 audio files. Export the video as MP4 with H.264 video and AAC audio for broad mobile compatibility. Renaming an extension does not convert a recording.

If your audio uses M4A instead, add the actual M4A files here and update the AUDIO paths near the top of the script in index.html. The SURPRISE_VIDEO setting contains the video path.

Match filename spelling and capitalization exactly. Files are not included yet; add your own. Keep this media folder next to index.html when copying or hosting the website, including a photo-personalized HTML export. Upload the files to GitHub in media/ when you are ready.

The visitor presses Play; audio/video does not autoplay. Closing the popup stops playback. The Letter option remains separate; Surprise me always opens your video.

## Photo matching game

Add four different pictures to the game/ subfolder, with these exact names:

| Photo | Path from index.html |
| --- | --- |
| 1 | media/game/photo-1.jpg |
| 2 | media/game/photo-2.jpg |
| 3 | media/game/photo-3.jpg |
| 4 | media/game/photo-4.jpg |

Each photo automatically appears on two shuffled cards. Match all four pairs to continue. Until photos are added, numbered cards keep the game playable. The game has no photo-upload control.

Use actual JPG files; renaming PNG or HEIC files to .jpg does not convert them. Square images work best; other shapes crop to fill the cards. For PNG/WebP files, change the corresponding GAME_PHOTOS paths in index.html. Keep images reasonably small for quick phone loading (around 800 x 800 pixels is plenty).

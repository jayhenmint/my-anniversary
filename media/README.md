# Your anniversary media

Place these three files in this folder, beside this README:

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
```

Use actual MP3 audio files. Export the video as MP4 with H.264 video and AAC audio for broad mobile compatibility. Renaming an extension does not convert a recording.

If your audio uses M4A instead, add the actual M4A files here and update the AUDIO paths near the top of the script in index.html. The SURPRISE_VIDEO setting contains the video path.

Match filename spelling and capitalization exactly. Files are not included yet; add your own. Keep this media folder next to index.html when copying or hosting the website, including a photo-personalized HTML export. Upload the files to GitHub in media/ when you are ready.

The visitor presses Play; audio/video does not autoplay. Closing the popup stops playback. The Letter option remains separate; Surprise me always opens your video.

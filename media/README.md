# Your anniversary media

Place your audio and video files in this folder, beside this README:

| Choice | Exact filename | Path from index.html |
| --- | --- | --- |
| Yes, sing for me | sing.mp3 | media/sing.mp3 |
| Recorded message inside the envelope | voice-message.mp3 | media/voice-message.mp3 |
| Final surprise video | surprise.mp4 | media/surprise.mp4 |

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
      jigsaw.jpg
```

Use actual MP3 audio files. Export the video as MP4 with H.264 video and AAC audio for broad mobile compatibility. Renaming an extension does not convert a recording.

If your audio uses M4A instead, add the actual M4A files here and update the AUDIO paths near the top of the script in index.html. The SURPRISE_VIDEO setting contains the video path.

Match filename spelling and capitalization exactly. Files are not included yet; add your own. Keep this media folder next to index.html when copying or hosting the website, including a photo-personalized HTML export. Upload the files to GitHub in media/ when you are ready.

The final question asks whether she wants to hear you sing. Yes starts sing.mp3 from that tap; No goes straight to the envelope. The envelope shows your LETTER text and has an optional Play my message button for voice-message.mp3. After opening the envelope, Open your surprise shows surprise.mp4. The song ending automatically opens the envelope; the video ending automatically shows the final plan. Each media panel also has a continue button. Leaving a panel stops playback.

## One-photo jigsaw game

Add one whole photo at: **media/game/jigsaw.jpg**.

No manual cutting is needed. The page divides it into four pieces automatically. Tap two pieces to swap them and rebuild the photo. The whole original photo is preserved; rectangular pictures get some padding inside the square puzzle.

Use an actual JPEG image, ideally around 1200 pixels on its longest side for quick phone loading. For a PNG or WebP, change JIGSAW_IMAGE near the top of the script in index.html to match the actual filename. Renaming a file extension does not convert an image.

The game includes a full-photo preview and optional number hints. Until the photo is added, the numbered puzzle stays playable. The old photo-1.jpg through photo-4.jpg files are no longer used; existing files have been left alone.

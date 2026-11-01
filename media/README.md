# Anniversary website

Live site: https://my-anniversary-inky.vercel.app

## Current experience

On every load or reload, a flying paper airplane carries a little letter. Tap it to reveal “Hi Lean, you have an invitation.” Then **slide the mail to the heart** to start the birthday questions. A partial slide returns to the start; tapping alone does not proceed. Keyboard users can use the arrow keys or End. Shared links and exported copies also start with the airplane.

1. “Unlock me — Guess my birth month”: guess the birthday month from four pictures. Feedback appears in a centered puppy-sticker popup. Wrong choices have Try Again. April/summer is correct; its success popup continues to the PIN after a short pause or with the Continue button.
2. Enter birthday passcode **15** using the phone-style 0–9 keypad. Two masked digits submit automatically. Only **15** unlocks the invitation; every wrong code stays locked and shows a retry popup with a descending sound. A correct code gets a success popup and chime. Clear, delete and physical keyboard entry work; wrong answers can retry.
3. The correct passcode proceeds directly to the first question, skipping the old “Hey, love” welcome. The first question shows three drink pictures and a person sticker. Drag a drink up to the person to give it; alternatively select a drink, then tap the person. Coffee is the only correct answer: the recipient and popup show a happy face. Other drinks show a sad face and allow retries.
4. Choose food and a place, solve the **six-piece jigsaw**, then choose a gift. Solving it shows a congratulations popup with the completed photo and advances automatically after three seconds; no Continue button is needed.
5. The centered song player appears. Play/Pause and the progress slider work; seeking to the end continues immediately.
6. Rate the song with one of four emojis. Each emoji gets a different reply.
7. Collect the three heart emojis in a simple nine-tile game to unlock the envelope. Bigg’s is no longer part of the game.
8. Open the envelope to read the original letter, ending with “Happy Anniversary, Be! ♡”. It has no voice-message player.
9. Answer the video-opening question by tapping **Yes, open & play it**. The video cannot advance before real playback finishes.
10. A message says “I hope you liked my simple video for you.” Continue to the final invitation question.
11. Yes/No gets the appropriate happy/sad response and opens the final plan with Save and Share buttons.

Question choices and buttons have gentle synthesized click sounds. Jigsaw pieces use tile/swap sounds, with a short chime on completion. Sounds start only after interaction and require no additional media files; device volume controls their loudness.

## Files to provide

Keep these paths and filename capitalization exactly as shown:

```text
my-anniversary/
  index.html
  media/
    sing.mp3
    surprise.mp4
    game/
      jigsaw.jpg
```

- **Song:** media/sing.mp3
- **Surprise video:** media/surprise.mp4
- **Whole jigsaw photo:** media/game/jigsaw.jpg — no manual cutting; the page makes 2 columns × 3 rows.

Use real MP3/MP4/JPG formats; changing a filename extension does not convert a file. Portrait and landscape jigsaw photos are preserved with padding when needed. Change AUDIO, SURPRISE_VIDEO or JIGSAW_IMAGE in index.html if your actual filenames differ.

The previous voice-message.mp3 is no longer used by the envelope. The former four separate matching-game images are also unused.

## Saving the final picture in Chrome

**Save details image** starts a direct PNG download named **our-anniversary-plan.png** and reveals the full-size picture.

- In Chrome, open the menu → Downloads and look for that filename.
- On Android, also check Files → Downloads. It may not appear automatically in Gallery/Photos.
- On iPhone, choose Save to Files if Chrome prompts for a destination.
- The visible **Download PNG** link is a second direct download action.
- You can press and hold the full-size picture and choose Download/Save Image.
- **Phone save/share menu** is a separate option shown when native image-file sharing is supported.

Official Chrome help:
- Android: https://support.google.com/chrome/answer/95759?co=GENIE.Platform%3DAndroid
- iPhone/iPad: https://support.google.com/chrome/answer/95759?co=GENIE.Platform%3DiOS

**Share plan image** uses the phone’s native sharing menu where supported. Choose Messenger if offered, or save the PNG and attach it manually. The site does not send messages automatically.

Only food, destination, gift, date/time placeholder and invitation response appear in the shared picture. Birthday, coffee guess, song rating and game answers are excluded. A legitimate Coffee & sweets food selection remains. The shared date reads “September • 💙💙💙💙💙 • 2026”, using blue hearts as the day hint rather than a written day number. The time is still To be arranged together. The blue hearts are a subtle hint, not private encryption.

## Video optimization and backups

The current video is **6,256,854 bytes**, reduced from 54,726,235 bytes (88.6% smaller). The CapCut ending screen has been removed; it now ends on the photo at **57.2 seconds**, with a short audio fade-out. It uses H.264 at 540 × 960, AAC audio and fast-start MP4 metadata.

The original is saved locally in **.video-backups/surprise-original.mp4**. The backup folder is excluded from Git and Vercel uploads.

## Personalization

Edit LETTER in index.html to change the letter text. SONG_RATINGS contains each emoji and its reply. Birthday month illustrations, drinks and puppy stickers are embedded SVGs and need no external picture files.

The collage’s photo controls can embed selected pictures in a saved HTML copy. Keep the media folder beside that copy so the linked song, video and jigsaw can load.

## Drink delivery interaction

The first question uses Pointer Events for actual touch/mouse dragging. The person highlights when a drink is over the drop area. Dropping elsewhere returns the drink without answering. Tap-to-select then tap-the-person, and native keyboard button activation, provide alternatives to dragging. Delivery is animated before the feedback appears. All drink and person illustrations are embedded SVGs; no extra assets are required.

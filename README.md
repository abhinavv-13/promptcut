# PromptCut

Motion graphics prompt templates for Claude. Pick a visual style, add your topic or voiceover, paste the prompt into Claude, and get an animated explainer with synced sound effects, written entirely in code.

**Live:** https://abhinavv-13.github.io/promptcut/

## What it is

Each style in the library is a complete animation prompt. You choose a look, give Claude a topic or a transcript, and it builds the video as an interactive artifact. The sound effects (clicks, pops, risers) are synthesized in the browser with Web Audio, so there are no licensing issues.

Before building anything, Claude writes a storyboard of every screen and waits for your OK. Changing the words and scenes at that stage is much faster than editing code later.

## What's in the site

- **Style Library:** sample animations you can watch, each with a copyable prompt. New styles are added regularly.
- **Clone a style:** attach 1 to 3 screenshots of a look you like and Claude rebuilds it as a new animated style.
- **Guide:** a walkthrough of the full workflow, from text to video, voiceover sync, style cloning and monetization.

## How to use it

### Text to video

1. Pick a style, for example Creator Motion Graphics or Clean Tech.
2. Enter your topic.
3. Copy the prompt and paste it into Claude.
4. Review the storyboard and ask for changes if needed.
5. Reply `OK` to render the animation.

For Shorts or Reels, ask for vertical 9:16 (1080x1920). The artifact window defaults to landscape.

### Voiceover sync

1. Ask Claude to transcribe your video or audio with word-level timestamps.
2. Pick a style, switch to **With Voiceover**, and paste the transcript.
3. Copy the prompt into Claude. Text and sound effects land on the exact word.

### Clone a style

1. Pick the closest starting style.
2. Copy the clone prompt into a new Claude chat.
3. Attach your screenshots and send.

Claude explains how the animation engine works, shows a test frame in your style, and builds the full video only after you approve.

## Recording the output

Play the artifact in Claude with sound on, record the browser window in OBS at 60 fps, then edit in Premiere or CapCut.

## Run locally

```bash
git clone https://github.com/abhinavv-13/promptcut.git
cd promptcut
<command to serve the site, e.g. npx serve .>
```

## Project structure

```
promptcut/
├── assets/     # logo and shared images
├── styles/     # one folder per style (poster, preview, prompt)
└── index.html
```

## License

The style prompts are free to use for your own videos.
Code is released under the [MIT License](LICENSE).

## Author

[Abhinav](https://github.com/abhinavv-13)

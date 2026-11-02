# reel-studio

A Claude Code skill file (`SKILL.md`) that describes one workflow for five kinds of short-form reel: interview clips, talking-head from a script, TTS voiceover, kinetic quote cards and motion-graphics explainers. It is the written playbook SkynetLabs uses with Claude Code, shared as-is.

## What the skill covers

- **interview** - long video into 9:16 shorts (pick the best moments).
- **saddamh1** - talking-head reel from a script, Hinglish/Urdu business-advice style (the default).
- **tts** - voiceover-only reel.
- **kinetic-stoic** - text-only quote reel.
- **mograph** - motion-graphics explainer with UI chips, no face cam.
- Locked defaults for title cards, B-roll card timing and contrast, caption style (Montserrat Bold, lower third), voice EQ, music ducking and loudness (-14 LUFS for Reels/TikTok/Shorts).

Stack named in the skill: FFmpeg, Python, Whisper, pyannote. Local-first, no paid editor.

## How to use it

```bash
git clone https://github.com/waseemnasir2k26/reel-studio.git ~/.claude/skills/reel-studio
```

Then in Claude Code ask for "a reel for ..." or run `/reel-studio`. The trigger phrases are listed in the `description` line at the top of `SKILL.md`.

## For you if

You use Claude Code and want a worked example of a long, opinionated video skill: what to lock, what to log, how to write down QA rules so they survive between sessions.

## Status and limits

- This repo holds `SKILL.md` only. The scripts and reference files it points to (`pipeline/`, `references/SADDAMH1-MASTER-PLAYBOOK.md`) and the `interview-clip-engine` project folder are not included, so the skill cannot run end to end from this repo alone.
- Paths in the file are Windows paths from the author's machine. Change them to yours.
- Tested by the author on Windows with an RTX 4060. Nothing here is verified on other setups.

## License

MIT, see [LICENSE](LICENSE).

---

Built by SkynetLabs. Contact: waseem@skynetjoe.com

Need this wired into your business? SkynetLabs builds voice agents, n8n back offices and sites that convert → https://skynetjoe.com

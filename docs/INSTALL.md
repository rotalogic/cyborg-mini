# Install / Activate CYBORG Mini

CYBORG Mini is plain Markdown — there is nothing to compile and no dependency to install. You activate it by giving its instructions to an AI. Pick the route that matches your AI:

> License reminder: CYBORG Mini is proprietary (see `../LICENSE`). Personal, non-commercial use with attribution intact is allowed; redistribution and commercial use need written permission from Hasyim Hasyimi / RotaLogic.

## 1. Any AI chat (fastest, no install)
Works with ChatGPT, Claude, Gemini, and other chat AIs.
1. Open `MASTER-PROMPT.md` in this repo.
2. Copy the entire text block.
3. Paste it as the **first message** in a new chat.
4. The AI replies with an activation confirmation, then waits for your first task.
CYBORG stays active for that chat session only.

## 2. As a permanent skill (assistants that load SKILL.md)
1. Download this repo for your own use.
2. Copy this folder into the skills folder your assistant reads from.
3. Start a new session — the assistant can now invoke CYBORG Mini by name.
4. Copy `state-template.md` to `cyborg-state.md` in your own workspace (not in this repo, and never committed — see `.gitignore`).

## 3. As full instructions / system prompt
Paste the entire contents of `SKILL.md` where your tool accepts custom instructions, a system prompt, or project instructions. `SKILL.md` is self-contained and needs no other file to work, except your own `cyborg-state.md` if you want persistent state.

## 4. ChatGPT — Custom GPT or Project (personal use)
- Custom GPT: paste the Master Prompt block into the GPT's Instructions field, for your own use.
- Project: add `SKILL.md` as a project file / paste it into Project instructions.
Test with: "focus today" — CYBORG should ask for / create your state instead of inventing goals.

## 5. Gemini — Gem (personal use)
Create a Gem and paste the Master Prompt block as its instructions. Test with the same check as above.

## Verify your copy
`CREDENTIAL.md` lists the SHA-256 of the official `SKILL.md` for this release.
Run `sha256sum SKILL.md` (macOS: `shasum -a 256 SKILL.md`) and compare — a match means the core file is unmodified from the release.

## Privacy rule
Your `cyborg-state.md` contains your goals, inbox, habits, and reflections. Keep it in your own private workspace. Do not publish it, do not commit it to a public repo, and do not paste it into chats you do not trust.

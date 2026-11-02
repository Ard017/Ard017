# CLAUDE.md

## What this repo is

`Ard017/Ard017` is a **GitHub profile repository**. GitHub shows `README.md` on
the profile page at https://github.com/Ard017. There's no application code.

Files:
- `README.md`: the profile page (Markdown mixed with inline HTML for images and badges).
- `SECURITY.md`: GitHub's default security-policy template, not yet filled in.

## Build / test / lint

There's **no build, no test suite, no package manager, and no CI**. Don't look
for `npm`, `pip` or `make` commands. To check a change:
- Read the rendered Markdown (GitHub preview or any CommonMark renderer).
- Check that every image and link URL resolves (`curl -sI <url>` and look for a 200).

## Style for README.md

- Keep the existing layout: greeting header, banner image, personal quote,
  skills line, emoji bullet list, then a row of social icons and a row of badges.
- Write images and links as inline HTML (`<img src='…' height='40'>`,
  `<a href='…'>`) to match what's already there. Use single quotes in the HTML attributes, as the file does.
- Icons come from `cdn.jsdelivr.net/npm/simple-icons@3.0.1`, with a fixed version. Keep that
  version unless asked to change it.
- Emoji bullets use the `- 🔭 …` / `- 🌱 …` pattern.
- Don't rewrite the personal text (the quote, the skills, what the owner is learning) unless
  asked. It's the owner's own voice.

## Known issues (fix only when asked)

- The social links are doubled: `https://github.com/https://github.com/Ard017`
  and `https://twitter.com/https://x.com/A__rO07`. They should be
  `https://github.com/Ard017` and `https://x.com/A__rO07`.
- `SECURITY.md` still has the template's placeholder text and version table.

## Git workflow

- Keep commits small, with descriptive messages (for example, "Fix social links in README").
- Work on the branch you're given. Don't push to `main` unless the owner asks.

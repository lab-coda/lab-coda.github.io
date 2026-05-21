# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Claude should only be used to debug code, check typos and never directly edit the code. 

For files under `content/` and `hugo.toml`, editing typos is permitted but do not generate text.

## Local development

```bash
hugo server --renderStaticToDisk
```

Do **not** use plain `hugo server` — static files (including CSS) may not sync on startup, causing styles to appear broken. The `--renderStaticToDisk` flag avoids this Hugo quirk.

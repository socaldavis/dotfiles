# dotfiles

My personal dotfiles. Small, deliberate, and portable — the config I drop onto a new machine so it
feels like home in a minute. From [Chris Davis / PC-Addicts](https://www.youtube.com/@PC-Addicts).

## What's here

| File | What it configures |
|---|---|
| `.vimrc` | A minimal, no-nonsense Vim setup — sensible defaults, [gruvbox](https://github.com/morhetz/gruvbox) theme, and a fast `jj` → `Esc` escape. |

More to come (bash, git, etc.) as I get around to cleaning them up for sharing.

## The `.vimrc`, in short

- **Line numbers** — absolute + relative (`number` / `relativenumber`) for quick motions.
- **4-space indent** — `expandtab`, `tabstop`/`shiftwidth` = 4, `smartindent`.
- **`jj` to escape** — tap `jj` in insert mode instead of reaching for `Esc`.
- **Quality-of-life** — `incsearch`, `scrolloff=8`, `colorcolumn=120`, `nowrap`, no error bells.
- **Plugin manager** — [vim-plug](https://github.com/junegunn/vim-plug), auto-installed on first launch.
- **Theme** — gruvbox (hard dark contrast).

## Install

The `.vimrc` bootstraps its own plugin manager, so setup is just two steps:

```bash
# 1. Back up any existing config, then drop this one in:
cp .vimrc ~/.vimrc

# 2. Open Vim — vim-plug installs itself and pulls the theme on first run:
vim
```

That's it. On first launch Vim fetches vim-plug and runs `:PlugInstall` automatically.

## Make it yours

These are *my* preferences, not gospel — fork it, keep what you like, change the rest. The `colorcolumn`,
the `jj` mapping, and the theme are the usual first things people tweak.

## License

[MIT](LICENSE) — copy, modify, and use freely.

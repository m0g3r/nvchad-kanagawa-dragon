# nvchad-kanagawa-dragon

Kanagawa Dragon for NvChad.

NvChad's built-in kanagawa is the Wave variant. Newer base46 has a kanagawa-dragon port, but it goes through base16 colors, so code doesn't look like kanagawa.nvim's Dragon and the text is dimmer. Here the code colors are copied from kanagawa.nvim's Dragon highlight groups, so files look the way they do with kanagawa.nvim, and the background and text match terminal themes made from Dragon (Ghostty's "Kanagawa Dragon", for one).

## Install

Copy `lua/themes/kanagawa_dragon.lua` into `~/.config/nvim/lua/themes/`, then set it in `lua/chadrc.lua`:

```lua
M.ui = { theme = "kanagawa_dragon" }      -- NvChad v2.5
M.base46 = { theme = "kanagawa_dragon" }  -- NvChad v3.0
```

Restart nvim. It's also in the theme picker (`<leader>th`).

Tested with NvChad v2.5. v3.0 loads custom themes the same way, but I haven't tried it there.

## Changed from kanagawa.nvim

- No separate background behind line numbers and git signs.
- Selected text is dark grey (#393836) instead of navy.
- Folders in nvim-tree are violet (#957fb8).
- The statusline, tabs, file tree and menus are NvChad's, colored like base46's kanagawa-dragon port.

## Credits

Colors from [kanagawa.nvim](https://github.com/rebelot/kanagawa.nvim) by rebelot (Copyright (c) 2021 Tommaso Laurenzi, MIT). NvChad UI colors from the kanagawa-dragon theme in [base46](https://github.com/NvChad/base46) (Copyright (c) 2019 Ashkan Kiani, MIT).

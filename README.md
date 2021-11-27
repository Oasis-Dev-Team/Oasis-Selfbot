# Oasis Themes

This will be a short explanation on Oasis Themes

Oasis uses `.toml` for its Themes

There are three types of Themes

- Single Color
- Multi Color
- Gradient

---

You can specify Colors in 2 ways

- `rgb(255,255,255)` as RGB
- `#FFFFFF` as HEX

---

1. `Single Color Themes`

```toml
Type = "Single"
[Colors]
Color = ""
Background = ""
```

---

2. `Multi Color Themes`

```toml
Type = "Multi"
[Colors]
First = ""
Second = ""
Third = ""
Fourth = ""
Fifth = ""
Background = ""
```

---

3. `Gradient Color Themes`

```toml
Type = "Gradient"
[Colors]
First = ""
Last = ""
Background = ""
```

---
How to implement the new custom theme:

- Create a `.toml` (for example `MySuperCoolTheme.toml`) file in your Themes folder and copy an example from this tutorial.
- Replace the color codes with your own.
- Enter the theme file's name in your `config.toml` file and don't forget to restart the Selfbot.

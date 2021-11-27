# Oasis Themes

---

This will be a short explanation on Oasis Themes

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
Color = "#FFFFFF"
Background = "#5F5F5F"
```

---

2. `Multi Color Themes`

```toml
Type = "Multi"
[Colors]
First = "rgb(245, 245, 187)"
Second = "rgb(245, 187, 187)"
Third = "#474747"
Fourth = "rgb(245, 245, 245)"
Fifth = "rgb(245, 245, 187)"
Background = "#5F5F5F"
```

---

3. `Gradient Color Themes`

```toml
Type = "Gradient"
[Colors]
First = "#505050"
Last = "#202020"
Background = "#FFFFFF"
```

---

Now replace the examples with the colors you want and put it in your themes folder.
Fill in the name of the file in the config and restart the Selfbot.

# Colour roles
## Roles (light theme)

| Role | Job | Hex |
|---|---|---|
| surface | Page background | F7F9FF |
| on-surface | Text on the page | 181C20 |
| primary | Main buttons, links | 30628C |
| on-primary | Text on main buttons | FFFFFF |
| primary-container | Soft highlight boxes | CEE5FF |
| on-primary-container | Text on those boxes | 104A73 |
| outline | Borders | 727774 |

## Contrast ratios (WebAIM)

| Pair | Ratio |
|---|---|
| on-surface on surface | 16.27:1 |
| on-primary on primary | 6.45:1 |
| on-primary-container on primary-container | 7.23:1 |
| primary on surface | 6.13:1 |
| outline on surface | 4.33:1 (borders only, not text) |

## Error roles (light theme)

| Role | Job | Hex |
|---|---|---|
| error | Error messages, error borders | BA1A1A |
| on-error | Text on an error-coloured background | FFFFFF |

## Contrast checks for error (WebAIM)

| Pair | Foreground | Background | Ratio |
|---|---|---|---|
| on-error on error | FFFFFF | BA1A1A | 6.46:1 |
| error on surface | BA1A1A | F7F9FF | 6.13:1 |

Both pairs pass the 4.5:1 bar for normal text. Neither reaches 7:1, so neither meets AAA.

Error is never shown by colour alone. Every error will have a caution icon beside it.


## Known issue
No tone in my ref primary list matches the primary role (30628C), so
the roles are separate hex values and not references to the palette.

Success: I chose a dark, muted green (316941) because it is easy on the
eyes on a phone screen. It gets 6.18:1 on the surface, which passes the
4.5:1 bar for normal text. The cost is that it is less eye-catching than
a bright green, so every success message will also carry an icon.

Warning: I chose a dark amber (855317) because I wanted my colour choices
to be inclusive, and not rely on a conventional bright amber. It gets
6.14:1 on the surface, which passes. A bright amber (F5A623) got [1.92:1]:1 in my own test, which fails. The cost is that a dark amber can
look brown, so it may not read as a warning on its own, which is why every
warning will also carry an icon.
## Tones


My primary palette has 18 tones, from 0 (black) to 100 (white). The
Material Theme Builder plugin generated them from my source colour.

This is enough for both light and dark themes because both use the same
strip but pick different tones. In a light theme, buttons use tone 40
and the text on them uses tone 100. In a dark theme, buttons use tone 80
and the text on them uses tone 20. The light tones make the dark ones
stand out, and the other way round.

I did not add more tones because there are already fine steps near white
and black (99, 98, 95 and 5, 10, 15), which is where backgrounds and
cards sit.

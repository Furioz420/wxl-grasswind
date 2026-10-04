# Grass Wind

In the stock client, grass just sits there. It doesn't react to wind, to you walking through it,
nothing. This module gives it a bit of life.

- It sways gently, like it's actually caught in the wind: two overlapping waves so it doesn't look like
  a single flat ripple.
- It parts around you as you walk through it, and settles back once you've passed.

That's it. No new textures, no new models, just motion on the grass that's already there.

## How it's done

Everything runs on the GPU, on the grass's own vertex shader, so there's no extra draw call and no
noticeable performance cost. It only touches how each blade bends: the base stays planted, the tip
moves the most, exactly like a real blade of grass would.

## Tunable

Wind direction and strength, sway speed, how far grass parts around you and how strongly, all
adjustable. Purely cosmetic either way: turning it off just leaves the client's grass static, like
before.

## Requirements

WarcraftXL on a 3.3.5a client, build **12340**.

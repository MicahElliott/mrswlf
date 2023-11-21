# Mrs. Wolf

Mrs. Wolf is a spinoff keybard layout derived from Colemak-DH, taking
learnings from more modern layouts to improve comfort: much less stretching,
fewer redirects, better SFBs, etc.

## Goals

- Learnable from Colemak-DH in a couple days (except `o`), by minimizing home
  row changes (and other high-freqs)
- Drastically decrease lateral stretching (eg, `m` shouldn't be on right hand)
- Reduce redirects
- Alt-finger/pivot workarounds possible for _every_ (D)SFB
- Progressive intermediate-step layout(s)

It's easy to learn if you've been stuck in Colemak land and struggling to work
your way out: only ~4 high-impact keys have changed significantly (10 total),
and most feel intuitive: **l o m a**. The home row has all the same keys and
only **m** and **a** have changed (capitalized significant changes).

```
w L f p J     B u y '
M r s t g   k n e i A
V x c d Q   Z h , . /
        o
```

- Sfb:  0.751%
- Dsfb: 4.988%
- Lsb:  0.504%
- BadRedirects: 0.142%

A few locations are still suboptimal: `p`, `c`, `n` all cause a lot of
theoretical SFBs, but it's a very good compromise for maintaning the Colemak
feel. In fact, I consider SFBs to be 0% if you're willing to learn to
alt-finger stacks like `sc`, `pt`, etc; Mrs. Wolf was designed to make them
all reasonable. And the LSBs are mostly from `k`, and
kinda negligible given an easy hand-shift for `kn`/`nk`.

Here's what's the same as Colemak-DH (if you squint at `w` and `k` a little):

```
w   f p         u y '
  r s t g   k n e i
  x c d       h , . /
```

As you can see, the whole Colemak-DH core is untouched (ignoring pinkies)!

## Intermediate Transitional (and other options)

> Time: couple days or weeks

To get started, here's an intermediate training layout where only 3 keys have
changed! `m`, `a`, `o` (thumb).

```
q w f p b   j l u y '
M r s t g     n e i A
z x c d v   k h , . /
        O
```

You won't believe this, but you can stop here and call it good if you like.
The stats are already getting shiny and significantly better than Colemak-DH
(all stats are from [Oxey's Layout Playground][3] analyzer).

- Sfb:  0.979%
- Dsfb: 6.973%
- Lsb:  0.618%
- BadRedirects: 0.142%

Colemak-DH in comparison:

- Sfb:  1.083%
- Dsfb: 8.259%
- Lsb:  1.923%
- BadRedirects: 1.466%

You could even start with only moving `o` to thumb (wait on `m` and `a`),
before doing the `m`/`a`/`o` swaps. Try just `o` for a week and see if you can
get past the hatred.

Honestly, the simplest possible winning Colemak-DH mod (if you feel lateral
stretch pain) I can come up with is to simply swap `m` and `z` (though the
`qam` stack is pretty nasty):

- Sfb:  1.682%
- Dsfb: 6.389%
- Lsb:  0.678% <=== THIS IS GOOD!!
- BadRedirects: 1.525%

Oooor, just move `m` to thumb and you're done.

- Sfb:  0.845% <=== WOW!
- Dsfb: 6.140%
- Lsb:  0.678%
- BadRedirects: 1.525%

Fun fact: `m` is the [first letter][2] of a lot of words, and I think that
makes it a pretty good thumb letter.

## About the big (and small) moves

- `a` — OK, it's annoying to use right-hand for `Ctrl-a` (select-all). But
  otherwise, this was a surprisingly easy move for my hands, and really is
  what gets you to having the important vowel (and consonant) hand(s) (common
  to most modern layouts).

- `w` — Barely notice the change.

- `m` — Also surpringly fast adjustment. You'll have to get used to having
  this on left for many layouts anyway.

- `l` — It has to go somewhere comfy, and this is a common stack, above `r`.

- `o` — Very challenging being on thumb. Wonder if it's worth trying only this
  move independently for a week to see if it's workable for you. Other layouts
  put `e` and `t` on thumb to great success, so we know it's possible. Just
  takes a lot of focus on learning. I recommend omitting it from your typing
  trainer while learning the other changes. The reason `o` has nowhere
  "normal" to go it because we take it as a given that we're stuck with `n` on
  right-index. `o` can't stay on right-pinky because of the awful `you`
  redirect. `o` can't go above or below `e` because `one` would be even worse
  than `you`.

- `b` — Kinda hard adjustment, but feels amazing. On this layout: if you feel
  yourself stretching, you're probably reaching far the wrong key.

- `k` — Optional, but easy change and really can help the lateral stretching,
  depending on your keyboard. The most common combos `kn`/`nk` (not really a
  stretch since you shift your hand) and `ck` (often ends in `k`) are
  negligible effort.

- `v` — Happy uncommon experiment that saved a ton of stretching and feels
  very natural.

- `j`/`z`/`q`/`x` — Doesn't matter much where you put them. Move them around
  to your taste, but keep `q` on the left.

## Optional Moves

Most of the low-freq moves aren't super important, statistically. You can keep
the `k` where it was -- but it's better on my keyboard on middle-row. I did find
that moving `v` was a really good lateral win. `q` just feels better on the left-hand
to me since always combined with `u`-vowel.

## Compelling Features

The scores aren't perfect, but they're better than they first appear. The SFUs
are largely alt-able in easy ways. It inherits some quirks froz Colemak, but
you're used to them.

Mrs. T's key selling point is its "lateral stretch" score of `0.772%`. This is
what happens when you remove that nasty `m` from the right hand.

## Graduation Path

When you're ready for more moves, these will get you closer to the big boys,
and can be attempted one at a time:

- Swap `m` and `n`.
- Swap `k` and `,`.
- Swap `v` and `q`.

## Reference Implementation

Probably not useful, but at least the picture gives some context for one
attempt at easier alt-fingering, using QMK:
[anatak60][4](`mrswlf` branch).

## Versian without thumb-`o`:

```
w l f p b   j y o u '
m r s t g   k n e i a
v x c d q   z h , . /
```

- Sfb:  1.098%
- Dsfb: 7.431%
- Lsb:  0.735%
- BadRedirects: 0.108%

The main challenges with this are:

- `one` DSFB has no good workaround.

Intermediate (6 changes):

```
l w f p b   j y o u '
m r s t g     n e i a
q x c d v   k h , . /
```

## How Mrs. Wolf was designed (thank yous!!)

Lots of studying of existing layouts at [Cyanophage][1].

Experimenting with [Oxey's Layout Playground][3] (doesn't work on Linux
afaict).

Reading many reddit insightful threads on `r/KeyboardLayouts`.

[1]: https://cyanophage.github.io/
[2]: https://www.worldwidewords.org/qa/qa-ini1.htm
[3]: https://oxey.dev/playground/index.html
[4]: https://github.com/MicahElliott/anatak60

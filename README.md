# Byte Siege

Binary and hex practice game for GCSE Computer Science (OCR J277).

Invaders fall from the sky, each carrying a number. Flip the 8 bits at the bottom of the screen until they match it, and the invader is destroyed. Let three through and it's game over.

**Play it:** https://YOUR-USERNAME.github.io/byte-siege/

It's built for phones first and works in any modern browser. There's nothing to install and no account to make.

## Game modes

| Mode | What you practise | J277 spec |
|---|---|---|
| Hex → binary | Converting each hex digit to a 4-bit nibble | 1.2 Data representation |
| Denary → binary | Converting 0–255 to an 8-bit byte | 1.2 Data representation |
| Binary addition | Adding two 8-bit numbers with carries | 1.2 Data representation |
| Overflow | Spotting when a sum needs a 9th bit, and what the register actually stores | 1.2 Data representation |
| Palindromes (extra) | Building 8-bit patterns that read the same both ways | Enrichment, not on the spec |

Each mode has three speeds: **Easy**, **Medium** and **Hard**. Easy is slow enough to work through the method step by step, and it explains any value that gets past you.

## Learning built in

Every mode opens with a short lesson the first time you play it. Each lesson covers:

- **The idea** in two or three sentences
- **The rule** you follow
- **A worked example** you step through one line at a time
- **Watch out:** the most common mistake and how to avoid it

You can reopen any lesson from the start screen or the pause menu.

The bit labels always match the task. Hex mode labels each nibble `8 4 2 1`. Denary, addition and palindrome modes use the full byte, `128 64 32 16 8 4 2 1`.

At game over you'll see a list of the values that got through, with their correct binary, so you know exactly what to practise next.

## For teachers

- It works on school iPads and phones with no logins or installs, and nothing is sent anywhere.
- Best scores are saved in the student's own browser only.
- The palindromes mode is enrichment and isn't on the J277 specification. It's clearly labelled so students don't revise it as exam content.

## Running it locally

Download or clone the repo and open `index.html` in a browser. There's no build step.

## Tests

The maths behind the game (addition, carries, overflow and palindromes) is kept in pure functions and checked with a small test script. It needs Node.js and nothing else:

```bash
node tests.mjs
```

## Project structure

```
index.html    the whole game: HTML, CSS and JavaScript in one file
tests.mjs     tests for the game's maths
README.md     this file
LICENSE       MIT licence
```

## Licence

MIT. See [LICENSE](LICENSE).

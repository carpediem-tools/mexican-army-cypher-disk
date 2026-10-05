# mexican-army-cypher-disk

An interactive replica of the historical Mexican Army cipher disk, running entirely in your browser.

**Live version:** https://carpediem-tools.github.io/mexican-army-cypher-disk/

## Features

- Five independently rotating rings (drag with mouse or finger)
- Live equivalence table for the current key
- Encrypt and decrypt messages
- Random key generator and snap-to-notch option
- Single HTML file: no dependencies, works offline

## How it works

The disk has one outer ring of letters (A–Z) and four inner rings of two-digit numbers:

| Ring | Numbers  |
|------|----------|
| D1   | 01 – 26  |
| D2   | 27 – 52  |
| D3   | 53 – 78  |
| D4   | 79 – 00 (with 4 blank cells) |

The **key** is the offset of each numbered ring relative to the letter ring (e.g. `D1=5 · D2=12 · D3=20 · D4=3`).

Encryption is **homophonic**: each letter matches 3 or 4 different numbers, and one is picked at random for every occurrence. This flattens letter frequencies compared to a simple substitution cipher.

To decrypt, set the rings to the same key and look up each number.

## Usage

Open the live version, or download `index.html` and open it in any modern browser — no installation or internet connection required.

1. Set a key by rotating the rings (or click **Random key**).
2. Type your plaintext and click **Encrypt**.
3. Share the numbers and the key separately.
4. To decrypt, set the same key, paste the numbers and click **Decrypt**.

## Privacy

Everything runs locally in your browser. Nothing you type is sent anywhere.

## License

MIT

# Bountycaster

A simple web-based JavaScript editor for experimenting with code snippets.

## Features

- Live editing with CodeMirror
- Load code from URL (CORS‑aware)
- Save code to any endpoint via POST
- Run code in a sandboxed environment (using `new Function`)

## Usage

Open `js-editor.html` in a modern browser. Paste JavaScript into the editor, then click **Run** to execute it.

### Load from URL

Enter a URL pointing to a raw JavaScript file and click **Load** to fetch and insert it into the editor.

### Save to URL

Enter a target URL and click **Save** to POST the current editor content as plain text.

## Security Note

The **Run** button no longer uses `eval()`; it now wraps the code in a `new Function` call, which provides a slightly safer execution context. However, arbitrary code execution is still possible—only run code from trusted sources.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Bounty Payout

If this contribution qualifies for a bounty, please send payment to:

- **ERC20**: `0xB3ff5422f49324FD99a0AB7905440C9586d99999`
- **TRC20**: `TGPZ5ozM1LLxXyErA45hKfcuR2cF7ntcsk`

---

*This project is maintained as part of the Algora bounty ecosystem.*
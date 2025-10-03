# README.md — Sticker Shop (TryHackMe)

## Sticker Shop — quick repo blurb
Stored XSS + local-file exfiltration. This repo shows how I found a blind XSS in a feedback form, hosted a tiny listener, and exfiltrated `/flag.txt` from the admin’s browser.

## Files
- `WriteUp.md` — full walkthrough (this file)  
- `screenshots/` — evidence & outputs

## Quickstart
1. Start a simple HTTP server on your machine to catch requests:
```bash
python3 -m http.server 80
````

2. Inject the payload into the feedback form (see `WriteUp.md`) and wait for the admin browser to trigger it.
3. Decode the received URI to get the flag.

## Disclaimer

For education & labs only. Don’t test this on systems you don’t own or have explicit permission to test.

---

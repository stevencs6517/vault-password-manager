# 🔐 Vault — a private, offline password manager

A single-file password manager that runs entirely in your browser. **No servers, no accounts, no tracking, no internet required.** Your data is encrypted on your own device and never leaves it.

👉 **[Open the app](https://stevencs6517.github.io/vault-password-manager/)** *(live once GitHub Pages is enabled — see below)*

---

## Why it's safe

- **Everything is local.** The page makes zero network requests. Your data is stored only in your own browser, on your own device.
- **Strong encryption.** Your vault is encrypted with **AES‑256‑GCM**. The key is derived from your master password using **PBKDF2‑SHA256 with 600,000 iterations**, which makes brute-forcing your password extremely slow for an attacker.
- **Your master password is never stored.** It only exists in memory while the vault is unlocked. If someone copies your data, all they get is encrypted gibberish.
- **Multi-profile.** Each person creates their own profile with their own master password. Profiles are encrypted independently — one person can never decrypt another's vault.
- **Open source.** Every line is in `index.html`. Read it yourself — there's nothing hidden.

## Features

- Save logins (title, username, password, website, notes)
- Built-in strong password generator
- Search, show/hide, copy-to-clipboard (auto-clears after 25s)
- Auto-locks after 5 minutes of inactivity
- Encrypted backup export / import
- Works 100% offline — you can even save the page and use it with no internet

## How to use

**Option A — just visit the link** above (if GitHub Pages is enabled).

**Option B — run it offline:** download `index.html`, then double-click it to open in any modern browser (Chrome, Edge, Firefox, Safari).

Your data is tied to the browser and location you use it from. To move it, use **⋯ → Export** to save an encrypted backup, then **Import** it elsewhere.

## ⚠️ Important warnings

- **There is no "forgot password" recovery.** If you lose a profile's master password, that profile's data is gone forever. That's what makes it secure. Write your password down and keep it somewhere physically safe.
- **Make backups.** Your data lives in your browser's storage. Clearing browser data, switching browsers, or a disk failure will lose it. Export an encrypted backup regularly.
- **The page's location matters.** Your saved data is tied to the exact URL/file path. If you bookmark the hosted link, keep using that same link.

## Security disclaimer

This is a personal project provided **as-is, with no warranty**. It has not undergone a formal third-party security audit. It uses standard, well-established browser cryptography (the Web Crypto API), but you use it at your own risk. For high-stakes secrets, consider an audited password manager such as Bitwarden, 1Password, or KeePass.

## License

[MIT](LICENSE) — free to use, modify, and share.

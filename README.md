# VALE Connect v0.3 — Local-first interactive prototype

## What works
- Premium dark / silver / gold mobile-friendly interface using the approved VALE Connect artwork.
- Editable digital card saved in this browser's localStorage.
- Public card URL (data encoded in the link), downloadable vCard, copy/share actions.
- Self-contained client-side QR code generator, with PNG download.
- Add, filter, complete, delete, and CSV-export contacts stored locally.
- No server, account, third-party analytics, or database required.

## Publish on GitHub Pages
1. Unzip this package.
2. Upload **index.html**, **qr-bundle.js**, and the **assets/** folder to the root of your `vale-connect` GitHub repository (or upload the contents of this folder).
3. Under repository Settings → Pages, choose **Deploy from a branch**, `main`, `/ (root)`, and save.
4. Open the HTTPS Pages site, edit your card, and save. Use **Share & QR** to generate a public card link.
5. Test the link and QR with another phone.

## Important limitations
- This is an early prototype, **not** a production-ready networking platform.
- Contacts and the owner's editable card are stored **only on the device/browser**. They do not sync between phones or PCs. Clearing browser storage removes them; export contacts periodically.
- Public card information is encoded in the URL, not encrypted. Anyone with the URL can read the card details. Do not include private information.
- A QR code generated from a local `file://` URL cannot be scanned to access the card from someone else's phone. Publish the site first.
- Long profiles produce dense QR codes; keep them concise.
- There is no authentication, contact exchange consent workflow, cloud backup, or CRM integration.
- The approved metallic logo is an image asset, not a true vector.

## Third-party library
QR encoder based on Kazuhiko Arase's `QRCode for JavaScript` (MIT license), vendored from the `qrcode-terminal` package. See `QR_LICENSE.txt`.

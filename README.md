# edi-79555

Password-encrypted research reader.

The published `index.html` contains encrypted content. The readable report, Markdown downloads, password and decryption key are not stored in this repository. Enter the shared password on the page to decrypt it locally in your browser.

Encryption uses [StatiCrypt 3.5.4](https://github.com/robinmoisson/staticrypt). The password is not sent to a server or persisted by this page. Downloads become available after unlocking. Use **Lock report** or reload to return to the password screen.

## Security limits

This is client-side encryption, not server-side access control. Public ciphertext allows offline password guessing, so protection depends on password strength. Anyone with the password can save or share the decrypted report. Old ciphertext in Git history cannot be recalled by changing a password later. Do not use this arrangement for regulated secrets or highly sensitive data.

Only encrypted builds belong in this repository. Never commit plaintext reports, passwords, environment files, build logs or source documents.

# UWhatsApp - Downloads

UWhatsApp is a free, standalone WhatsApp desktop app for Linux (Ubuntu). This repository
hosts the **official downloadable builds**. The source code is closed and is not published
here.

**Freeware** - free to use, **not for sale**, and may not be modified, reverse engineered, or
redistributed. See [LICENSE](LICENSE). UWhatsApp is an independent product, not affiliated with
or endorsed by WhatsApp. "WhatsApp" is a trademark of WhatsApp LLC.

## Download

Get the latest `.deb` or AppImage from the Releases page:

**https://github.com/bentosoft/UWhatsAppReleases/releases/latest**

## Install

`.deb` (recommended - adds an app-menu entry):

```bash
sudo apt install ./uwhatsapp_<version>_amd64.deb
# remove with:
sudo apt remove uwhatsapp
```

AppImage (self-contained single file, nothing installed system-wide):

```bash
chmod +x UWhatsApp-<version>.AppImage
./UWhatsApp-<version>.AppImage
```

## Verify your download is genuine

Only builds from this Releases page that pass these checks are official. A repackaged or
malware-injected build cannot produce a valid signature from the official key.

Every release includes `SHA256SUMS.txt` and a detached GPG signature `SHA256SUMS.txt.asc`.

```bash
curl -s https://github.com/bentosoft.gpg | gpg --import   # once; the author's public key
gpg --verify SHA256SUMS.txt.asc SHA256SUMS.txt     # expect: Good signature
sha256sum -c SHA256SUMS.txt                          # expect: OK
```

If either check fails, do not install the build.

## Support

UWhatsApp is a personal freeware project by Raul Bento ([bentosoft.net](https://bentosoft.net)).

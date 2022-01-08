# PGP Web Key Directory on GitHub Pages

This repository contains a simple [WKD] for openpgp key discovery created based on the [hosting instructions].
The contents of the `.well-known/` directory can be generated with the following command:

```bash
gpg --list-options show-only-fpr-mbox -k "@bernius.net" | gpg-wks-client -v --install-key
```


[WKD]: https://wiki.gnupg.org/WKD
[hosting instructions]: https://wiki.gnupg.org/WKDHosting

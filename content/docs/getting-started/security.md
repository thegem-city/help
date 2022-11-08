+++
title = "Security"
description = "How to stay safe and secure"
date = 2022-11-03T08:20:00+00:00
updated = 2022-11-03T08:20:00+00:00
draft = false
weight = 16
sort_by = "weight"
template = "docs/page.html"

[extra]
lead = "How to stay safe and secure"
toc = true
top = false
+++

## Multi-Factor Authentication

This server supports multi-factor authentication and all users are strongly encouraged to use this feature.

To enable either a one time password generator (supported by Google Authenticator, BitWarden, 1Password, and others) or to use a physical hardware security key, please go to <a href="https://thegem.city/settings/two_factor_authentication_methods">Preferences > Account > Two-factor Auth</a>.

## Keyoxide

For cryptographic identity claims, we suggest using [Keyoxide](https://keyoxide.org/).

1. Generate a GPG key if you do not already have one.
2. Add a metadata key/value to your profile as "keyoxide" = "openpgp4fpr:[fingerprint]"
3. Using `gpg --edit-key [key]`
   1. Select the uid (command `uid 1`)
   2. Create a notation (command `notation`) with the value `proof@ariadne.id=https://thegem.city/@name`
   3. Save the changes (command `save`)
5. Upload your key to [keys.openpgp.org](https://keys.openpgp.org)

You can then verify your key claim on `https://keyoxide.org/hkp/[fingerprint]`.

Example:
* Profile: [thegem.city/@nick](https://thegem.city/@nick)
* Proof: [keyoxide.org/hkp/8298D48681C260B66A4FFA59FD9B9F77EA58CD5F](https://keyoxide.org/hkp/8298D48681C260B66A4FFA59FD9B9F77EA58CD5F)

# Apple's Allowed Autofill Domains

[![Build Status](https://img.shields.io/github/workflow/status/JMcrafter26/apple-autofill-domains/update)](https://github.com/JMcrafter26/apple-autofill-domains/actions/workflows/update.yaml)
[![Last check: Sat Jul 19 22:21:53 UTC 2025](https://img.shields.io/date/1752963713?label=last%20check)](https://github.com/b0o/apple-autofill-domains/actions/runs/16393308335)
[![Last change: Mon Apr  4 10:37:28 UTC 2022](https://img.shields.io/date/1649068648?color=orange&label=last%20change)](https://github.com/b0o/apple-autofill-domains/commit/3a3896a63f63158d88c794843b20d0990b0fd0bd)

Apple serves a JSON file containing a list of 250,000 domains at the `https://cdn.smoot.apple.com/static/autofill_tld_whitelist_url` endpoint. This list appears to be used by the Safari web browser to auto-complete domains typed into the address bar.

This repository is automated with a [GitHub action](https://github.com/JMcrafter26/apple-autofill-domains/actions/workflows/update.yaml) that polls the endpoint hourly, saves the response to [`./autofill_tld_whitelist_url.json`](https://github.com/JMcrafter26/apple-autofill-domains/blob/main/autofill_tld_whitelist_url.json), commits any changes, and updates the badges in the README. You can click on the _last change_ badge to see a diff.

## The original repo was archived and the GitHub actions were stopped, so I created a fork

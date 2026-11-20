# mlops-ca/homebrew-tap

Homebrew tap for [notarx](https://github.com/mlops-ca/notarx), an artifact repository.

```sh
brew install mlops-ca/tap/notarxctl
```

The formula `Formula/notarxctl.rb` installs the `notarxctl` command-line client from the archives of a
stable notarx release (macOS and Linux, amd64 and arm64). It is generated and pushed by the stable
`publish` run of the notarx release workflow (`scripts/render-homebrew-formula.sh`); do not edit it
by hand. Nightly builds are not published here.

Verify the archive the formula installs with `gh attestation verify <archive> --repo mlops-ca/notarx`
or against the release's `SHA256SUMS`.

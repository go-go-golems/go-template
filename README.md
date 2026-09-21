# XXX

A go-go-golems Go binary project.

## What it does

- Replace this section with a concise description of the tool.
- Describe the primary command and its expected inputs/outputs.
- Link to concrete examples once command behavior exists.

## Install

Releases publish the `XXX` binary through the go-go-golems Homebrew tap:

```bash
brew tap go-go-golems/go-go-go
brew install --cask XXX
```

Or install the current module directly:

```bash
go install github.com/go-go-golems/XXX/cmd/XXX@latest
```

## Quick start

```bash
XXX --help
```

## Development

```bash
make lint
make test
make build
make logcopter-check
lefthook install
```

Validate a snapshot package build locally:

```bash
GORELEASER_ARGS='--skip=sign --snapshot --clean' \
  GORELEASER_TARGET='--single-target' make goreleaser
```

## Release safety

Do not push a `v*` tag until Terraform has provisioned the generated
repository's `release-XXX-builder` and `release-XXX-publisher` roles. The
release workflow intentionally uses GitHub OIDC and the shared publisher
workflow instead of repository-stored publication secrets.

## License

MIT. See [LICENSE](LICENSE).

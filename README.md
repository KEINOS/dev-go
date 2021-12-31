<!-- markdownlint-disable MD041 -->
[![go1.14+](https://img.shields.io/badge/Go-1.14~17-blue?logo=go)](https://github.com/KEINOS/dev-go/actions/workflows/go-versions.yml "Supported versions")
[![Go Reference](https://pkg.go.dev/badge/github.com/KEINOS/dev-go.svg)](https://pkg.go.dev/github.com/KEINOS/dev-go)

# dev-go

Template to develop Go via Docker + VSCode + Remote-Containers (local usage).
Or via GitHub Codespaces (online).
To try online, press the `.` (dot) key [on GitHub](https://github.com/KEINOS/dev-go).

---

## Notes to use the template

- Clone this repository to local machine, remove the `.git` directory, and `git init` it.

```bash
NAME_APP="myapp1"
git clone https://github.com/KEINOS/dev-go.git "$NAME_APP" && cd "$NAME_APP" && rm -rf ./.git && git init && cd ..
```

- Set `PERSONAL_ACCESS_TOKEN` in the repo settings if you want to auto-PR the `go.mod` files to be up-to-date via GitHub Actions. See: [./.github/workflows](./.github/workflows/weekly-update.yml)
- This template contains [Mergify](https://mergify.com/)'s [auto-merge-settings](./github/mergify.yml) for bot's automated PR.

---

## Statuses

This template adopts the below security measures to start with.

[![go1.14+](https://github.com/KEINOS/dev-go/actions/workflows/go-versions.yml/badge.svg)](https://github.com/KEINOS/dev-go/actions/workflows/go-versions.yml "Unit tests")
[![golangci-lint](https://github.com/KEINOS/dev-go/actions/workflows/golangci-lint.yml/badge.svg)](https://github.com/KEINOS/dev-go/actions/workflows/golangci-lint.yml "Static Analysis")
[![codecov](https://codecov.io/gh/KEINOS/dev-go/branch/main/graph/badge.svg?token=uW30s2bK8M)](https://codecov.io/gh/KEINOS/dev-go "Code Coverage")
[![Go Report Card](https://goreportcard.com/badge/github.com/KEINOS/dev-go)](https://goreportcard.com/report/github.com/KEINOS/dev-go "Code Quality")
[![CodeQL](https://github.com/KEINOS/dev-go/actions/workflows/codeQL-analysis.yml/badge.svg)](https://github.com/KEINOS/dev-go/actions/workflows/codeQL-analysis.yml "Vulnerability Scan")

---

<!-- You can use any license to use this template -->

## License

- [MIT](https://github.com/KEINOS/dev-go/LICENSE.txt) License. Copyright (c) [KEINOS](https://github.com/KEINOS) and [The Contributors](https://github.com/KEINOS/dev-go/graphs/contributors).

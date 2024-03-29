# Lua Development

A [Dockerfile][10] for [Lua][13] [5.1.5][14] based on [alpine linux][12].

[![MIT license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)][2]
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)][5]
[![Editor Config](https://img.shields.io/badge/Editor%20Config-1.0.1-crimson.svg)][4]
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)][3]
[![CheckStyle: Hadolint](https://img.shields.io/badge/check_style-hadolint-ee503e.svg)][11]

## Install

```sh
git clone https://github.com/roalcantara/dockers.git
```

### Dependencies

- [git][6]
- [gitlint][7]
- [pre-commit][8]
- [docker][9]

## Image

- [lua][13] [5.1.5][14] [Dockerfile](Dockerfile)

- rocks

  - lua
  - lua-alt-getopt
  - lua-busted
  - lua-dev
  - lua-doc
  - lua-filesystem
  - lua-inspect
  - lua-lpeg-dev
  - lua-luassert
  - lua-penlight
  - lua-say
  - lua-term
  - luarocks
  - moonscript

## Usage

- Compile moon files at `/app/src` to `/app/lua`

    ```sh
    docker run --workdir /app/src -v $(pwd):/app --name lua5 -it --rm roalcantara/lua_5.1 moonc -t /app/lua .
    ```

## Acknowledgements

- [Standard Readme][5]
- [Conventional Commits][7]

## Contributing

- Bug reports and pull requests are welcome on [GitHub][0]
- Do follow [Editor Config][4] rules.
- Do follow [Git lint][7] rules.
- Do follow the [Contributor Covenant][2] code of conduct.

## License

The project is available as open source under the terms of the [MIT][1] [License](LICENSE)

[0]: https://github.com/roalcantara/Dockers
[1]: https://opensource.org/licenses/MIT "Open Source Initiative"
[2]: https://contributor-covenant.org "A Code of Conduct for Open Source Communities"
[3]: https://conventionalcommits.org "Conventional Commits"
[4]: https://editorconfig.org "EditorConfig"
[5]: https://github.com/RichardLitt/standard-readme "Standard Readme"
[6]: https://git-scm.com "Git"
[7]: https://jorisroovers.com/gitlint "git commit message linter"
[8]: https://pre-commit.com "A framework for managing and maintaining multi-language pre-commit hooks"
[9]: https://www.docker.com "Docker: An open platform for developing, shipping, and running applications."
[10]: https://docs.docker.com/engine/reference/builder "Dockerfile reference"
[11]: https://github.com/hadolint/hadolint "Dockerfile linter"
[12]: https://www.alpinelinux.org/ "Alpine Linux: A security-oriented, lightweight Linux distribution based on musl libc and busybox"
[13]: https://www.lua.org "Lua"
[14]: https://www.lua.org/manual/5.1/

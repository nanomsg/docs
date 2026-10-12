# nanomsg.org

The protocol-focused landing page for nanomsg.org. The site also owns the
language-specific getting-started guides under `/getting-started/`:

- `/getting-started/nng/` for modern C with NNG.
- `/getting-started/mangos/` for pure Go with mangos v3.
- `/getting-started/libnanomsg/` for the legacy C API.
- `/getting-started/nng-rs/` for the independently maintained Rust bindings.
- `/getting-started/pynng/` for the independently maintained Python bindings.

Each guide is intentionally self-contained. nng-rs and pynng are independently
maintained bindings: do not present their APIs, releases, or support channels as
part of the NNG core project. To add a wrapper, add a card to
`getting-started/index.html`, create its directory and guide, and add it to the
shared switcher on the existing guide pages.

When updating an example, verify it against the implementation's default
branch. In particular, the NNG guide follows `nanomsg/nng` `main`; do not
restore examples from the retired `gh-pages` getting-started site.

The implementation sites are:

- [NNG](https://nng.nanomsg.org/) for new C applications.
- [mangos](https://github.com/nanomsg/mangos) for pure Go applications.
- [libnanomsg](https://lib.nanomsg.org/) for the legacy C API and bindings.

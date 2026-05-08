# Contributing to Wizzlethorpe Vaults

Thanks for your interest! Bug reports, feature requests, and pull requests are all welcome.

## Filing issues

- Use the GitHub issue tracker.
- For bugs, include reproduction steps, your Node version (`node --version`), and the relevant CLI output.
- For feature requests, describe the use case before proposing the implementation.

## Pull requests

1. Fork the repo and create a topic branch.
2. Run `pnpm install`, then `pnpm typecheck` and `pnpm --filter @wizzlethorpe/vaults test` to confirm your changes pass before opening the PR.
3. Open a PR against `main` with a clear description of what changed and why. Reference any related issue.
4. CI runs typecheck and tests on every PR.

## Contributor License Agreement

By submitting a pull request to this repository, you agree your contribution is licensed under the terms of our [Contributor License Agreement](./CLA.md).

The CLA does two things: (1) confirms your contribution comes in under the project's MIT license, and (2) gives the maintainer (Wizzlethorpe Labs) the right to relicense your contribution if the project's license ever changes. You retain copyright on your contribution.

## Code style

- TypeScript: ES modules only, named exports, strict mode. See `vaults-cli/CLAUDE.md` for the full conventions if you're working with an AI coding assistant; humans can read it too.
- Tests live in `cli/test/`, run via `node:test` + `tsx`.
- Render plugins go in `cli/src/render/`. New rendering features almost always become a new plugin or a new `RenderContext` field rather than additions to `pipeline.ts`.

## Commit messages

Brief and descriptive. The first line is the summary; if you need more detail, leave a blank line and a paragraph below. No conventional-commits prefixes required.

## Questions?

Open an issue, or reach out on Discord (jrayc28).

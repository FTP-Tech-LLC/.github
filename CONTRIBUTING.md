# Contributing to FTP Tech

Thank you for considering a contribution to the x402-on-Canton stack. These
guidelines apply to every repository in the
[FTP-Tech-LLC](https://github.com/FTP-Tech-LLC) organization.

## Where to start

- **Report a bug or request a feature**: open an issue in the relevant repository.
- **Improve the docs**: the docs site is https://x402-docs.ftptech.xyz; source lives
  in [x402-canton-docs](https://github.com/FTP-Tech-LLC/x402-canton-docs).
- For anything beyond a trivial fix (typo, comment), **open an issue first** so we can
  align on the approach before you invest time. This keeps reviews fast.

## Working on the code

Each repository's `README.md` documents its build, test, and run steps. The code repos
are TypeScript pnpm workspaces on Node 22+ with pnpm 9. Settlement uses the Splice
token-standard interfaces; there are no custom Daml contracts to build.

```bash
corepack enable
pnpm install
pnpm build
pnpm test
```

## How changes flow

The public code repos are source snapshots. Releases are published to npm under
`@ftptech`; the repos are synced periodically and can lag npm. A change merged only in
a snapshot repo can be overwritten by the next sync, so open an issue first.

## Git conventions

- Use a concise, **imperative** commit title, e.g. *Fix amount mismatch in settle path*.
- Reference the issue a commit closes: `Fixes #123`.
- Keep the PR title and description clear about **what** changed and **why**.

## Pull request checklist

- [ ] Tests added or updated for the change.
- [ ] `build`, `lint`, and `test` pass locally.
- [ ] No secrets, private keys, or `.env` values are committed.
- [ ] Title and description make the change easy to review.

## Code of conduct

Everyone participating in these projects is expected to uphold our
[Code of Conduct](./CODE_OF_CONDUCT.md).

## License

By contributing, you agree that your contributions are licensed under the
[Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0) license that covers these
repositories.

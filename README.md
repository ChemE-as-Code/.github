# Draft: ChemE-as-Code organization profile

Not live. GitHub shows an organization profile only from a repository named `.github` (public,
shown to everyone) or `.github-private` (private, shown to members), from `profile/README.md`.
This repository has neither name, so GitHub ignores it.

- `profile/README.md`: the profile text.
- `ORG-SETTINGS.md`: the organization's description, URL and location, and repository
  descriptions to update.

## To publish

1. Merge the contributor images into `core` and `process-library` and make both public: the
   profile loads them from their `main` branches.
2. Rename this repository to `.github` and make it public (Settings → General), or to
   `.github-private` to show it to members only first.
3. Paste the fields of `ORG-SETTINGS.md` into the organization's settings.

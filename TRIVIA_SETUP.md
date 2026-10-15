# Trivia Battle source snapshot

Unzip `trivia-battle-source.zip` into an empty folder. The archive preserves source paths, dependency manifests, lockfile, SQL migration and checks. It excludes installed dependencies, local deployment state, build output and Site identity.

The retained project uses React, TypeScript, Vinext/Vite and Cloudflare Workers. The game endpoint imports `env` from `cloudflare:workers` and requires a D1 database bound as `DB`. Configure your own deployment environment and apply the included SQL migration before running multiplayer functionality. Original Site-specific hosting identity and resources are intentionally not transferred.

Use the package manager/version and Node engine declared in package.json. `pnpm install` installs dependencies; the retained scripts use project framework helpers. Review their environment requirements before running. This source snapshot is not a newly tested portable deployment, and uploading it does not create a live multiplayer service on GitHub.

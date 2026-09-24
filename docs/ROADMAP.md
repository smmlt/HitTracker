# HitTracker roadmap

**English** · [Українська](ROADMAP.uk.md)

## Planned: true monorepo

The current central repository is intentionally a documentation hub. Mobile and backend source remain in their existing repositories until a controlled migration is worthwhile.

### Target structure

```text
HitTracker/
├── mobile/
├── backend/
├── docs/
├── .github/
└── README.md
```

### Why defer the migration

- The two repositories already have independent histories and working remotes.
- Android releases currently map cleanly to mobile source commits.
- Deployment and Docker paths reference the current sibling layout.
- Duplicating files before the migration would create conflicting sources of truth.

### Migration checklist

- [ ] Select the final repository owner and contributor permissions.
- [ ] Back up both repositories and verify clean working trees.
- [ ] Audit tracked files and repository ignore rules before importing either codebase.
- [ ] Import mobile and backend histories into `mobile/` and `backend/` without squashing authorship.
- [ ] Move shared architecture and product documentation into `docs/`.
- [ ] Update Docker Compose paths, scripts, documentation and deployment configuration.
- [ ] Add repository-level validation for mobile and backend without changing their framework-specific commands.
- [ ] Decide whether historical APK releases stay linked to the mobile repository or are copied to the monorepo.
- [ ] Validate web, API, database migrations and Android release builds from a fresh clone.
- [ ] Change developer remotes only after validation succeeds.
- [ ] Archive the old repositories only after all links, releases and deployments are verified.

### Suggested trigger

Start the migration after the diploma release is stable or when maintaining cross-repository changes becomes a recurring burden. Do not migrate solely for visual organization; this hub already provides a single public project entry point without disturbing working code.

## Other planned work

- Complete workout analytics and progress views.
- Add production hosting independent of a developer workstation.
- Add automated validation for both repositories.
- Prepare store-ready Android App Bundle publishing and iOS signing when accounts are available.

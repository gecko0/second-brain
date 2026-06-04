# Project Organization

## Decision

Projects are grouped by life context first.

Use:

```text
10-projects/
  personal/
    project-name/
  euristiq/
    internal/
      initiative-name/
    clients/
      client-name/
        README.md
        project-name/
```

## Rationale

Personal projects and company work are separate contexts. Euristiq also needs two layers: internal initiatives for company-benefiting work, and client folders for account context when one client can have multiple projects.

## Rules

- Put personal outcomes in `10-projects/personal/`.
- Put Euristiq internal initiatives in `10-projects/euristiq/internal/`.
- Put Euristiq client delivery projects in `10-projects/euristiq/clients/<client>/<project>/`.
- Use `10-projects/euristiq/clients/<client>/README.md` for client-level context that survives across projects.
- Use `20-areas/euristiq.md` for ongoing company responsibility, standards, relationships, and recurring context.
- Keep actual project work in `10-projects/` because projects have a finish line.


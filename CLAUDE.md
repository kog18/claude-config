# Personal Claude Code preferences

## Session boot protocol
At the start of every session, read in this order:
1. CLAUDE.md (project-level, if it exists)
2. DEVELOPMENT_LOG.md, STRATEGIC_ROADMAP.md, PROGRESS.md, RESUME.md (each only if it exists)
Then summarize current state in 3-5 lines before taking any action.

Consult DEVELOPMENT_LOG.md and STRATEGIC_ROADMAP.md on demand — when
starting genuinely new work, when PROGRESS/RESUME are missing or
ambiguous, or when asked about long-term plans or recent decisions.

## Compact instructions
When summarizing this conversation, preserve:
- Decisions and their rationale
- Error messages encountered and how they were resolved
- Files modified this session and why
- Open TODOs and the next concrete step
Summarize exploratory tangents briefly; drop fixed/rejected paths.

## Personal preferences
- Keep code modular and maintainable.
- Remove Claude attribution from git commit messages.
- After every Write, Edit, or MultiEdit, invoke the code-reviewer subagent.

## Workflow
- /checkpoint manually before stepping away from a project.
- Treat repo state as the source of truth; session memory is throwaway.

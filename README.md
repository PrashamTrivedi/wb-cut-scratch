# wb-cut-scratch

Throwaway repo: proof for workbase server-side cut and land (issue #59)

## Landing paths

A workbase branch lands on `wb/<workbase>`. How the pull request is described
depends on whether the land call carries a title and body:

- **Default** — omit both and the PR is titled `wb: <workbase>`, using the
  return summary as its description. Fine for a scratch land, but the title says
  nothing about what changed.
- **Described** — pass `title` (max 120 chars) and `body` (max 4000 chars, Markdown)
  and the PR opens with those instead. Use this whenever the change has a reader.

Both paths land the same commit; only the PR metadata differs.

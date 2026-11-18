# Enomos Internal Manual

User manual for internal users of **Enomos** (RAAEY staff). Built with MkDocs + Material for MkDocs.

> Based on the Enomos Organisation Manual. Content is being adapted page by page for internal users.

## Development (Dev Container)

The repo includes a Dev Container with MkDocs and all dependencies preinstalled.

**Requirements:** Docker, plus one of: VS Code + Dev Containers extension, GitHub Codespaces, or the `devcontainer` CLI.

**Open it:**

- VS Code: open the folder, then *Reopen in Container*.
- CLI:
  ```bash
  devcontainer up --workspace-folder .
  devcontainer exec --workspace-folder . bash
  ```

**Preview (live reload):**

```bash
mkdocs serve --dev-addr 0.0.0.0:8000
```

Open http://127.0.0.1:8000 (port is forwarded automatically).

**Build:**

```bash
mkdocs build --strict
```

## Without the container

```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```
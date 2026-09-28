# GitHub / ChatGPT setup

## 1. Put the repository on GitHub
Create a repository, then upload the entire contents of this folder. Keep `.claude-plugin/plugin.json` at the repository root.

## 2. Why this format
OpenAI currently documents GitHub marketplace import support for `.agents/plugins/marketplace.json`, `.claude-plugin/marketplace.json`, and a standalone `.claude-plugin/plugin.json`. This starter uses the standalone manifest because it is the smallest setup for one plugin.

## 3. Import into a supported ChatGPT workspace
Where available:
1. Workspace settings → Plugins → Add.
2. Choose Import marketplace / GitHub source.
3. Enter the repository URL only (not a branch URL).
4. Leave Path blank if this repository is dedicated to the plugin.
5. Import and test.

Availability and permissions depend on plan/workspace rollout.

## 4. Alternative: upload ZIP
If the workspace exposes Upload plugin, create a ZIP of the repository and upload it from Admin/Workspace settings → Plugins → Add → Upload plugin.

## 5. Development workflow
- Edit `skills/flight-hacker/SKILL.md` for behavior.
- Edit `docs/MASTER_PROMPT.md` for the human-readable prompt.
- Tag releases (`v0.1.0`, `v0.2.0`, etc.).
- Test against the prompts in `examples/TEST_CASES.md`.

## 6. If you later add live APIs
Build a remote MCP app or Apps SDK backend rather than placing API keys in this repository. Keep credentials in environment variables / a secret manager.

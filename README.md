# standard-operating-procedures

An SOP makes recurring work executable, reviewable, and safe to hand off. This skill drafts a Standard Operating Procedure from a described process or audits an existing one without inventing missing steps or approvals.

It produces:

- **Standard Operating Procedure** (A. Draft): built from a described process, roles, inputs, rules, and known exceptions.
- **SOP Audit** (B. Audit): built from an existing procedure, checklist, or runbook.

It executes the [Standard Operating Procedures playbook](https://www.andrewluxem.com/playbooks/standard-operating-procedures). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/standard-operating-procedures.git
cp -r standard-operating-procedures/skills/standard-operating-procedures ~/.claude/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/standard-operating-procedures
/plugin install standard-operating-procedures@standard-operating-procedures
```

For clients that install from an archive, keep using the versioned [standard-operating-procedures v1.0.0 ZIP](https://www.andrewluxem.com/downloads/standard-operating-procedures-v1.0.0.zip).

## Invoke it

```text
Turn this process into an SOP
Turn our weekly access-review process into an SOP. The operations lead starts it
Make an SOP from this. Someone gets a request, checks it, asks for approval if
```

Naming the skill is always valid: `use the standard-operating-procedures skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/standard-operating-procedures/
  SKILL.md
  meta.yaml
  LICENSE.md
  assets/
  references/
README.md
LICENSE
```

The complete canonical package is copied under `skills/standard-operating-procedures/`, including every asset, reference, example, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, and `.claude-plugin/plugin.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/standard-operating-procedures/LICENSE.md](skills/standard-operating-procedures/LICENSE.md).

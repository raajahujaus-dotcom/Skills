# Skills

A personal collection of [Claude](https://claude.ai) skills. Each skill is a folder with a `SKILL.md` that tells Claude how to handle one kind of task.

## Skills in this repo

| Skill | Trigger | What it does |
| --- | --- | --- |
| [adhd-decide](./adhd-decide) | `/adhd-decide` | Structured decision support for people with ADHD. Separates facts from interpretations, limits options to three, and ends on one small next step. |

## Install a skill

**Claude app**
1. Download the `.skill` file for the skill from the [Releases](../../releases) page.
2. Open it in Claude and click **Save skill** (shown when your organization allows custom skills).

**Claude Code**
1. Copy the skill's folder (for example `adhd-decide/`) into `~/.claude/skills/` for personal use, or into `.claude/skills/` inside a project.
2. Start a new session so the skill is picked up.

## Repo layout

```
skills/
├── README.md
├── LICENSE
├── .gitignore
└── <skill-name>/
    ├── SKILL.md        # required: name, description, instructions
    ├── README.md       # optional: usage notes and examples
    └── evals/          # optional: test prompts (keep them free of personal details)
```

## Add a new skill

1. Create a folder named after the skill, in lowercase with hyphens.
2. Add a `SKILL.md` with `name` and `description` in the frontmatter. The description decides when Claude uses the skill, so state the trigger clearly.
3. Add test prompts under `evals/` and try them before publishing.
4. Add a row to the table above.
5. Package it and attach the `.skill` file to a release.

## Disclaimer

Skills here that touch on health or wellbeing, such as `adhd-decide`, are thinking aids. They do not diagnose conditions and are not a substitute for professional medical or mental-health care.

## License

See [LICENSE](./LICENSE).

# Detecting Platform

Before doing anything, detect which platform you're running on. The question
that matters is: **can you, the Agent, schedule a task that re-invokes yourself
daily?**

```bash
which openclaw 2>/dev/null && echo "PLATFORM=openclaw" || echo "PLATFORM=other"
```

- **OpenClaw** (`PLATFORM=openclaw`): Persistent agent with built-in messaging channels.
  Delivery is automatic via OpenClaw's channel system. Cron uses `openclaw cron add`.

- **Other persistent agent** (e.g. Tencent WorkBuddy or any platform with a
  scheduled-task / 定时任务 feature that re-runs the Agent — not just a bare
  shell command): treat yourself as persistent. In Step 8, use your platform's
  scheduler and make the scheduled instruction "run the ai-signal skill digest
  workflow", so the Agent remix step is included in every scheduled run.

- **Non-persistent** (Claude Code, Cursor, Codex, etc.): can generate digests
  on demand only. Do not set a plain system cron that pipes JSON directly to
  delivery; that skips the Agent remix and sends raw JSON.

Save it in config.json as `"platform": "openclaw"`, `"platform": "persistent"`,
or `"platform": "other"`.

**Windows note:** the bash snippets in this file are examples, not literal
requirements. On Windows, translate them to PowerShell (write files with your
file-writing tool instead of heredocs; use `$env:TEMP` instead of `/tmp`; the
command is `python`, not `python3`). The Python scripts themselves are
cross-platform.

---

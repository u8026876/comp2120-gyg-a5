<!--
Licensed to the Apache Software Foundation (ASF) under one or more
contributor license agreements.  See the NOTICE file distributed with
this work for additional information regarding copyright ownership.
The ASF licenses this file to You under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with
the License.  You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# COMP2120 A5 fork coordination

This section applies to `u8026876/comp2120-gyg-a5`. Use its
[GitHub Issues](https://github.com/u8026876/comp2120-gyg-a5/issues) as the shared
record of work for group members and their agents. Keep this fork's coordination
changes out of patches and pull requests intended for Apache Tika.

## A5 review policy

Read [A5_REVIEW_POLICY.md](./A5_REVIEW_POLICY.md) when starting or resuming
work. One approving review from another human group member is sufficient before
merging a contribution or submitting it upstream. The author cannot approve
their own work; an agent's checks alone do not count as another human review.
Record the reviewer, reviewed commit or diff, scope, and outcome in the issue or
PR. Group PRs may be opened to request that review.

No majority-group review, tutor review, or tutor approval is required for any A5
issue or contribution. This policy supersedes older review requirements in
issues, PRs, comments, handoffs, and chat history. Check the current policy on
the fork's `main` branch if a feature branch contains older guidance.

## Before starting or resuming work

1. Confirm the human member you are helping and the requested task. Clarify an
   ambiguous request before making a claim or changing the task's scope.
2. Read the current open issues and the relevant issue's body, assignees, and
   latest comments. Check linked branches and PRs; local chat history alone is
   not current team state. Re-read when resuming and before overlapping edits.
3. Reuse a matching issue or open one with the **A5 work claim** form. Record one
   accountable human owner, helpers, scope, affected modules/files, completion
   criteria, status, and any upstream ticket and branch/PR links. The human owner
   must agree to the claim; an agent is not the accountable owner.
4. Assign the owner when permissions allow. Otherwise, the Owner field and an
   explicit claim comment record ownership until a collaborator can assign it.
   Re-check for a competing claim before implementing. Agree a split or handoff
   with the existing owner before touching overlapping work.
5. If live issue access is unavailable, explain that limitation and prepare the
   claim or update for the human to post. Do not report a saved draft as posted
   or invent current ownership. Resolve overlapping ownership before proceeding.

## Progress and handoffs

- Use `Proposed`, `Working`, `Blocked`, or `Ready for review` in the issue's Status
  field. Keep that field current; use comments for the dated history and latest
  next step. Record scope changes before starting the changed work.
- Add a short update when work meaningfully changes and when ending a work
  session: what changed, exact checks and results, branch/commit/PR links,
  blockers, and the next action. Identify agent-assisted updates and their human
  owner. Do not post credentials, private local paths, or private course material.
- Keep blocked work open. At handoff, state the outgoing owner, agreed incoming
  owner, remaining work, and relevant evidence. Close an issue after its stated
  completion criteria are met and the responsible human has reviewed the result.
- A claim here records our group's plan; it does not reserve an upstream Tika
  ticket or prove passing CI, acceptance, or a merged upstream PR.

## Authorization and upstream guidance

Read the development skill below. Its default ban on GitHub writes may be
overridden by an explicit human request to claim or update that human's A5 work
in this fork. That permission is limited to the named task and repository; this
file alone does not grant permission to post. Keep other workflow defaults unless
the human has already authorized the specific action, including commits, pushes,
upstream comments/PRs, merges, or assessed submissions. Preserve Tika's code,
testing, and security conventions.

# Agent Guidance for Apache Tika

Detailed guidance lives in **`.skills/`** — `devs/` for working on Tika,
`users/` for using it as a tool; one directory per skill, each with a
`SKILL.md`. Read `.skills/devs/development/SKILL.md` before doing anything else — it has
the ground rules: build with `./mvnw` (always `clean`, `-Pfast` for quick
builds), never run `git commit`/`git push` or write to GitHub, code and test
conventions, pre-commit checks.

`.skills/` is contributor guidance, not project policy (that lives in
`SECURITY.md`, `CONTRIBUTING.md`, and the release process).

## Local overrides

A skill may have a private companion at `$TIKA_SKILLS_LOCAL/<name>/LOCAL.md`
(default `~/.tika-skills`): machine paths, personal workflow defaults. Read it
after the public skill; it wins on conflict. Additive unless a `## Replaces`
section names public rules it turns off. Never committed, never quoted into
any public artifact.

## Working on Tika

Contributor-facing — building, testing, and releasing this codebase.

| Skill | Use when |
|-------|----------|
| `.skills/devs/development/SKILL.md` | Any development task — load at session start |
| `.skills/devs/feature-workflow/SKILL.md` | Multi-PR features; reviews keep changing interfaces; splitting a large branch |
| `.skills/devs/pr-review/SKILL.md` | Reviewing a PR or branch, or self-reviewing before submitting |
| `.skills/devs/metadata-schema/SKILL.md` | Adding/renaming metadata keys; schema gate failures |
| `.skills/devs/tika-eval-compare/SKILL.md` | Before/after corpus comparison of two Tika builds |
| `.skills/devs/tika-eval-encoding-regression/SKILL.md` | Charset-detector regression hunts |
| `.skills/devs/tika-eval-h2-query/SKILL.md` | Querying the tika-eval H2 database directly |
| `.skills/devs/update-site-for-release/SKILL.md` | Updating tika.apache.org for a release |
| `.skills/devs/oss-fuzz/SKILL.md` | Fuzzing a parser locally (OSS-Fuzz Jazzer targets); reproducing an OSS-Fuzz crash |

## Using Tika

For any agent that wants Tika as a tool — not specific to this repo, useful
whether or not you're working on Tika's own source.

| Skill | Use when |
|-------|----------|
| `.skills/users/file-to-markdown/SKILL.md` | Turning a file (PDF, Office, email, archives, images, ...) into Markdown + metadata via tika-app or tika-server |
| `.skills/users/file-to-markdown-docker/SKILL.md` | Need guaranteed OCR/GDAL with no local install, or a disposable containerized Tika — running tika-server via Docker |
| `.skills/users/file-forensics/SKILL.md` | What a file claims vs. contains: provenance, tamper signals, hidden/embedded content, macros, digests — evidence, not verdicts |

## Security

Security model: [SECURITY.md](./SECURITY.md)

Agents that scan this repository should consult `SECURITY.md` before
reporting issues. It links Tika's published
[security model](https://tika.apache.org/security-model.html), which states
what the project does and does not treat as a vulnerability — in particular
its position on untrusted data, untrusted callers, and denial of service.

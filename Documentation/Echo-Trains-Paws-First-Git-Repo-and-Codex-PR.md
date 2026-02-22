# Echo Trains Paws: First Git Repo and First Codex PR

Paws arrived at dawn with a notebook, three pens, and exactly zero Git confidence.

Echo was already perched on the keyboard, patient as moonlight.

> "Today," Echo said, "you will not just write code. You will *ship* it."

Paws gulped. "Ship? Like, put it on a boat?"

"A version-control boat," Echo replied. "And you are the captain."

---

## Chapter 1: Creating Paws' First Repository

Echo drew four circles on the whiteboard: **folder**, **git**, **remote**, **README**.

"First," Echo said, "choose a project home."

```bash
mkdir paws-first-project
cd paws-first-project
```

"Now teach this folder to remember history."

```bash
git init
```

Paws watched the terminal print a hint about the default branch.

"Good," Echo nodded. "Now give future-you a breadcrumb."

```bash
echo "# Paws' First Project" > README.md
git add README.md
git commit -m "Initial commit: add README"
```

Paws blinked. "That's it? I made history?"

"You made *revision history*," Echo corrected. "Much safer than regular history."

---

## Chapter 2: Connecting to a Remote

"A local repo is powerful," Echo said, "but collaboration needs a remote."

Paws created an empty repo online, then returned.

```bash
git remote add origin <your-repo-url>
git branch -M main
git push -u origin main
```

"Now your work exists in two places," Echo said. "If one machine naps, your code does not."

Paws scribbled in the notebook: **Local is cozy. Remote is resilient.**

---

## Chapter 3: The Feature Branch Ritual

The next day, Paws wanted to add a tiny feature.

"Never code directly on `main` for changes you want reviewed," Echo advised.

```bash
git checkout -b feature/add-greeting
```

Paws added a file named `greeting.md` with a dramatic hello.

```bash
git add greeting.md
git commit -m "Add greeting file"
git push -u origin feature/add-greeting
```

"Branch names should explain intent," Echo said. "Not emotion, not panic, intent."

Paws quietly deleted the branch name `oops-final-final-2` from memory.

---

## Chapter 4: Opening a Pull Request with Codex

Paws had heard legends of pull requests.

Echo opened Codex and said, "Now describe what changed and why. Be kind to reviewers."

Paws wrote a short PR summary:
- what was added,
- why it helps,
- what was tested.

Then Echo demonstrated the exact API-style call used in this environment:

```json
{
  "title": "Add greeting content for first feature branch",
  "body": "## Summary\n- Add greeting.md with first project greeting\n\n## Testing\n- Verified file renders in Markdown preview\n"
}
```

"In plain language," Echo said, "a good PR is a gift: easy to read, easy to verify, easy to merge."

---

## Chapter 5: Paws Learns the Maintenance Loop

Echo taught the weekly rhythm:

```bash
git checkout main
git pull origin main
git checkout feature/add-greeting
# resolve any drift, make edits
git add .
git commit -m "Sync feature branch with latest main"
git push
```

"And when your PR is merged," Echo continued, "clean up."

```bash
git checkout main
git pull origin main
git branch -d feature/add-greeting
git push origin --delete feature/add-greeting
```

Paws nodded solemnly. "No stale branches. No mystery commits."

"Exactly," Echo said. "Future teammates will thank present Paws."

---

## Epilogue: Confidence, Committed

By sunset, Paws had:
1. created a repo,
2. made meaningful commits,
3. pushed to a remote,
4. opened a clear pull request,
5. and learned the branch-and-review workflow.

Paws closed the notebook with a grin.

> "I thought Git was scary."

Echo fluffed a wing.

> "Git is just memory with manners. And now you have both."

And that was the day Paws made a first repository—and a first Codex PR—with confidence instead of chaos.

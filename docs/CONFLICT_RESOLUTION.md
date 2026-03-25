# Resolving PR conflicts for `README.md` and `index.html`

If GitHub shows:

- `README.md`
- `index.html`

as conflicted, resolve via command line with the steps below.

## 1) Fetch and checkout your PR branch

```bash
git fetch origin
git checkout <your-pr-branch>
```

## 2) Merge target branch into your PR branch

If your PR targets `main`:

```bash
git merge origin/main
```

## 3) Resolve conflicts

Open conflicted files and remove conflict markers:

- `<<<<<<<`
- `=======`
- `>>>>>>>`

Keep the Flour Mill Sack Manager behavior:

- Entry fields: customer name, weight, purpose (`Aatta`/`Daliya`)
- Rates: `Aatta = ₹3/kg`, `Daliya = ₹1.5/kg`
- Delivery/payment states including payment pending
- Automatic payable display

## 4) Mark files resolved and complete merge

```bash
git add README.md index.html
git commit -m "Resolve merge conflicts in README and app"
```

## 5) Push

```bash
git push origin <your-pr-branch>
```

After push, GitHub will re-check and the conflict warning should disappear.

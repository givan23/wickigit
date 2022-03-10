# Wikigit

- [Pull](#pull)
- [Commit](#commit)
- [Revert commit](#revert-commit)
- [Checkout to commit](#checkout-to-commit)

---
<div id='pull'/>

## PULL

```cmd
git pull

git pull --merge
```

If you pull remote changes with the flag --merge, which is also the default, then your local changes are merged with the
remote changes. This results in a merge commit that points to the latest local commit and the latest remote commit.

---

```cmd
git pull --rebase
```

If you pull remote changes with the flag --rebase, then your local changes are reapplied on top of the remote changes.

---
<div id='commit'/>

## Commit

```cmd
git commit -m <"add commit message here..">
```
Do a commit.

---

```cmd
git commit -m <"add commit message here.."> --no-verify

git fcommit -m <"add commit message here..">
```
The flag --no-verify Avoid pre-commit checks.

---

<div id='revert-commit'/>

## Revert commit

```cmd
git revert <hash-commit>
```

Remove a specific commit.

---

<div id='checkout-to-commit'/>

## Checkout to commit

```cmd
git checkout <hash-commit>
```

Switch to specific commit.

---

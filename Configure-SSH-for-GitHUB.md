# Configure SSH for GitHUB

This guide shows how to set up SSH for GitHub on macOS in a compact, classic way.

---

## 1. Check existing SSH keys

```bash
ls -al ~/.ssh
```
If you see id_ed25519.pub or id_rsa.pub, you may reuse them. Otherwise, create a new key.

## create new ssh keys

Recommended (Ed25519):
```bash
ssh-keygen -t ed25519 -C "your-github-email@example.com" -f id_yourkey
```
Fallback (older version of mac os)
```bash
ssh-keygen -t rsa -b 4096 -C "your-github-email@example.com" -f id_yourkey
````


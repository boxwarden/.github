<p align="center">
  <img src="https://boxwarden.sh/brand/boxwarden-512.png" width="96" alt="Boxwarden">
</p>

<h3 align="center">Know what's open on your server before someone else does.</h3>

<p align="center">
  <a href="https://boxwarden.sh">boxwarden.sh</a> ·
  <a href="https://app.boxwarden.sh">Dashboard</a> ·
  <a href="https://github.com/boxwarden/agent">Agent</a>
</p>

---

Boxwarden watches a VPS for the boring things that get it hacked: SSH that takes passwords,
a database Docker quietly published past the firewall, packages with known exploits, and the
quiet signs of a break-in — a new user, a cron job, a process running from `/tmp`.

A small open-source agent checks the server every 15 minutes and sends critical findings to
Telegram, each with the command that fixes it.

**Why you can let it run as root**

- **Read-only.** It never changes your system; every fix is a command you run yourself.
- **No open ports.** It only connects out. The service cannot send it commands.
- **Findings only.** No files, logs or secrets leave the server.
- **Open source.** The agent is [AGPL-3.0](https://github.com/boxwarden/agent/blob/main/LICENSE): read every line, or run it without an account.
- **Verifiable releases.** Built by GitHub Actions from a tag, with signed provenance:
  `gh attestation verify boxwarden-linux-amd64 --repo boxwarden/agent`

**Try it**

Sign in at [app.boxwarden.sh](https://app.boxwarden.sh), add a server and paste the one-line
install as root. Free during beta. Ubuntu and Debian.

Found a vulnerability? Please report it privately — see [SECURITY.md](https://github.com/boxwarden/agent/blob/main/SECURITY.md).

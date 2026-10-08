# MangoSSH feedback

This is where bugs, feature requests and questions go for all four Mango products.

There is **no code in this repository**. The products are closed-source and
their repositories are private; this one exists so the conversation about them
can be public — so you can see whether something is already reported before
writing it out again, and add your vote to what you want next.

## The products

| | |
|---|---|
| **[MangoSSH](https://mangossh.com/)** | SSH, RDP, VNC and SFTP hosts side by side, with an encrypted vault, an audit log, and an MCP server your AI tools can drive. Windows, macOS and Linux. |
| **[MangoDock](https://mangossh.com/products/mangodock)** | Docker management with nothing on the hosts. Reaches each daemon over an ordinary SSH session — no agent to install, no port to open. |
| **[MangoFly](https://mangossh.com/products/mangofly)** | A self-hosted WireGuard mesh. Devices connect straight to each other; the coordination server is one binary and a SQLite file, and never sees their traffic. |
| **[MangoWiFi](https://mangossh.com/products/mangowifi)** | A Wi-Fi 6/7/8 test bench. One binary runs as Console or Agent either side of the access point under test, measuring latency under real load. |

Downloads and documentation are at **[mangossh.com](https://mangossh.com/)**.

## Where to put things

**[Issues](../../issues)** — something is broken, or something is missing.
Use the templates; they ask for the version and platform because without
those most bugs cannot be reproduced.

**[Discussions](../../discussions)** — anything that isn't a defect:

- **Q&A** — "how do I…", "is this supposed to…"
- **Ideas** — a feature you want. Others can vote, and that ordering is what
  gets built next.
- **Show and tell** — what you built with it, what your setup looks like.

**Security** — please **do not** open an issue. Email
**contact@mangossh.com** instead, and give me a reasonable window to fix it
before it's public.

## A good bug report

The version, the platform, what you did, what happened, what you expected.
That's it — but all five, because a report missing one of them usually ends
in a round trip that costs us both a day.

- **Version** — Settings → About, or the installer filename
- **Platform** — Windows / macOS / Linux, and which distribution
- **How you're connecting** — SSH, RDP, VNC, SFTP, serial; socket, SSH or TLS
  for MangoDock
- **Logs**, if the app produced any — but **read them first**. Hostnames,
  usernames, IPs and keys turn up in logs more often than people expect, and
  this is a public repository. Redact before you paste.

## What to expect

This is built by a small team, and most of what gets fixed next is whatever
somebody took the trouble to report. There is no support SLA on the free
tier — I read everything, I reply to most things, and I'll tell you plainly
if something isn't going to get built.

Companies with a paid licence get support by email; that's on the pricing
section of each product page.

## Things worth knowing before you file

- **The installers aren't code-signed yet.** Windows SmartScreen and macOS
  Gatekeeper will both warn you. That's expected, not a bug — the
  [download section](https://mangossh.com/#download) explains how to get
  past each one. Code signing is in progress.
- **macOS is currently a version behind** the Windows and Linux builds.
- **Nothing in any of these products phones home.** No telemetry, no
  analytics, no crash reporter, no account. That also means nothing reports a
  crash for you — if it breaks, this is the only way I'll hear about it.

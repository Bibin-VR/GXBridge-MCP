# GXBridge — control Mitsubishi GX Works3 & your PLC with AI

**GXBridge turns Mitsubishi GX Works3 and a connected PLC into something you can simply talk to.**
It's a Model Context Protocol (MCP) server, so Claude — or any AI agent that speaks MCP — can open
projects, write and build logic, read and write live device values, and download to the PLC, all from
plain natural language.

No more clicking through menus and dialogs for routine engineering work. You describe the outcome; the
agent drives the software and the PLC for you.

---

## What you can do — just by asking

> *"Open my conveyor project and list all the program blocks and global labels."*

> *"Write a Structured Text program: run the motor on Y0 when X0 is on and X1 is off, then build it."*

> *"Read D100, and monitor X0–X7 and Y0–Y7 live while I test the panel."*

> *"Compare this project against last week's backup and tell me what changed."*

> *"Download the program to the PLC."* *(safety-gated — it asks you to confirm first)*

The agent translates each request into the right engineering operations and reports back what happened.

---

## Capabilities at a glance

- **Projects** — open, create, save, rename, verify against another project, even change the target CPU.
- **Program authoring** — write logic in **Ladder, Structured Text, FBD, or SFC**; build and rebuild.
- **Explore a project** — list POUs, structured data types, and labels with their data types and
  device assignments.
- **Objects & libraries** — export, rename, or delete individual blocks; package and reuse libraries.
- **PLC communication** — check online status, run/stop, download to the PLC, upload from the PLC, and
  start live monitoring.
- **Live device I/O** — read and write real device values (D, M, X, Y, …) and watch them update in
  real time.

Dozens of fine-grained operations, all exposed as clean, well-described tools your agent can pick from.

---

## Every programming mode, the way you prefer

Whether your team works in **Ladder Diagram**, **Structured Text**, **Function Block Diagram**, or
**SFC**, GXBridge can create projects in that language and author logic for it — so AI assistance fits
naturally into how you already engineer.

---

## Works with your tools — locally or from anywhere

GXBridge connects to **Claude Code, Claude Desktop, Cursor, Cline, Windsurf**, and any other MCP-capable
agent. It runs right next to GX Works3 on the engineering PC, and can also be reached **securely over the
network** — so you can drive the PLC bench from your laptop while the heavy lifting happens on the
machine that has the software.

---

## Safe by design

GXBridge is built for real equipment. Operations that affect a live PLC or change a project —
downloading, run/stop, deleting, overwriting — **require an explicit confirmation** before they run, so
the agent can move fast on the safe stuff and never surprise you on the rest.

---

## Why it matters

Industrial engineering tools are powerful but slow to operate by hand. GXBridge puts a capable AI in the
driver's seat of that power: faster iteration, fewer repetitive clicks, easier onboarding, and a natural
way to inspect, author, and test PLC programs — without giving up control or safety.

*GXBridge bridges Mitsubishi GX Works3 and MX Component to the world of AI agents.*

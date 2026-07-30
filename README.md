# GXBridge — GX Works3 + PLC bridge for AI agents

**GXBridge turns Mitsubishi GX Works3 and a connected PLC into something you can simply talk to.**
It's a production-quality Model Context Protocol (MCP) server, so Claude — or any AI agent that
speaks MCP — can open projects, write and build logic, download to the PLC, run/stop it, and
read, write, and monitor live device values, all from plain natural language.

All Mitsubishi COM access is isolated inside a reusable bridge library; the MCP server itself is a
thin, COM-free layer on top of it.

```
  Claude / Cursor / Cline / any MCP agent
        │  MCP (stdio or Streamable HTTP)
        ▼
  GXBridge MCP Server      ── exposes 46 tools; no COM here
        │  in-proc calls
        ▼
  GXBridge bridge library  ── all COM isolated here
        │  COM / interop
        ▼
  GX Works3 Open I/F  +  MX Component  →  PLC (e.g. FX5U)
```

## What you can do — just by asking

> *"Open my conveyor project and list all the program blocks and global labels."*

> *"Write a Structured Text program: run the motor on Y0 when X0 is on and X1 is off, then build it."*

> *"Read D100, and monitor X0–X7 and Y0–Y7 live while I test the panel."*

> *"Compare this project against last week's backup and tell me what changed."*

> *"Download the program to the PLC."* — destructive operations require an explicit confirmation first.

## Tool surface — 46 tools

| Area | Covers |
|---|---|
| Sessions | Open, close, list open projects |
| Project ops | Save, save-as, rename, delete, verify, change PLC type |
| Build | Build, rebuild |
| Authoring | Create projects in Ladder, Structured Text, FBD, or SFC; author ST programs |
| Inspection | List POUs, structured data types, global label lists, exported object details |
| Objects & libraries | Export, rename, delete objects; export, register, delete libraries |
| PLCopen XML | Export / import, including graphical layout |
| Download / run | Get download files, download, upload, run, stop |
| Communication | Online status, live monitoring, simulator control |
| Devices (MX Component) | Status, read / write / monitor live device values |

Destructive operations — download, run/stop, delete, overwrite — require an explicit confirmation
before they execute.

## Remote engineering over SSH

GX Works3 only runs on Windows. GXBridge supports driving it from any Mac, Linux, or other Windows
machine over SSH: one host process on the Windows PC owns the GX Works3 engine and its visible
window, while every connected agent — local or remote — shares that single engine instead of
spawning its own. No open ports, no token; SSH does the authenticating. A Streamable HTTP mode with
bearer-token auth is also available for network deployments.

## Every programming mode

Whether your team works in **Ladder Diagram**, **Structured Text**, **Function Block Diagram**, or
**SFC**, GXBridge creates projects in that language and authors logic for it — so AI assistance fits
naturally into how you already engineer.

## Why it matters

Industrial engineering tools are powerful but slow to operate by hand. GXBridge puts a capable AI in
the driver's seat of that power: faster iteration, fewer repetitive clicks, easier onboarding, and a
natural way to inspect, author, and test PLC programs — without giving up control or safety.

---

<sub>GXBridge is proprietary. This repository is an overview; the source is not public.</sub>

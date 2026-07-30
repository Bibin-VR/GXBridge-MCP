# GXBridge

**Control Mitsubishi GX Works3 and your PLC with AI.**

GXBridge is a Model Context Protocol (MCP) server for Mitsubishi GX Works3. It lets
Claude — or any MCP-capable agent — open projects, write and build logic, read and
write live device values, and download to the PLC, all from plain natural language.

Routine engineering work no longer means clicking through menus and dialogs. You
describe the outcome; the agent drives the software and the PLC.

---

## What you can ask for

> *"Open my conveyor project and list all the program blocks and global labels."*

> *"Write a Structured Text program: run the motor on Y0 when X0 is on and X1 is off, then build it."*

> *"Read D100, and monitor X0–X7 and Y0–Y7 live while I test the panel."*

> *"Compare this project against last week's backup and tell me what changed."*

> *"Download the program to the PLC."* — safety-gated; it asks you to confirm first.

The agent translates each request into the right engineering operations and reports
back what happened.

## Capabilities

| Area | What it covers |
|---|---|
| **Projects** | Open, create, save, rename, verify against another project, change the target CPU |
| **Program authoring** | Write logic in Ladder, Structured Text, FBD, or SFC; build and rebuild |
| **Project exploration** | List POUs, structured data types, and labels with their data types and device assignments |
| **Objects & libraries** | Export, rename, or delete individual blocks; package and reuse libraries |
| **PLC communication** | Check online status, run/stop, download to the PLC, upload from the PLC, start live monitoring |
| **Live device I/O** | Read and write real device values (D, M, X, Y, …) and watch them update in real time |

Dozens of fine-grained operations, each exposed as a clearly described tool the
agent can select from.

## Every programming mode

Whether your team works in **Ladder Diagram**, **Structured Text**, **Function Block
Diagram**, or **SFC**, GXBridge can create projects in that language and author logic
for it — so AI assistance fits how you already engineer.

## Works with your tools, locally or remotely

GXBridge connects to **Claude Code, Claude Desktop, Cursor, Cline, Windsurf**, and any
other MCP-capable agent. It runs next to GX Works3 on the engineering PC and can also
be reached securely over the network — so you can drive the PLC bench from your laptop
while the heavy lifting happens on the machine that has the software installed.

## Safe by design

GXBridge is built for real equipment. Any operation that affects a live PLC or changes
a project — downloading, run/stop, deleting, overwriting — **requires explicit
confirmation** before it runs. The agent moves fast on the safe operations and never
surprises you on the rest.

## Why it matters

Industrial engineering tools are powerful but slow to operate by hand. GXBridge puts a
capable AI in the driver's seat of that power: faster iteration, fewer repetitive
clicks, easier onboarding, and a natural way to inspect, author, and test PLC programs
— without giving up control or safety.

---

<sub>GXBridge bridges Mitsubishi GX Works3 and MX Component to the world of AI agents.</sub>

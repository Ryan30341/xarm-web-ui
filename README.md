# xArm Web UI

Production-deployed chemist-facing web application for the xArm robotic arm system.

## Overview

This repo is the frontend + API server for the xArm Web Interface project. It is developed and deployed from [Replit](https://replit.com) and serves as a submodule of the parent [`xarm-web-interface`](https://github.com/Ryan30341/xarm-web-interface) repo.

## Features (planned)

- **Voice-first chat interface** — OpenAI Realtime API with GPT-4o function calling
- **Skills browser** — searchable catalog of xArm skills (stir, pick-and-place, dispense, etc.)
- **Live telemetry** — joint state, arm status, 3D URDF preview via three.js
- **Camera pane** — WebRTC stream from the Intel RealSense D435i
- **Skill execution** — voice or manual trigger → REST call to the Linux ROS 2 bridge

## Stack

- React + Vite (frontend)
- Express 5 (API server)
- PostgreSQL + Drizzle ORM (skills database)
- OpenAI Realtime API (voice + function calling)
- Clerk (authentication)
- pnpm monorepo

## Development

This project is developed on Replit. Clone and open in Replit, or run locally:

```bash
pnpm install
pnpm --filter @workspace/api-server run dev
```

## Part of

[`xarm-web-interface`](https://github.com/Ryan30341/xarm-web-interface) — umbrella repo for the full system.

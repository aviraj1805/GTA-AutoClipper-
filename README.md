# GTA Clipping Toolkit

A local toolkit for making vertical GTA gameplay clips and optionally scheduling reviewed clips to social accounts.

## Components

- [`GTA-Auto-Clipper/`](GTA-Auto-Clipper/README.md): source code from [AnIntellectualBeing/GTA-Auto-Clipper](https://github.com/AnIntellectualBeing/GTA-Auto-Clipper), distributed under the MIT license included in that folder. Promotional website assets, payment-site code, paid guide PDFs, and paid prompt packs are omitted.
- [`GTA-Auto-Sender/`](https://github.com/AnIntellectualBeing/GTA-Auto-Sender): linked as a Git submodule so its source remains in the upstream repository.

## Setup

1. Clone this project with its sender reference: `git clone --recurse-submodules https://github.com/aviraj1805/GTA-AutoClipper-.git`.
2. Follow `GTA-Auto-Clipper/README.md` to install Python dependencies and FFmpeg. Keep the YouTube API key in a private environment variable.
3. Set up the sender from its upstream README. Copy `.env.example` to `.env` and `config/channels.example.json` to `config/channels.json`; fill those local files only. They contain credentials and account IDs and must not be committed.
4. Run the sender's dry runs before enabling scheduled posting. Review every clip and use only source footage you are permitted to reuse.

## Private/runtime files

Credentials, API keys, channel IDs, local queues, captured or reviewed videos, generated clips, model caches, and virtual environments are intentionally excluded. The root `.gitignore` protects common local runtime files.

The sender is an upstream submodule rather than copied source. This repository does not assert a license for the sender; consult its owner for redistribution rights.

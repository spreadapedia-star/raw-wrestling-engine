# RAW-Style Wrestling Engine — Project Specification

Status: planning baseline; no playable implementation yet.

## Goal
Build a standalone Windows 10/11 wrestling game with the same 16-bit pixel-art visual style, wrestler proportions, ring perspective, animation timing, and gameplay feel as SNES WWF Raw (1994). This project is separate from existing SNES ROM hacks.

## Platform
- Windows first; investigate SNES cartridge adaptation later.
- Internal rendering target: 256 x 224, nearest-neighbor integer scaling.
- Fixed-step 60 Hz simulation target; verify original mechanics through measurement rather than assumption.
- Local keyboard and controller input; two-player gameplay target for initial prototype.

## Gameplay fidelity
Reconstruct movement, strikes, grapples, reversals, throws, damage, stamina/recovery, ropes, pins, AI and win conditions through documented reference tests. Avoid claiming frame-perfect parity without tests.

## Content pipeline
Data-driven wrestlers, sprite sheets, animation timelines, move definitions, sound cues, and arenas. New wrestlers should not require custom engine code for standard moves.

## First playable milestone
Two wrestlers, one ring, one complete match, input, collision, grapples, attacks, knockdowns, pins, AI and match end. Build and run on Windows.

## Scope guardrails
No ROMs, copyrighted game assets or proprietary source files committed to this public repository. Keep extracted/reference assets local unless distribution rights are established.

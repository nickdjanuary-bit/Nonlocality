# SNATCHER (1994 US Sega CD) — Autonomous One-Prompt Native-Port Benchmark

The original Sega CD SNATCHER disc image is located at `input/snatcher.iso` in this private workspace. You have REA, Ghidra, and native Linux development tools. Independently analyze the original game and produce a playable native-Linux PC port that loads the user's original disc image at runtime. Attempt the entire game, not just an intro screen or static mock-up.

Work autonomously. Investigate the game program, its 68000 architecture, Sega CD hardware/BIOS dependencies, data and scenario formats, graphics, inputs, CD audio, and timing. Write executable source and build instructions, run the port, test observable behavior, and save logs and evidence. When required, debug and revise. Do not substitute a video recording or preauthored walkthrough for actual executable gameplay. Do not consult any existing DART source recovery, prior disassembly, BIOS maps, walkthroughs, port code, or benchmark findings; this is an independent one-prompt experiment.

Preserve original game instructions and data where feasible rather than simply rewriting the narrative. Describe any emulation layers or behavioral replacements precisely. Never fabricate progress or test results. If you cannot finish, deliver the best *executed and verified* checkpoint, with the exact blocker and working evidence. Do not publish or embed game assets in the generated project; the launcher must load the user's own disc image locally at runtime.

Place all new output in `output/`, including buildable source, executable if obtained, reproducible launch commands, test logs, and `RESULT.md` that clearly states completed, partial, or failed. This is one instruction; proceed without further questions.

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A content repository for the LinkedIn post series **"Because running VSLAM is fun"** — documenting real-world experiments with Visual SLAM systems run through [VSLAMLAB](https://github.com/VSLAM-LAB/VSLAM-LAB).

## Repository structure

Posts live in `posts/` as plain UTF-8 text files with no extension, named `because_running_VSLAM_is_fun_<series>_<episode>` (e.g. `1_0`, `1_1`, …). Each post is a self-contained LinkedIn draft including the body text, video links, acknowledgements, and hashtags.

## Tooling

The repo uses [pixi](https://pixi.sh) for environment management (`pixi.toml`). The `pixi.lock` file is treated as a binary (see `.gitattributes`) to avoid merge conflicts. Currently no pixi tasks or dependencies are defined in this repo — the `pixi run` commands referenced inside post drafts (e.g. `pixi run demo allfeature-dev videos GX010216`) belong to the VSLAMLAB project, not this one.

## Post content conventions

- Each post opens with the series title and episode number: `Because running VSLAM is fun (1.X) 📷🧭📍`
- Body covers: dataset/location, VSLAM systems used (AllFeature-VSLAM, DROID-SLAM, MASt3R-SLAM), feature types coupled (ORB, ALIKED, SuperPoint, SIFT), and the single reproducibility command
- Ends with acknowledgements, cross-links to adjacent posts (`Next Post` / `Previous Post`), and a hashtag block

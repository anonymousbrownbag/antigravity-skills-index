---
name: opus-agent-skills
description: "Prompt engineering and content strategy for automated Agent Opus video generation"
risk: safe
source: "Agent Opus Prompt Guide"
date_added: "2026-03-12"
---

# Opus Agent Skills

## Overview

Content creation strategy and prompt engineering specifically optimized for Agent Opus video generation workflows. This skill bridges the gap between raw input data—such as scraped articles or automation pipeline outputs—and high-quality, narrative-style video prompts.

## When to Use This Skill

Use this skill when you need to construct effective text instructions for Agent Opus to generate videos, particularly for explainer, thought leadership, news, or promotional content formats.

## Instructions

As the Opus Agent, your primary function is to process input text, URLs, and asset references to output a highly structured, directly executable prompt for Agent Opus. Follow these core guidelines to ensure maximum output quality:

**1. Be Clear and Specific**
* Define the video's scope, target audience, and desired style or tone immediately.
* *Implementation:* Always state the desired outcome upfront (e.g., "Create an informative 60-second explainer video about [Topic] targeting [Audience] with a [Tone] tone.").

**2. Provide Necessary Context & Sources**
* Include relevant background information and overarching goals.
* Directly embed source URLs or the full extracted text to ground the video's facts. Since Agent Opus cannot pull from paywalls, rely on the scraped text summaries provided in your input.

**3. Script Integration**
* Generate and provide a complete, well-rounded script. Agent Opus produces the best results when it turns a precise written script into voiced narration rather than generating the narrative from scratch.

**4. Asset Referencing**
* When incorporating downloaded media, user files, or URLs, refer to them explicitly using the `@` symbol (e.g., `@headline_screenshot.png` or `@audio_file.mp3`).
* Describe the exact role of the asset in the prompt rather than just stating its existence (e.g., "Display `@chart.png` while the narrator explains the data trends").

**5. Strict Constraints**
* **Do NOT** instruct Agent Opus to add animated captions to raw videos or clip long videos into shorts (these are OpusClip functions).
* **Do NOT** describe specific logos, fonts, or color palettes in the text prompt; assume custom branding is handled via manual asset uploads.

**Standard Output Structure:**
When finalizing your prompt generation, organize the output into clear sections:
* **Role & Context**
* **Source Material**
* **Asset Instructions** * **Narration Script**
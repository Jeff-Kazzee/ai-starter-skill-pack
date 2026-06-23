# Claude Website Prompt

Copy/paste this into Claude when you want it to build the Astro website.

```text
You are working in this repo:
C:\Users\jeffk\dev\AI Beginner SKills\ai-starter-skill-pack

Goal:
Build the Astro website for AI Starter Skill Pack and prepare it for GitHub Pages. This is a public open-source skill pack for beginners who need a calm, practical way into AI: onboarding, prompt debugging, tutoring, project ideas, and career proof.

Important repo truth:
- Default development branch: dev.
- Production branch: prod currently matches the verified baseline.
- GitHub Pages is live from the gh-pages branch, path /.
- Live URL: https://jeff-kazzee.github.io/ai-starter-skill-pack/
- Repo URL: https://github.com/Jeff-Kazzee/ai-starter-skill-pack
- Root package.json is a data-package manifest for installing the skills from GitHub. Do not turn the repo root into the Astro app if that would blur the package boundary.
- Keep package.json "files" focused on skills/ and shared/ unless Jeff explicitly asks otherwise.
- Do not include post/ or RESEARCH-DIGEST.md in the public site or package.

Build shape:
- Create the Astro app under site/ so the root repo can remain an installable skill package.
- Configure Astro for GitHub Pages project hosting:
  - site: "https://jeff-kazzee.github.io"
  - base: "/ai-starter-skill-pack"
- Use the generated assets:
  - assets/ai-starter-skill-pack-hero.png (1672 x 941): homepage hero or wide visual lead.
  - assets/ai-starter-skill-pack-social.png (1731 x 909): README/social/Open Graph/package section.
- Use docs/STATS.md as the baseline stats source.
- Keep docs/CLAUDE-WEBSITE-PROMPT.md and assets/README.md as handoff/reference docs.

Site content requirements:
- First viewport should immediately show the product: "AI Starter Skill Pack", one clear sentence, the hero asset, and two direct actions:
  - View skills on GitHub
  - Install from GitHub
- Include the install command:
  npm install github:Jeff-Kazzee/ai-starter-skill-pack
- Explain that installs expose:
  node_modules/ai-starter-skill-pack/skills/
  node_modules/ai-starter-skill-pack/shared/
- Show the five skills as practical modules:
  - ai-beginner-onboarding: calm first setup, seven-day plan, first workflow, practice project
  - prompt-debugger: diagnose failed prompts, rewrite, variants, test cases
  - personal-ai-tutor: learning path, milestones, proof artifacts, review checkpoints
  - ai-project-idea: ranked small projects, scoped MVP, seven-day build plan
  - no-bs-ai-career: honest claims, gap analysis, portfolio proof, 30-day plan
- Include a compact stats section:
  - 5 skills
  - 5 eval query sets
  - 5 manual test READMEs
  - 45.7 KB dry-run package
  - 130.2 KB unpacked
- Include a section that says the package ships skills/shared only, while website/README imagery stays as repo assets.
- Include a footer with GitHub repo link and Pages URL.

Design direction:
- Practical, beginner-safe, calm, confident.
- Use the assets as real visual anchors, not tiny decorative thumbnails.
- Use a balanced palette: fresh green, sky blue, coral, graphite, off-white.
- Avoid dominant purple gradients, beige-only pages, dark slate monotone, floating orb decoration, generic AI neon, and fake code screenshots.
- Cards can be used for the five skill modules, but keep radius <= 8px and avoid cards inside cards.
- No in-app explanatory filler about how to use the website. The site should be self-evident.
- Mobile must be polished: no overlapping text, no cropped CTA text, images with stable responsive dimensions.

Tests/verification before finishing:
1. From repo root, run npm run pack:check and confirm the package still contains only skills/shared plus normal package metadata.
2. From site/, run npm install if needed, then npm run build.
3. Preview the built site locally if possible and inspect desktop and mobile.
4. Verify the generated site respects the GitHub Pages base path /ai-starter-skill-pack.
5. Deploy by copying site/dist contents into the gh-pages worktree:
   C:\Users\jeffk\dev\AI Beginner SKills\ai-starter-skill-pack-gh-pages
   Then commit and push gh-pages.
6. After deploy, curl or open:
   https://jeff-kazzee.github.io/ai-starter-skill-pack/
7. Update docs/STATS.md if counts, package size, or deployment facts change.

Deliverables:
- Astro site in site/.
- Updated gh-pages branch with built static output.
- README.md may be refined, but keep it useful for GitHub and npm-style installs.
- Final response should include the live URL, files changed, and verification commands/results.
```

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a documentation and template repository containing GitHub profile setup templates and guides. It contains:

- `duong-github-profile.md`: Complete GitHub profile README template with markdown code
- `github.txt`: Detailed Vietnamese instructions for setting up GitHub profiles and GitHub Actions
- `github_profiles_dep_nhat.txt`: Comprehensive list of 80+ curated GitHub profile resources, tools, and inspiration
- `1.gif`: Visual asset for templates
- Template includes modern GitHub profile features: stats widgets, skill icons, contribution snake animation, typing effects

## Repository Structure

This is a documentation/template repository, not an active development project:
- No package managers or dependency files
- No source code or build tools
- No testing frameworks
- Not initialized as a git repository

## File Contents

### duong-github-profile.md
- Complete ready-to-use GitHub profile template
- Includes: header animation, typing effect, GitHub stats, tech stack showcase, contribution snake
- JavaScript-style bio section for personality
- Multiple widget integrations (Spotify, WakaTime, activity graph)
- Social media badges and links section

### github.txt
- Vietnamese step-by-step setup guide
- GitHub Actions configuration for automated updates
- Snake animation setup (using Platane/snk)
- Spotify and WakaTime integration instructions
- Theme customization guide
- Troubleshooting section for common issues

### github_profiles_dep_nhat.txt
- Curated collection of 80+ GitHub profile resources
- 10 main categories: awesome lists, notable profiles, generators, tools, tutorials
- API endpoints for stats, streaks, trophies
- Vietnamese and English resources
- Markdown and image editing tools

## Working with Templates

When modifying the GitHub profile templates:
- The template uses username `duong` as placeholder - replace with actual GitHub username
- Template includes various widgets that require GitHub Actions setup
- Color scheme uses cyan blue (#00D9FF) with GitHub dark theme (#0D1117)
- All URLs and usernames must be updated consistently across the template
- Contains both Vietnamese and English documentation

## GitHub Actions Setup

The templates require GitHub Actions for dynamic features:

**Snake Animation** (github.txt:27-57):
- Create `.github/workflows/snake.yml`
- Runs every 6 hours via cron schedule
- Uses Platane/snk@v2 for snake generation
- Outputs to separate branch named `output`

**WakaTime Stats** (github.txt:65-86):
- Requires WakaTime API key in repository secrets
- Create `.github/workflows/wakatime.yml`
- Updates daily with coding time statistics

## Widget URLs & APIs

Key API endpoints used in templates:
- GitHub Stats: `https://github-readme-stats.vercel.app/api?username={USERNAME}`
- Streak Stats: `https://github-readme-streak-stats.herokuapp.com/?user={USERNAME}`
- Top Languages: `https://github-readme-stats.vercel.app/api/top-langs/?username={USERNAME}`
- Skill Icons: `https://skillicons.dev/icons?i={ICON_NAMES}`
- Typing SVG: `https://readme-typing-svg.herokuapp.com`
- Capsule Render: `https://capsule-render.vercel.app/api`

## Common Tasks

To use these templates:
1. Copy markdown from `duong-github-profile.md`
2. Create new GitHub repository with same name as username (e.g., if username is `johndoe`, repo must be named `johndoe`)
3. Replace all instances of placeholder username `duong` with actual GitHub username
4. Update personal information: email, LinkedIn, Twitter, website links
5. Set up GitHub Actions workflows from `github.txt` for automated features
6. Customize color scheme by replacing hex codes if desired
7. Add API keys to repository secrets for optional integrations (Spotify, WakaTime)
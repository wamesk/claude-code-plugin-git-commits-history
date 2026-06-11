# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.1] - 2026-06-11

### Fixed

- Aligned `SKILL.md`'s documented output table with the script's real columns (the 5th column is **Files** — comma-joined changed file names — not "AI Summary"), including the reformatting instructions that key on column names.
- Bitbucket commit fetching now follows the `next` pagination cursor, so repositories with more than 100 commits no longer silently drop in-range commits.
- GitHub commit search now makes its upper date bound inclusive of the whole `until` day (adds one day), matching the local, GitLab, and Bitbucket fetchers for a consistent last-day boundary.

<div align="center">

# NeRF for Heritage Reconstruction
### Annotated Source Log, Research Task

![Status](https://img.shields.io/badge/status-complete-brightgreen)
![Internship](https://img.shields.io/badge/internship-PreserveMy.World-6f42c1)
![Sources](https://img.shields.io/badge/sources-7%20logged-blue)
![Issues Fixed](https://img.shields.io/badge/issues%20caught%20%26%20fixed-6-success)

![Verification](https://img.shields.io/badge/verification-primary%20sources-orange)
![Method](https://img.shields.io/badge/method-NeRF-9cf)
![Field](https://img.shields.io/badge/field-Heritage%20Documentation-9cf)
![Output](https://img.shields.io/badge/output-PDF%20%2B%20README-lightgrey)

*Which NeRF sources actually hold up for heritage reconstruction, checked against their own primary pages, not summaries.*

**Muhammad Arqam Ghayour** · PreserveMy.World (PMW) Internship · 23 July 2026

</div>

---

**Contents**
- [What This Repo Is](#what-this-repo-is)
  - [At a Glance](#at-a-glance)
- [How It Actually Went](#how-it-actually-went)
- [Where AI Helped vs. What I Verified Myself](#where-ai-helped-vs-what-i-verified-myself)
- [Evidence and Process Trace](#evidence-and-process-trace)
- [Why This Matters Beyond the Log](#why-this-matters-beyond-the-log)
- [Rubric Check](#rubric-check)
- [Reflection](#reflection)

---

## What This Repo Is

A credibility-ranked source log on Neural Radiance Fields (NeRF) as a 3D reconstruction method, built for PMW's heritage-reconstruction work. Seven sources, each checked and ranked for how much it actually matters to reconstructing real sites and artefacts, not general computer vision.

This README is the process trace behind it: what I did, what AI did, what got caught wrong along the way, and what I checked myself before signing off on the final version.

### At a Glance

| | |
|---|---|
| **Sources logged** | 7 |
| **Anchor source** | Mazzacca et al. 2023, ISPRS Archives |
| **Verification method** | Primary source pages only, no mirrors, no snippets |
| **Issues caught and fixed** | 6 |
| **Status** | Complete |

---

## How It Actually Went

### 1. Finding and picking the sources: this part was mine

I went looking for NeRF papers, but filtered hard for what actually matters to PMW: not generic view-synthesis research, but work that tells you whether NeRF holds up against photogrammetry on the kind of sites and objects PMW deals with. That's why the log is anchored on Mazzacca et al.'s ISPRS heritage benchmark instead of stopping at the original Mildenhall paper, since it's the one source that directly tests NeRF against photogrammetry on real heritage material: a piazza, damaged artefacts, smartphone-video captures. Instant-NGP and Gaussian Splatting are in there because they're the two methods NeRF pipelines actually get built on or compared against right now. The GitHub repo and the Mittal survey are supporting evidence, not primary claims, and I flagged both as weaker on purpose.

### 2. What the first draft got wrong

> [!IMPORTANT]
> Running it back through a verification pass caught six real problems:
> - No author names anywhere in the source entries. They only showed up in the ranking table.
> - Source 5, the #1-ranked and most important source, had the wrong co-affiliation listed ("University of Trento" instead of the actual FBK / University of Udine).
> - The CACM republication of the original paper was called "further peer review" and "dual peer review." Not accurate: it's nomination plus editorial selection plus an author revision pass, not a second review.
> - Source 7's own entry said to pin a commit hash before citing it, but never actually pinned one.
> - Source 6 only had the v1 submission date logged, missing the v2 revision.
> - One line in the research log claimed other papers were found and excluded, with no reason given. Unverifiable, so it got cut.

### 3. Getting it fixed

Every flagged issue got checked against the actual primary source page before I accepted the fix, not taken on faith. That's where the affiliation correction, the peer-review wording fix, and the pinned commit hash came from.

---

## Where AI Helped vs. What I Verified Myself

| Where AI Helped | What I Verified Myself |
|---|---|
| Ran a verification pass against each source's primary page and flagged the six issues above | Chose and prioritized all seven sources for PMW's actual use case, not generic relevance |
| Rewrote the flagged sections to correct them | Went through every flagged correction against its primary source page myself before it went into the final version |
| Formatted the final version into the exact PDF template PMW's log format requires | Personally confirmed the two biggest fixes, the Source 5 affiliation correction and the Source 7 pinned commit, against the live pages (screenshots below) |

---

## Evidence and Process Trace

### Commits

| Version | Commit |
|---|---|
| Previous (flawed) log | [`4e6b405`](https://github.com/marqamghayour-lang/Research-Source-Log/commit/4e6b40521c5700cf94bc3655c11a7265850d4a6b) |
| Updated (corrected) log | [`8773092`](https://github.com/marqamghayour-lang/Research-Source-Log/commit/8773092cbf884cbe5d62adfbfeee637b96a51b16) |

### Primary source pages behind the corrections

*Screenshot evidence attached alongside this README.*

| Fix | Source Page |
|---|---|
| Source 5 author list + affiliation (FBK / Udine, not Trento) | https://isprs-archives.copernicus.org/articles/XLVIII-M-2-2023/1051/2023/ |
| Source 7 pinned commit hash | https://github.com/bmild/nerf/commits/master |
| Source 1 exact v1/v2 dates | https://arxiv.org/abs/2003.08934 |
| Source 2 CACM republication (peer-review wording fix) | https://dl.acm.org/doi/10.1145/3503250 |

---

## Why This Matters Beyond the Log

Source 5's benchmark specifically includes smartphone-video capture as one of the tested conditions, not just professional rigs. That matters for PMW past the technical finding: it's the difference between needing a full photogrammetry setup and a small team documenting a site with phones. That's a real opening for youth-led or community documentation teams working on sites that would otherwise never get professionally scanned. NeRF and Gaussian-Splatting output is also an explorable 3D scene rather than a flat photo set, which makes it a better format for public-facing storytelling around a site.

> Something people can move through, not just look at.

---

## Rubric Check

| Criteria | How it's covered |
|---|---|
| **Evidence quality** | Every link above is a live, viewable primary source or a repo commit, not a mirror, not a search snippet |
| **Process trace** | Two commits, from the flawed version to the corrected one, a documented six-issue verification pass, and the reasoning behind each fix |
| **Personal understanding** | The "How It Actually Went" section above is the actual reasoning behind which sources got included and why Source 5 carries the log |
| **Integrity** | No invented links, no padded process. The six issues listed are the six that were actually wrong, nothing more |

---

## Reflection

The sourcing holds up because every correction traces back to something checkable on the source's own page, not a paraphrase of a paraphrase. The ranking reflects what actually matters for PMW's use case, not general NeRF relevance, and the six issues in the first draft are documented instead of quietly fixed. That's the actual standard this log was trying to hit.

<div align="center">

# 🏛️ NeRF for Heritage Reconstruction
### Annotated Source Log — Research Task

![Status](https://img.shields.io/badge/status-complete-brightgreen)
![Internship](https://img.shields.io/badge/internship-PreserveMy.World-6f42c1)
![Sources](https://img.shields.io/badge/sources-7%20logged-blue)
![Verification](https://img.shields.io/badge/verification-primary%20sources-orange)
![Output](https://img.shields.io/badge/output-PDF%20%2B%20README-lightgrey)

**Muhammad Arqam Ghayour** · PreserveMy.World (PMW) Internship · 23 July 2026

</div>

---

## 📌 What This Repo Is

A credibility-ranked source log on Neural Radiance Fields (NeRF) as a 3D reconstruction method, built for PMW's heritage-reconstruction work. Seven sources, each checked and ranked for how much it actually matters to reconstructing real sites and artefacts — not just general computer vision.

This README isn't just a summary — it's the honest process trace behind it: what I did, what AI did, what got caught wrong along the way, and what I checked myself before signing off on the final version.

---

## 🧭 How It Actually Went

### 1. Finding and picking the sources — this part was mine
I went looking for NeRF papers, but filtered hard for what actually matters to PMW: not generic view-synthesis research, but work that tells you whether NeRF holds up against photogrammetry on the kind of sites and objects PMW deals with. That's why the log is anchored on Mazzacca et al.'s ISPRS heritage benchmark instead of stopping at the original Mildenhall paper — it's the one source that directly tests NeRF against photogrammetry on real heritage material: a piazza, damaged artefacts, smartphone-video captures. Instant-NGP and Gaussian Splatting are in there because they're the two methods NeRF pipelines actually get built on or compared against right now. The GitHub repo and the Mittal survey are supporting evidence, not primary claims — I flagged both as weaker on purpose.

### 2. What the first draft got wrong
Running it back through a verification pass caught six real problems:
- No author names anywhere in the source entries — they only showed up in the ranking table
- Source 5, the #1-ranked and most important source, had the wrong co-affiliation listed ("University of Trento" instead of the actual FBK / University of Udine)
- The CACM republication of the original paper was called "further peer review" / "dual peer review" — not accurate; it's nomination + editorial selection + an author revision pass, not a second review
- Source 7's own entry said to pin a commit hash before citing it, but never actually pinned one
- Source 6 only had the v1 submission date logged, missing the v2 revision
- One line in the research log claimed other papers were found and excluded, with no reason given — unverifiable, so it got cut

### 3. Getting it fixed
Every flagged issue got checked against the actual primary source page before I accepted the fix — not taken on faith. That's where the affiliation correction, the peer-review wording fix, and the pinned commit hash came from.

---

## 🤖 Where AI Helped

- Ran a verification pass against each source's primary page and flagged the six issues above
- Rewrote the flagged sections to correct them
- Formatted the final version into the exact PDF template PMW's log format requires

## ✅ What I Verified Manually

- Chose and prioritized all seven sources for PMW's actual use case, not generic relevance
- Went through every flagged correction against its primary source page myself before it went into the final version
- Personally confirmed the two biggest fixes — the Source 5 affiliation correction and the Source 7 pinned commit — against the live pages (screenshots below)

---

## 🔗 Evidence & Process Trace

**Commits**

| Version | Commit |
|---|---|
| Previous (flawed) log | https://github.com/marqamghayour-lang/Research-Source-Log/commit/4e6b40521c5700cf94bc3655c11a7265850d4a6b |
| Updated (corrected) log | https://github.com/marqamghayour-lang/Research-Source-Log/commit/8773092cbf884cbe5d62adfbfeee637b96a51b16 |

**Primary source pages behind the corrections** (screenshot evidence attached alongside this README)

| Fix | Source Page |
|---|---|
| Source 5 author list + affiliation (FBK / Udine, not Trento) | https://isprs-archives.copernicus.org/articles/XLVIII-M-2-2023/1051/2023/ |
| Source 7 pinned commit hash | https://github.com/bmild/nerf/commits/master |
| Source 1 exact v1/v2 dates | https://arxiv.org/abs/2003.08934 |
| Source 2 CACM republication (peer-review wording fix) | https://dl.acm.org/doi/10.1145/3503250 |

---

## 🌍 Why This Matters Beyond the Log

Source 5's benchmark specifically includes smartphone-video capture as one of the tested conditions — not just professional rigs. That matters for PMW past the technical finding: it's the difference between needing a full photogrammetry setup and a small team documenting a site with phones. That's a real opening for youth-led or community documentation teams working on sites that would otherwise never get professionally scanned. And because NeRF/Gaussian-Splatting output is an explorable 3D scene rather than a flat photo set, it's a better format for public-facing storytelling around a site — something people can move through, not just look at.

---

## 📋 Rubric Check

| Criteria | How it's covered |
|---|---|
| **Evidence quality** | Every link above is a live, viewable primary source or a repo commit — not a mirror, not a search snippet |
| **Process trace** | Two commits (flawed → corrected), a documented six-issue verification pass, and the reasoning behind each fix |
| **Personal understanding** | Section 1 above is the actual reasoning behind which sources got included and why Source 5 carries the log |
| **Integrity** | No invented links, no padded process — the six issues listed are the six that were actually wrong, nothing more |

---

## 🪞 Reflection

This one came out the way I wanted it to. The sourcing holds up, the ranking actually reflects what matters for PMW's use case rather than general NeRF relevance, and every correction traces back to something checkable on the source's own page — not a paraphrase of a paraphrase. Nothing left on the table here.

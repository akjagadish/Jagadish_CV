# CV edits — what changed, what didn't

The 16 `.tex` files in this folder are drop-in replacements for `cv/`. Every edit is listed in `CHANGES.diff`. I only changed things I could verify from your own files or from a source I checked; everything else is in Part B for you to decide.

---

## Part A — Changes made (65 edits)

### Verified facts
| File | Change | Basis |
|---|---|---|
| honors.tex | ICLR 2026 Top Reviewer location `USA` → `Brazil`; `Conference for` → `Conference on`; added `(ICLR)` | ICLR 2026 was in Rio de Janeiro; your NeurIPS entries use conference venue as location |
| organization.tex | `Computation and Cognitive Tübingen Summer School` → `Computation and Cognition Tübingen Summer Internship` | MPI's own program name |
| service.tex | `Psychology Reviews` → `Psychological Review` | matches your service statement |
| supervison.tex | Schubert `[PDF]` link `2402.01821` → `2402.03969` | 2402.01821 is *your* ICML paper (publications.tex L72); Schubert's is 2402.03969 (publications.tex L81) |
| supervison.tex | Lan Pan location `USA` → `Germany` | project is at Osnabrück; column convention elsewhere is institution country |
| selected_publications / working_papers | `Griffiths, T.` → `Griffiths, T. L.` (5×); `Lake, B.` → `Lake, B. M.` (2×) | matches the initials you use for both in conference_proceedings.tex and working_papers.tex |
| publications.tex | `Toward a automated science of the mind  {Neuron}` → `Toward an automated science of the mind. {Neuron}` | matches selected_publications.tex |
| supervison.tex | `Computational Cognitive Neuroscience Conference` → `Conference on Cognitive Computational Neuroscience (CCN)` | word order of CCN |
| conference_proceedings.tex | `Annual Conference Cognitive Computational Neuroscience` → `Annual Conference on Cognitive Computational Neuroscience (CCN)` (2×) | |

### Spelling / typos
- honors.tex: `National Geography Story Tellers` → `National Geographic Storytellers`; `M.Sc in` → `M.Sc. in`; `Ph.D. with Magna cum Laude` → `Ph.D. magna cum laude`
- talks.tex, supervison.tex: `Münich` → `Munich` (2×)
- education.tex, experience.tex: `Ecole Polytechnique Federale` → `École Polytechnique Fédérale` (2×)
- experience.tex: `Twin-cities` → `Twin Cities`
- publications.tex: `Frontiers in psychology` → `Frontiers in Psychology`
- supervison.tex: `Arxiv` → `arXiv`
- funding.tex: `~\$150 dollars` → `\$150`; `from Scully Peretsman Foundation for period of` → `from the Scully Peretsman Foundation for a period of`; removed `Generous` (3×)
- talks.tex: `in the the Princeton AI Lab` → `in the`; `the longest running scientific discussion groups` → `the longest-running scientific discussion group`; `University of California Berkeley` → `University of California, Berkeley`
- working_papers.tex: stray space in `Models .` removed (doubled word left — see B2)
- cv.tex: `\googlescholar{B42Mr-sAAAAJ&hl}` → `\googlescholar{B42Mr-sAAAAJ}` (leftover `&hl` from a copied URL)

### Grammar / punctuation consistency
- `at the Princeton University` → `at Princeton University` (5×); `at the New York University` → `at New York University`
- Missing `\&` before final author: Chandramouli et al., Xie et al.
- Missing serial comma `Binz, M. \& Schulz` → `Binz, M., \& Schulz` (3 files)
- Misplaced year in the "Bounded ecologically rational…" entry moved after authors
- `In 5th Multidisciplinary` → `In the 5th`
- Missing period after title: Cohen et al.
- `Wang, J.X.` → `Wang, J. X.` (2×)
- `In 2016 {IEEE Region 10…}` → `{In 2016 IEEE Region 10…}` (brace placement)
- `*` → `$^*$` for Jagadish/Strittmatter equal-contribution marks (4×), matching the rest of the CV
- position.tex: added `~·~` before "Mentors:" (matches experience.tex style) and serial comma
- supervison.tex: `Research Project` → `Research project`; quoted the Han/Kawaja project title like every other entry
- `Top 10 \%` → `Top 10\%` (4×)

### Quote marks
- All `\"…\"` / mixed `` ``…" `` / `''…''` fixed to `` ``…'' `` or `“…”` consistently: organization.tex (3), press.tex (3), talks.tex (1), teaching.tex (1), supervison.tex (1)
- talks.tex: non-breaking hyphen U+2011 in `In‑context` → regular hyphen
- talks.tex: two `\href{}{…}` with empty URLs unwrapped to plain text (they rendered as dead links)

### Ordering / links
- organization.tex: 2020 Volunteer entry moved above 2019 entry
- organization.tex: `AI for scientific discovery` → `AI for Scientific Discovery` (matches talks.tex and service statement); added colon in `Connecting Minds and Machines: a…`; `CogSci-2024` → `CogSci 2024`
- press.tex: NYT link `http://` → `https://`; Fortune link `?abc123` stripped

---

## Part B — Not changed: needs your decision

### B1. Things that look wrong but I can't resolve
1. **working_papers.tex L32** — `Lake, B. M.$^*$` carries a lone equal-contribution asterisk; the same paper in selected_publications.tex L69 has none. Either remove it or add `$^*$` to a second author.
2. **working_papers.tex L113** — `Language Language Models`: doubled word, but I don't know whether you mean "Large Language Models" or "Language Model Agents". This entry is also the same project as the *published* CogSci paper in conference_proceedings.tex L38. If it's a journal follow-up, say so; if not, delete it.
3. **publications.tex L42–44** — Cohen et al. dated 2025, but the PMLR URL is `v320/cohen26a`, which suggests 2026.
4. **publications.tex L88** — Ben-Zion et al. dated 2024 in *npj Digital Medicine*, but the NYT, Fortune, and ScienceDaily coverage of it are all dated March 2025. Check the journal publication year.
5. **press.tex L15** — "An opinion piece": the URL is under `/science/`, not `/opinion/`. Likely a news article; verify and relabel.
6. **press.tex L15 vs publications.tex L51** — press says the Nature paper is titled *A foundation model to predict and capture human cognition*; the publication list says *Centaur: a foundation model of human cognition*. I believe the former is the published Nature title and the latter the arXiv title, in which case the **publications entry** is the one to update. Please confirm.
7. **honors.tex L39, funding.tex L14** — fellowship is "Peretsman-Scully" but the foundation is written "Scully Peretsman". Check which order the foundation uses.
8. **talks.tex L28** — the 2026 CogSci workshop *Laying the foundations for foundation models of cognition* links to `workshop-compositionality-cogsci-2024.info`, which is the 2024 compositionality workshop. Wrong URL.
9. **organization.tex L14 vs talks.tex L45** — "Diverse Intelligences workshop series" vs "Diverse Intelligence Summit". Your statements use "Summit". Pick one.
10. **supervison.tex L81** — `University of Munich` is ambiguous (LMU or TUM). Name the institution.

### B2. Consistency choices
11. `AoE` in the location column (press.tex ×5, service.tex ×7). Reads as a deadline time-zone or a typo. Options: blank `{}`, `Remote`, or the outlet's country for press.
12. Eric Schulz is `Dr.` for the master thesis (2020) and `Prof.` for the doctorate (2021–25). If that's historically accurate, keep; otherwise align.
13. experience.tex L65 `Minnesota, USA` — every other entry uses a city. Minneapolis?
14. `Bangalore` (experience.tex L79) vs `Bengaluru` (funding.tex L42).
15. `Prof. D. van de Ville` (experience.tex L71) vs `Van De Ville, D.` (publications.tex L127) — capitalization; also the only advisors listed by initial rather than first name.
16. Strittmatter "Led to an **abstract** in the Cognitive Science Conference" vs Braga "Led to a **publication** in…" — both appear as proceedings papers with eScholarship links in conference_proceedings.tex. Align if they're the same kind of thing.
17. `LLMs for cognitive modeling` (NYU) vs `LLM for cognitive modeling` (Princeton) — intentional?
18. `UK` (honors.tex L71) vs `United Kingdom` (talks.tex L138).
19. Title casing: some papers in Title Case (*Closing the Loop to Discover…*), most in sentence case. Pick one.
20. `“Chat-GPT on the Couch”` (press.tex) vs `“Chat-GPT on the couch”` (publications.tex).
21. Jerry Han and Alex Kawaja have identical entries — merge into one line with both names, or differentiate.
22. Edward Gu: "work done during his part-time at Princeton" needs a noun — "part-time appointment"? You know the arrangement.

### B3. Additions the statements now depend on
23. Degree level for Schapiro, Fermin, Gu, Pan (post-bacc / master's) so the 4 + 4 + 3 + 2 count in the teaching statement is checkable.
24. New section **Datasets and Software**: Psych-101, Psych-201, Psyche, CogGym (+ the GitHub / HuggingFace links already scattered in supervison.tex).
25. **Memberships** line: IEEE, CSI, Cognitive Science Society.
26. MindRL Hub Cognitive Modeling challenge → service.tex.
27. NatGeo entry: confirm the exact program title and consider `participants` instead of `members`.

### B4. Structural (your call)
28. Cut 2011 high-school award; consider cutting the 2013 entrance-exam rankings.
29. Selected / Working / Publications / Proceedings overlap — six entries appear twice. Consider one appearance each outside the Selected list.
30. The Selected Publications theme header "Meta-learned models of cognition" is identical to a paper title beneath it.
31. Three `\href{}{[PDF Coming soon]}` in working_papers.tex render as dead links; plain text is safer.
32. File is named `supervison.tex` (and `\input{cv/supervison}` in cv.tex). Harmless, but if you rename, change both.

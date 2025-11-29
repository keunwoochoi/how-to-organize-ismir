# ISMIR Proceedings Publication Guide for Future Years

**For: General Chairs & Publication Chairs of ISMIR 202X**

This guide provides a comprehensive overview of the proceedings publication process, based on the ISMIR 2025 experience where proceedings were published within 2 months of the conference.

---

## Table of Contents

1. [Overview & Timeline](#overview--timeline)
2. [Staffing Recommendation](#staffing-recommendation)
3. [Phase 1: Pre-Conference Preparation](#phase-1-pre-conference-preparation-3-6-months-before)
4. [Phase 2: During Conference](#phase-2-during-conference)
5. [Phase 3: Post-Conference Production](#phase-3-post-conference-production-week-1-4)
6. [Phase 4: Archival & Publication](#phase-4-archival--publication-week-5-8)
7. [Data Collection Checklist](#data-collection-checklist)
8. [Common Pitfalls & How to Avoid Them](#common-pitfalls--how-to-avoid-them)
9. [Technical Resources](#technical-resources)
10. [Time Budget & Workload Estimate](#time-budget--workload-estimate)

---

## Overview & Timeline

### What is the Proceedings Publication Task?

The proceedings publication involves:
1. Compiling all accepted papers into a single PDF with complete front matter
2. Generating individual paper PDFs with page numbers
3. Uploading papers to Zenodo (with individual DOIs)
4. Creating archival metadata (JSON, DBLP XML)
5. Submitting to ISMIR archives and DBLP

### Realistic Timeline

| Phase | When | Duration | Key Deliverables |
|-------|------|----------|------------------|
| **Pre-Conference** | 3-6 months before | Ongoing | Data collection, relationships established |
| **During Conference** | Conference week | 1 week | Final content collected |
| **Production** | Week 1-4 after | 3-4 weeks | Compiled proceedings PDF |
| **Archival** | Week 5-8 after | 3-4 weeks | Zenodo upload, DBLP submission |
| **Total** | | **6-8 weeks** | Complete proceedings published |

**ISMIR 2025 Achievement:** Published within 2 months (faster than typical, but can be improved).

---

## Staffing Recommendation

### Option 1: Two Publication Chairs (Recommended)

**Role Split:**
- **Publication Chair 1:** Technical lead (LaTeX, Python, Git/GitHub)
- **Publication Chair 2:** Content coordinator (committee liaisons, copy editing, logo collection)

**Workload:** ~40-60 hours each over 6-8 weeks

### Option 2: One Publication Chair + Technical Assistant

**Role Split:**
- **Publication Chair:** Overall coordination, content, final review
- **Technical Assistant:** LaTeX compilation, script execution, uploads

**Workload:** 60-80 hours for chair, 30-40 hours for assistant

### Key Skills Needed

At least one person should have:
- ✅ LaTeX experience (required)
- ✅ Python scripting (required)
- ✅ Git/GitHub proficiency (required)
- ✅ PDF manipulation tools (helpful)
- ✅ Attention to detail (required!)
- ✅ Patience for debugging (required!)

---

## Phase 1: Pre-Conference Preparation (3-6 Months Before)

### Goal: Collect Everything You Need BEFORE People Stop Responding

**Critical Principle:** After the conference, people are exhausted and less responsive. Collect data proactively.

### 1.1 Establish Relationships (Month -6 to -3)

**Action Items:**
- [ ] Contact previous year's publication chair
- [ ] Join ISMIR technical committee Slack/email list
- [ ] Get access to:
  - [ ] Conference Management Toolkit (CMT) or OpenReview
  - [ ] Sponsor information (from sponsorship chair)
  - [ ] Organizing committee email list
  - [ ] Session chairs information

**Key Contacts to Establish:**
- Scientific Program Chairs (SPC)
- Sponsorship Chair
- Local Organization Chair
- DEI Chair
- Tutorial/Satellite Event organizers
- Award Committee Chair

### 1.2 Set Up Data Collection Systems (Month -3 to -1)

**Create Shared Folders/Docs for:**

1. **Paper Metadata** (from CMT/OpenReview)
   - Paper IDs, titles, authors, emails
   - Acceptance status
   - Session assignments
   - Presentation schedule

2. **Front Matter Content**
   - Welcome message from General Chairs
   - Organizing committee list (with affiliations)
   - Program committee (reviewers, meta-reviewers)
   - Keynote speaker bios & abstracts
   - Tutorial descriptions & organizers
   - Satellite event details
   - Special session descriptions
   - Awards information

3. **Visual Assets**
   - Sponsor logos (PNG/PDF, high resolution)
   - Organizing institution logos
   - Conference logo/theme artwork
   - Cover design (if custom)

4. **Statistics to Track**
   - Number of submissions
   - Number of papers reviewed
   - Acceptance rate
   - Number of reviewers/meta-reviewers
   - Number of sponsors
   - Attendee statistics (optional, if available)

### 1.3 Get ISBN Early (Month -3)

**Action:**
- [ ] Request ISBN from ISMIR Board/previous publication chair

**Why Early:** LaTeX template needs ISBN, easier to include than add later.

### 1.4 Prepare Camera-Ready Paper Collection (Month -2 to -1)

**Action:**
- [ ] Confirm camera-ready deadline with SPCs
- [ ] Set up paper collection system in CMT/OpenReview
- [ ] Verify paper format requirements:
  - [ ] Page limits
  - [ ] Template version
  - [ ] Supplementary materials policy
  - [ ] Copyright/license statements

**Important:** If papers already have their own headers/footers, our proceedings headers would NOT override them (done in ISMIR 2025).

### 1.5 Plan for Special Cases (Month -2)

**Identify and Plan for:**
- [ ] Papers to exclude (e.g., TISMIR papers, MIREX papers)
- [ ] Late-breaking/demo papers
- [ ] Papers with special characters in author names (Unicode/CJK)
- [ ] Papers with very long author lists
- [ ] Papers with wrong metadata (Yes authors do that)
- [ ] Withdrawn papers

---

## Phase 2: During Conference

### Goal: Collect Final Content While Everyone is Available

### 2.1 Final Content Collection (Conference Week)

**Must Collect During Conference:**
- [ ] Final welcome message from General Chairs
- [ ] Complete volunteer list with names (this can be updated last minute)
- [ ] Outstanding reviewer awards (announced during conference)
- [ ] Best paper awards & nominees
- [ ] Photos for social program section (optional)
- [ ] Any last-minute sponsor additions
- [ ] Confirmed keynote/tutorial abstracts (sometimes updated last minute)

**Pro Tip:** Schedule a 30-minute "content collection meeting" during the conference with key chairs. Much easier than email follow-ups later.

### 2.2 Verify Critical Data (During or Immediately After)

**Before Everyone Leaves:**
- [ ] Verify all paper PDFs collected
- [ ] Verify final session schedule
- [ ] Verify complete reviewer list (who actually reviewed, not just invited)
- [ ] Verify sponsor tier levels (Platinum/Gold/Silver/Bronze)
- [ ] Get approval on front matter content from General Chairs

---

## Phase 3: Post-Conference Production (Week 1-4)

### Goal: Compile the Proceedings PDF

### 3.1 Week 1: Setup & Metadata Preparation

**Working Directory Setup:**
```bash
git clone https://github.com/ismir/proceedings-builder
cd proceedings-builder
cp -r 2025_Proceedings_ISMIR 202X_Proceedings_ISMIR
cd 202X_Proceedings_ISMIR
```

**Install Dependencies:**
```bash
# Python environment
uv venv  # or python3 -m venv .venv
source .venv/bin/activate
uv pip install pypdf pdfrw titlecase unidecode

# Verify LaTeX installation (with CJK support if needed)
pdflatex --version
```

**Prepare Metadata:**

1. **Export from CMT/OpenReview:**
   - All accepted papers (CSV)
   - Author information (CSV)
   - Session assignments (CSV)

2. **Merge Metadata:**
   ```bash
   python scripts/prepare_metadata.py \
     --submissions "path/to/cmt_papers.csv" \
     --schedule "path/to/schedule.csv" \
     --mapping "path/to/presentation_mapping.csv" \
     --output "cmt-metadata.csv"
   ```

3. **Filter if Needed:**
   ```bash
   # If excluding certain papers (e.g., TISMIR)
   python scripts/complete_filter_pipeline.py
   ```

**Expected Time:** 8-10 hours

### 3.2 Week 1-2: Front Matter Content

**Update LaTeX Files:**

1. **imprint.tex**
   - Year, dates, location
   - ISBN
   - Editor names (GCs, SPCs, Publication Chairs)
   - Copyright notice

2. **preface.tex**
   - Welcome message
   - Conference theme/logo description
   - Statistics (submissions, acceptance, reviewers, sponsors, attendees)
   - Acknowledgements (grants, mentoring programs, DEI initiatives)

3. **organizers.tex**
   - General Chairs
   - Scientific Program Chairs
   - All organizing committee chairs
   - **Complete volunteer list** (get this during conference!)

4. **keynotes.tex**
   - Keynote speaker bios
   - Special session descriptions
   - Industry sessions
   - Music program (if applicable)

5. **tutorials.tex**
   - Tutorial descriptions with organizers
   - Satellite event details

6. **awards.tex**
   - Test-of-Time Awards
   - Best Paper Awards (nominees + winners)
   - Best Student Paper Awards
   - Outstanding Reviewer Awards

7. **committee.tex** (auto-generated)
   - Meta-reviewers
   - Reviewers
   
   Generate with:
   ```bash
   python scripts/3_generate_committee_tex.py
   ```

8. **logos.tex**
   - Sponsor logos organized by tier
   - WIMIR sponsors (if applicable)
   - Organizing institutions
   - Funding acknowledgements

**Pro Tip:** Use `\begin{CJK}{UTF8}{mj}...\end{CJK}` for Korean/Chinese/Japanese names.

**Expected Time:** 15-20 hours

### 3.3 Week 2-3: Paper Integration & Compilation

**Generate Paper Includes:**
```bash
cd scripts
python 1_generate_metadata_json.py  # Creates paper-metadata.json
python 2_generate_paper_tex.py      # Creates papers.tex
cd ..
```

**First Compilation:**
```bash
./00-run.sh
```

This runs:
- pdflatex (first pass)
- pdflatex (second pass)
- perl authorindex.pl (generate author index)
- pdflatex (third pass - includes author index)
- pdflatex (final pass - resolve references)

**Common Issues to Fix:**

1. **Unicode Errors:**
   - Wrap non-ASCII names in CJK environments
   - Already set up in 2025 template

2. **Header Height Warnings:**
   - Already fixed in `ismirproc.cls`

3. **Author Index Sorting:**
   - Some special characters may sort incorrectly
   - May need manual adjustment in `papers.tex`

4. **Page Number Mismatches:**
   - Check Table of Contents
   - Verify paper page numbers in footer

**Review Checklist:**
- [ ] Cover page looks correct
- [ ] All front matter sections included
- [ ] Table of Contents complete
- [ ] Papers in correct session order
- [ ] Author Index alphabetically correct
- [ ] Page numbers consistent throughout
- [ ] No LaTeX warnings/errors
- [ ] PDF file size reasonable (<100MB ideal)

**Expected Time:** 20-25 hours (including debugging)

### 3.4 Week 3-4: Review & Iteration

**Get Feedback From:**
- [ ] General Chairs (overall review)
- [ ] Scientific Program Chairs (paper content, order)
- [ ] Previous publication chair (technical review)

**Common Feedback Items:**
- Sponsor logo sizing/positioning
- Committee member name corrections
- Award wording
- Statistics accuracy
- Cover page design

**Budget 2-3 rounds of revisions.**

**Expected Time:** 10-15 hours

---

## Phase 4: Archival & Publication (Week 5-8)

### Goal: Upload to Zenodo, Submit to DBLP, Archive

### 4.1 Week 5: Split Proceedings & Generate Metadata

**Find Starting Page:**
```bash
# The physical page number where first paper's content starts
# Look in the compiled PDF for where Session 1 header appears
# Usually page 35-45
```

**Split into Individual Papers:**
```bash
python scripts/4_split_proceedings_6digit.py \
  --start_page [PAGE_NUMBER] \
  -o ./split_articles_6digit \
  -j ./paper-metadata-split-6digit.json \
  202X_Proceedings_ISMIR.pdf \
  paper-metadata.json \
  session-order.json
```

**Output:** E.g., 99 PDFs as `000001.pdf` through `0000XX.pdf`

**Generate Archival Metadata:**
```bash
python scripts/6_generate_final_outputs.py \
  -o ./archival_outputs \
  --start_page [SAME_PAGE] \
  paper-metadata-split-6digit.json \
  session-order.json
```

**Output:**
- `202X.json` (public metadata)
- `202X_internal.json` (extended metadata)
- `202X_dblp.xml` (for DBLP)
- `overview.csv` (for MiniConf website)

**Expected Time:** 5-8 hours

### 4.2 Week 5-6: Zenodo Sandbox Testing

**Why Test on Sandbox First:**
- Zenodo production uploads are permanent
- DOIs cannot be deleted
- Mistakes are costly

**Setup:**
```bash
# Get Zenodo tokens from ISMIR Board or previous chair
export ZENODO_TOKEN_DEV="your_sandbox_token"
export ZENODO_TOKEN_PROD="your_production_token"

# Clone conference-archive repo
git clone https://github.com/ismir/conference-archive
cd conference-archive
```

**Add Conference Entry:**

Edit `database/conferences.json`:
```json
"202X": {
  "conference_dates": "Month DD-DD, 202X",
  "conference_place": "City, Country and Online",
  "imprint_place": "City, Country",
  "conference_title": "International Society for Music Information Retrieval Conference",
  "partof_title": "Proceedings of the XXth International Society for Music Information Retrieval Conference",
  "publication_date": "202X-MM-DD",
  "imprint_isbn": "978-X-XXXXXXX-X-X",
  "doi": "10.5281/zenodo.XXXXXXX",  // Leave as placeholder initially
  "conference_acronym": "ISMIR 202X",
  "conference_url": "https://ismir202X.ismir.net",
  "imprint_publisher": "ISMIR",
  "upload_type": "publication",
  "publication_type": "conferencepaper",
  "access_right": "open",
  "license": "CC-BY-4.0",
  "editors": [
    "General Chair 1",
    "General Chair 2",
    "SPC 1",
    "SPC 2",
    "Publication Chair"
  ]
}
```

**Test Upload (3-5 papers first):**
```bash
# Create a test JSON with first 3 papers only
head -n 3 ../202X_Proceedings_ISMIR/archival_outputs/202X.json > test_202X.json

cd conference-archive
PYTHONPATH=$(pwd):$PYTHONPATH python scripts/upload_to_zenodo.py \
  test_202X.json \
  database/conferences.json \
  database/proceedings/test_202X_output.json \
  --stage dev \
  --num_cpus 1
```

**Verify on Zenodo Sandbox:**
- Check metadata accuracy
- Check PDF renders correctly
- Check author names
- Check DOI generation
- Check all links work

**Expected Time:** 8-10 hours

### 4.3 Week 6-7: Production Zenodo Upload

**⚠️ Important:** This creates permanent DOIs. Double-check everything.

**Update JSON with Local Paths:**

The `ee` field should point to local files:
```json
"ee": "../202X_Proceedings_ISMIR/split_articles_6digit/000001.pdf"
```

**Run Production Upload:**
```bash
export ZENODO_TOKEN_PROD="your_production_token"

cd conference-archive
PYTHONPATH=$(pwd):$PYTHONPATH python scripts/upload_to_zenodo.py \
  ../202X_Proceedings_ISMIR/archival_outputs/202X.json \
  database/conferences.json \
  database/proceedings/202X.json \
  --stage prod \
  --num_cpus 1 \
  --verbose 5 2>&1 | tee /tmp/zenodo_upload.log
```

**This will take 2-4 hours for ~100 papers.**

**If Upload Interrupts:**
```bash
# Use resume script
cd ..
python scripts/resume_upload.py

# Follow the generated command to continue
```

**After Upload Completes:**

1. **Update Page Numbers in JSON:**
   - Extract correct page ranges from LaTeX `.toc` file
   - Update `pages` field in `202X.json`
   - Regenerate `202X_dblp.xml`

2. **Upload Full Proceedings to Zenodo:**
   - Create a separate Zenodo deposit for the full PDF
   - This gets a separate DOI (for the proceedings as a whole)

3. **Submit for Review:**
   - Request ISMIR Board to add to ISMIR Zenodo community
   - They will review and approve

**Expected Time:** 10-15 hours (including monitoring, fixes, review)

### 4.4 Week 7-8: DBLP Submission & Archive Upload

**Create Pull Request to conference-archive:**

```bash
cd conference-archive
git checkout -b add-202X-data

# Commit your changes
git add database/conferences.json
git add database/proceedings/202X.json
git add database/proceedings/202X_dblp.xml
git commit -m "Add ISMIR 202X proceedings metadata"

git push origin add-202X-data
# Create PR on GitHub
```

**Create Backup Archive ZIP:**
```bash
cd ../202X_Proceedings_ISMIR/split_articles_6digit
zip -r ismir202X-archives-backup.zip *.pdf
```

**Send to Archives Coordinator:**
- Contact ISMIR Board for current archives coordinator
- Provide ZIP file for upload to `archives.ismir.net`
- Verify upload at: `https://archives.ismir.net/ismir202X/paper/000001.pdf`

**DBLP Submission:**
- ISMIR Board typically handles DBLP submission
- Provide `202X_dblp.xml` to them
- Verify appearance at: `https://dblp.org/db/conf/ismir/ismir202X.html`

**Expected Time:** 5-8 hours

---

## Data Collection Checklist

### Critical Data (Must Have)

**From CMT/OpenReview:**
- [ ] All accepted paper PDFs (in final camera-ready version)
- [ ] Paper metadata (ID, title, authors, emails, affiliations)
- [ ] Session assignments
- [ ] Presentation schedule (day, time, session)
- [ ] Complete reviewer list (who actually reviewed)
- [ ] Complete meta-reviewer list

**From Committee Chairs:**
- [ ] Welcome message from General Chairs
- [ ] Complete organizing committee list with affiliations
- [ ] Complete volunteer list with names
- [ ] Keynote speaker bios & talk abstracts
- [ ] Tutorial descriptions with organizer names
- [ ] Satellite event details
- [ ] Special session descriptions
- [ ] Award information (all categories)

**From Sponsorship Chair:**
- [ ] All sponsor logos (PNG or PDF, high resolution)
- [ ] Sponsor tier levels (Platinum/Gold/Silver/Bronze)
- [ ] WIMIR sponsor list (if applicable)
- [ ] Organizing institution logos

**From ISMIR Board:**
- [ ] ISBN for proceedings
- [ ] Zenodo API tokens (sandbox + production)
- [ ] Conference-archive repository access

### Important Data (Should Have)

- [ ] Conference statistics (submissions, acceptance rate, etc.)
- [ ] Attendee statistics
- [ ] Newcomer/mentoring program details
- [ ] DEI initiative descriptions
- [ ] Funding acknowledgements
- [ ] Outstanding reviewer list
- [ ] Cover design or booklet first page

### Optional Data (Nice to Have)

- [ ] Photos from conference
- [ ] Social program descriptions
- [ ] Music program details
- [ ] Local culture information

---

## Common Pitfalls & How to Avoid Them

### Pitfall 1: Missing Data After Conference

**Problem:** Trying to chase down committee members weeks after conference.

**Solution:** Collect everything during or immediately after conference. Schedule a "content collection meeting" during the conference week.

### Pitfall 2: Incorrect Reviewer Lists

**Problem:** Using invitation list instead of actual reviewers who completed reviews.

**Solution:** Export final reviewer completion data from CMT/OpenReview. Cross-reference with meta-reviewer reports.

### Pitfall 3: Wrong Page Numbers in Metadata

**Problem:** Page numbers in JSON/DBLP don't match compiled PDF.

**Solution:** Extract page ranges from LaTeX `.toc` file after final compilation. Verify by spot-checking random papers.

### Pitfall 4: Zenodo Upload Failures

**Problem:** Upload fails midway, unclear what succeeded.

**Solution:** Use the resume script provided in 2025 template. Always use `num_cpus=1` for production uploads.

### Pitfall 5: Unicode Character Errors

**Problem:** Names with special characters break LaTeX compilation.

**Solution:** Use `\begin{CJK}{UTF8}{mj}...\end{CJK}` environments. Already set up in 2025 template.

### Pitfall 6: Double Headers on Papers

**Problem:** Proceedings headers appear over paper's original headers.

**Solution:** Already fixed in 2025 `ismirproc.cls` with `\thispagestyle{plain}`.

### Pitfall 7: Author Index Sorting Issues

**Problem:** Names with special characters sort to the end.

**Solution:** May need to adjust names in `papers.tex` for sorting (while preserving display in PDF content).

### Pitfall 8: Last-Minute Content Changes

**Problem:** Sponsors, awards, or committee changes after you've finalized.

**Solution:** Set a "content freeze date" 1 week after conference. After that, only critical corrections.

### Pitfall 9: Unclear Task Scope

**Problem:** Not knowing the full scope until you're in the middle of it.

**Solution:** Read this entire guide before accepting the role. Budget 60-80 hours over 6-8 weeks.

### Pitfall 10: Version Control Chaos

**Problem:** Multiple versions of files, unclear which is latest.

**Solution:** Use Git from day one. Commit often. Use branches for major changes.

---

## Technical Resources

### Essential Repositories

1. **proceedings-builder**
   - URL: https://github.com/ismir/proceedings-builder
   - Your working directory
   - Contains LaTeX templates and Python scripts

2. **conference-archive**
   - URL: https://github.com/ismir/conference-archive
   - For Zenodo uploads and metadata
   - Contains historical proceedings data

### Documentation to Read

1. **proceedings-builder README**
   - `202X_scripts/README.md` - Current workflow
   - `2025_Proceedings_ISMIR/README.md` - ISMIR 2025 specific guide
   - `2025_Proceedings_ISMIR/QUICK_START.md` - Quick reference

2. **conference-archive README**
   - Main README explains Zenodo workflow
   - Critical for Phase 4

### External Resources

1. **Zenodo Documentation**
   - https://developers.zenodo.org/
   - API documentation for uploads

2. **DBLP Submission Guidelines**
   - https://dblp.org/
   - XML format requirements

3. **LaTeX CJK Package**
   - For Unicode support
   - Already integrated in 2025 template

### Contact Points

1. **ISMIR Board**
   - For: ISBN, Zenodo tokens, archives access
   - When: 2-3 months before conference

2. **Previous Publication Chair**
   - For: Handoff, tips, technical questions
   - When: As soon as you're appointed

3. **Technical Committee**
   - For: Website integration, MiniConf data
   - When: After proceedings published

---

## Time Budget & Workload Estimate

### Detailed Time Breakdown

| Phase | Task | Hours | When |
|-------|------|-------|------|
| **Pre-Conference** | | | |
| | Setup meetings & relationships | 3-5 | Month -6 to -3 |
| | Data collection system setup | 2-3 | Month -3 |
| | Ongoing data collection | 5-8 | Month -3 to 0 |
| | **Subtotal** | **10-16** | |
| **During Conference** | | | |
| | Final content collection | 2-3 | Week 0 |
| | **Subtotal** | **2-3** | |
| **Post-Conference Production** | | | |
| | Setup & metadata prep | 8-10 | Week 1 |
| | Front matter content | 15-20 | Week 1-2 |
| | Paper integration & compilation | 20-25 | Week 2-3 |
| | Review & iteration | 10-15 | Week 3-4 |
| | **Subtotal** | **53-70** | |
| **Archival & Publication** | | | |
| | Split & generate metadata | 5-8 | Week 5 |
| | Zenodo sandbox testing | 8-10 | Week 5-6 |
| | Production upload | 10-15 | Week 6-7 |
| | DBLP & archive submission | 5-8 | Week 7-8 |
| | **Subtotal** | **28-41** | |
| **TOTAL** | | **93-130 hours** | **6-8 weeks** |

### Workload Distribution (Two-Chair Model)

**Publication Chair 1 (Technical Lead):**
- Metadata preparation: 8-10 hours
- LaTeX compilation & debugging: 25-30 hours
- Script execution: 10-15 hours
- Zenodo uploads: 15-20 hours
- **Total: 58-75 hours**

**Publication Chair 2 (Content Coordinator):**
- Data collection: 15-20 hours
- Front matter content editing: 15-20 hours
- Committee liaison: 5-8 hours
- Review & feedback coordination: 10-15 hours
- **Total: 45-63 hours**

### Critical Path Items

**These tasks have dependencies and can delay everything:**
1. ✅ ISBN acquisition (need early)
2. ✅ Camera-ready paper collection (need complete set)
3. ✅ Reviewer list finalization (need accurate data)
4. ✅ Zenodo token access (need before upload)
5. ✅ General Chair approval (need for publication)

---

## Moving to OpenReview (If Applicable)

If ISMIR moves to OpenReview.net instead of CMT:

### What Changes

**System Differences:**
- Different export formats (but same content needed)
- Different metadata fields
- Different API access

**Adaptation Needed:**
- Update `prepare_metadata.py` script to parse OpenReview format
- Metadata mapping might need adjustment
- Paper PDF download process might differ

### What Doesn't Change

**Data Collection Requirements:**
- Still need same content (papers, metadata, committee, etc.)
- Still need same front matter information
- Still need sponsor logos, bios, etc.

**Publication Workflow:**
- LaTeX compilation process unchanged
- Zenodo upload process unchanged
- DBLP submission unchanged

**The 2025 scripts are designed to be adaptable.** Main change needed is in Step 1 (metadata import).

---

## Recommendations for Success

### For General Chairs

1. **Appoint Publication Chair(s) Early**
   - At least 6 months before conference
   - Consider two chairs (technical + content)

2. **Provide Clear Access**
   - CMT/OpenReview admin access
   - Organizing committee email list
   - Budget for any needed tools/services

3. **Set Expectations**
   - 60-80 hours of work per chair
   - 6-8 weeks post-conference
   - Need technical skills (LaTeX, Python, Git)

4. **Support Data Collection**
   - Emphasize to all chairs to respond to publication chair requests
   - Schedule "content collection meeting" during conference
   - Set content freeze date

### For Publication Chairs

1. **Start Early**
   - Don't wait until after conference
   - Build relationships with committee chairs
   - Set up data collection systems in advance

2. **Use Git from Day One**
   - Version control everything
   - Commit often
   - Use branches for experiments

3. **Test Early and Often**
   - Compile LaTeX frequently
   - Test scripts on sample data
   - Use Zenodo sandbox before production

4. **Document Your Process**
   - Keep notes of what worked/didn't work
   - Update this guide for next year
   - Create handoff document

5. **Ask for Help**
   - Contact previous publication chair
   - Post questions in ISMIR technical committee
   - Don't struggle alone

6. **Set Realistic Expectations**
   - 6-8 weeks is realistic
   - 2 months is good
   - 3 months is still acceptable
   - Communicate timeline to General Chairs

---

## Final Checklist: Before You Start

Before accepting the Publication Chair role, confirm:

- [ ] You have 60-80 hours available over next 3 months
- [ ] You are comfortable with LaTeX
- [ ] You are comfortable with Python scripting
- [ ] You are comfortable with Git/GitHub
- [ ] You have support from General Chairs
- [ ] You have been given access to necessary systems
- [ ] You have contacted previous publication chair
- [ ] You understand the full scope (read this entire guide)
- [ ] You are ready to collect data proactively
- [ ] You have a co-chair or technical assistant (recommended)

---

## Conclusion

The ISMIR proceedings publication is a significant but manageable task. With proper preparation, clear communication, and systematic execution, proceedings can be published within 6-8 weeks post-conference.

**Key Success Factors:**
1. ✅ **Collect data early** - Don't wait until after conference
2. ✅ **Use existing templates** - 2025 template is comprehensive
3. ✅ **Test thoroughly** - Especially Zenodo uploads
4. ✅ **Communicate clearly** - Set expectations with General Chairs
5. ✅ **Ask for help** - Leverage previous chairs and technical committee

**ISMIR 2025 proved that 2-month publication is achievable.** With this guide and the 2025 template, future publication chairs can achieve the same or better.

Good luck with your proceedings publication! 🎉

---

**Document Prepared By:** Keunwoo Choi, Publication Chair, ISMIR 2025  
**Date:** November 2025  
**Based On:** ISMIR 2025 proceedings published within 2 months post-conference  
**Next Update:** ISMIR 2026 Publication Chair should review and update based on their experience


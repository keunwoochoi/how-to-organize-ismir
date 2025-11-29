# ISMIR 2025: Specific Decisions & Data

This document records the specific decisions, data, and context from the 2025 conference. It serves as a historical record and a reference for specific numbers and "this year's choices".

## 1. Core Organization & Strategy

### Overall Timeline & Milestones
*   **Chairs**: 3 General Chairs (Juhan, Dasaem, Keunwoo).
    *   **Remote Chair**: Keunwoo joined a year late and worked remotely from New York. This worked fine for many tasks but required strong local coordination from the other two.
*   **Satellite Events**: No chairs in 2025. One GC handled this workload, which contributed to overworking.
    *   **Recommendation**: Appoint a dedicated Satellite Chair. The workload is distinct enough to warrant it.

### Budget & Finance
*   **Grants**: Provided the highest number of grants in 2025 history.
    *   **The "Why"**: We wanted to maximize accessibility.
    *   **The Cost**: The workload was underestimated. It wasn't just selection; it was hundreds of individual bank transfers, visa letters, and hotel bookings.
    *   **Lesson**: We desperately needed a local Grant Chair to handle the PCO interface.
*   **Paid Roles**:
    *   **Web Chair**: Paid position in 2025. The workload (constant updates, custom design) and skill requirement justified this. It was cost-effective compared to a contractor.
    *   **Virtual Chairs**: Students received gift cards. This was deemed fair as the role has high labor but low networking benefits.

### Venue & Local Logistics
*   **Location**: KAIST campus (Daejeon).
    *   **Setup**: Multiple buildings used.
    *   **Impact**: The isolated location (vs. a downtown hotel) led to high session attendance. Attendees stayed focused on the conference.
    *   **Issues**:
        *   **Display Failures**: The Creative Learning Building display failed the day before. Required emergency fixes by local staff.
        *   **Weather**: Rain impacted outdoor tents (which weren't waterproof). Always have an indoor backup.
*   **Catering**:
    *   **Format**: Boxed lunches were used.
    *   **Perk**: Unlimited coffee/snacks all day was very popular and highly appreciated.
*   **Events**:
    *   **Welcome Reception**: Casual interaction with light meals.
    *   **Banquet**: Seated dinner. Finding a venue in Daejeon that fit the budget and vibe was difficult; required extensive scouting.
    *   **K-Culture Night**: Added based on attendee interest. A special event showcasing local culture.
*   **Transportation**:
    *   **Shuttles**: Buses ran from 3 hotel areas with fixed schedules.
    *   **Outcome**: Essential. It was nearly impossible for non-Korean speakers to grab taxis during rush hour in Daejeon.
    *   **Lesson**: Do not rely on public transit/taxis for isolated venues, especially if there is a language barrier.
*   **Registration**:
    *   **Staffing**: Staffed desks.
    *   **Badges**: Physical badges with stickers for social signals (e.g., "No Photos").
*   **Photography**:
    *   **Consent**: Yellow lanyards offered for "do not photograph".
    *   **Usage**: Rarely used in practice.
    *   **Sharing**: Photos shared via Google Photos (non-archival, good for preview).

### Virtual/Hybrid Strategy
*   **Platforms**:
    *   **Zoom**: Used for sessions.
    *   **Slack**: Used for communication.
    *   **YouTube**: Used for livestreaming & archiving.
*   **Streaming**:
    *   **Feature**: YouTube livestream with DVR (rewind) allowed attendees to catch up on missed morning sessions.
    *   **The Scare**: We were terrified of YouTube shutting down the channel due to copyright strikes from music in presentations.
    *   **Mitigation**: We considered a "kill switch" but mostly relied on luck and the fact that live takedowns are rarer than VOD takedowns.
*   **Consent Experience**:
    *   **Tutorials**: Asked post-conference. This slowed down archiving significantly. **Mistake**.
    *   **Industry**: Negotiated case-by-case (some opted out).
    *   **Keynotes**: Discussed during invitation.
    *   **Music**: Required explicit consent due to rights issues.
    *   **Papers**: Defaulted to public sharing (standard for academic conferences).
*   **Unconference**: Geoffroy was the sole chair (2023-2025). The session felt under-defined and needs rethinking.

## 2. Scientific Program

### Stats & Data
*   **Submissions**: 278 papers.
*   **Acceptance Rate**: 35.6% (99 accepted).
    *   **Breakdown**:
        *   Generative Tasks: ~47% (High)
        *   Creativity: 50% (High)
        *   Human-Centered MIR: 12.5% (Low - potentially concerning)
        *   Applications: 28%
*   **Reviewers**: ~250 reviewers, ~30 meta-reviewers.

### Review Process Issues
*   **The "Chatbot Reviewer" Incident**:
    *   **Issue**: A reviewer submitted generic, low-quality reviews that appeared AI-generated.
    *   **Action**: SPC Chairs drafted a direct email: *"It was brought to our attention... that your submitted reviews [contain] generic, chatbot-like prose."*
    *   **Outcome**: The reviewer was asked to revise. This set a precedent for active policing of review quality.
*   **The "Fake Citation" Desk Reject**:
    *   **Issue**: A paper (ID 336) cited 3 non-existent papers (e.g., "Singscope: A mobile application...").
    *   **Action**: Immediate desk rejection.
    *   **Lesson**: Verify citations if something looks "off". Hallucinations are real.
*   **Meta-Reviewer Confusion**:
    *   **Issue**: Confusion over whether the Meta-Reviewer's "Final Recommendation" (Q22) was visible to authors as a decision.
    *   **Clarification**: It is a recommendation. Chairs make the final decision. The notification email explicitly stated this to avoid ambiguity.

### Awards
*   **Best Paper Committee**:
    *   **Composition**: 22 Meta-Reviewers.
    *   **Process**: Invited on Sep 9 (Tuesday of conference week). Voting closed Sep 11 (Thursday).
    *   **Shortlist**: 8 papers (IDs: 4, 7, 47, 208, 286, 229, 278, 308).
    *   **Criteria**: Read paper + *Strongly Suggested* to attend oral/poster presentation.
*   **Test of Time**:
    *   **Categories**: Two awards (Classical & 10-year).
    *   **Ceremony**: In-person talks were a highlight.

### Program Scheduling
*   **Online Fun-Facts**:
    *   **Idea**: We asked authors for "fun facts" to share on Slack/Social Media.
    *   **Execution**: Mixed success. It adds personality but is another administrative task to track.
*   **Session Management**:
    *   **Kill Switch**: Session chairs were briefed on the risk of YouTube copyright strikes during music demos.
    *   **Status Updates**: Chairs manually updated paper statuses in the system to avoid bulk-edit disasters.

### Publication & Proceedings
*   **Timeline**:
    *   **Published**: Nov 21 (Conference ended Sep 26). Total ~8 weeks.
    *   **Speed Factor**: We used the `proceedings-builder` scripts which automated metadata generation and PDF splitting.
*   **Workflow Decisions**:
    *   **Zenodo Sandbox**: We tested the upload on Zenodo Sandbox first. This saved us from a metadata error that would have been permanent on the production site.
    *   **Split Proceedings**: We published individual PDFs for each paper (with DOIs) *and* a single compiled PDF. This maximized visibility for authors.
*   **Staffing**:
    *   **Model**: 1 Chair (Keunwoo) + 1 Technical Assistant.
    *   **Workload**: The Chair spent ~60 hours; Assistant ~30 hours.
*   **Deliverables**:
    *   **Posters**: A0 portrait confirmed.
    *   **Slides**: Managed via Google Drive. Volunteers/Session Chairs handled the flow.

## 3. Events & Programming

### Music Program
*   **The "Jam Bot" Incident**:
    *   **Context**: A selected performance ("Jam Bot") promised a "special guest".
    *   **The Crisis**: During the conference week, it was revealed the guest was a locally hired musician found last-minute, not a core collaborator.
    *   **Friction**: Organizers had spent political capital (banquet tickets, confidentiality) for this "guest", feeling misled.
    *   **Lesson**: Demand transparency from performers early. No "surprises" for organizers.
*   **Format**:
    *   **Concert**: Held in a dedicated hall.
    *   **Jam Session**: Held in the main hall (Creative Learning Bldg).
    *   **Tech**: We relied on local volunteers for stage management, which was stressful but worked.

### Tutorials
*   **Format Decision**:
    *   **Hybrid**: We stuck with Hybrid (Zoom + In-person) despite known issues.
    *   **Feedback**: Presenters found it burdensome ("screenshare + mic + camera"). Remote attendance was low.
    *   **Verdict**: The "Hybrid Tax" is too high. Future years should consider separating them.
*   **Topics**: 6 tutorials accepted.
*   **Schedule**: Pre-conference Sunday; parallel sessions.
*   **Consent**: Asked post-conference, which caused delays.

### Industry
*   **Booths**:
    *   **Space**: We ran out of space for desks. One sponsor asked for an extra desk last minute, and we had to say no.
    *   **Placement**: Located near the coffee/snacks, which ensured good traffic.
*   **Presentations**:
    *   **Lightning Talks**: 1-minute talks worked well to drive traffic to booths.

### Unconference
*   **Chair**: Geoffroy (sole chair).
*   **Issues**: The session felt under-structured.
*   **Topics**: Ethics, Safety, Copyright (voted by attendees).
*   **Timing**: Held after LBD. Attendance was ~70 people.
*   **Format**: Moved to main room due to weather.
*   **Follow-up**: Slack channels created for each topic.

### Late Breaking Demos (LBD)
*   **Capacity**: Capped at 75 (first-come-first-served).
*   **System**: CMT (Author console -> LBD).
*   **Screening**: Rolling basis. No resubmissions allowed.
    *   **Outcome**: Smoothed the workload for chairs.
*   **Specs**: A0 poster required. Video optional (conflicting specs noted between web/email).

### Industry & Sponsorship
*   **Sponsorship**:
    *   **Tiers**: Registration-based benefits were highly appreciated by sponsors.
    *   **Recruitment**: Targeted outreach strategy.
*   **Industry Events**:
    *   **Presentations**: 8min (Platinum), 4min (Silver).
    *   **Booths**: Assigned via raffle.
    *   **Lightning Talks**: 25 slots (1-min, 1-slide).
    *   **Job Board**: Platinum access; self-hosted PDFs.
    *   **Panel**: Cancelled due to time constraints.
    *   **System**: Google Forms used for submissions.

## 4. Community & Support

### Diversity, Equity, & Inclusion (DEI)
*   **Photo Consent**: Yellow lanyards provided for "do not photograph". Rarely used.
*   **Programs**: Newcomer squads and WIMIR activities executed by respective chairs.
*   **Grants**: Led by Grants Chairs; DEI collaboration was minimal in 2025.

### Travel Grants
*   **Stats**:
    *   99 waivers (inc. 15 virtual).
    *   44 accommodation grants.
    *   5 travel grants.
*   **Categories**: Authors, WIMIR, Music, LBD/Satellite (added late).
*   **Scoring Weights**: +1 for Student, Underrepresented, LMIC, Queer, Unaffiliated, Women, Accessibility.
*   **Logistics**:
    *   **Travel**: Pre-purchased tickets. Proved logistically simple but budget-unpredictable.
    *   **Accommodation**: Shared twin rooms. Preferences collected via Google Form.
    *   **Confirmation**: Email with embedded form + LinkedIn outreach for non-responders.

### Volunteers
*   **Roles**:
    *   **Specialization**: We required English/Korean proficiency for specific roles (Registration, Info Desk).
    *   **Outcome**: Crucial for bridging the gap between the PCO (local staff) and attendees.
*   **Shifts**:
    *   **One-day**: We used one-day shifts.
    *   **Outcome**: Volunteers preferred this as it allowed them to enjoy the conference on off-days.

## 5. Communication & Operations

### Website
*   **Workflow**:
    *   **Google Docs**: All content was drafted and approved in Google Docs before being touched by the Web Chair.
    *   **Menu Structure**: We explicitly merged "Registration" and "Grants" into a single "Attend" menu to simplify navigation, following the 2024 model.
*   **Tech**:
    *   **Static Site**: Continued using the Jekyll-based template.
    *   **Data**: Tutorial schedules were handled via CSV imports to generate tables.

### Social Media
*   **Design Decision**:
    *   **Ratio**: We used a 4:3 image ratio for all assets.
    *   **Why**: It crops correctly on Instagram (square), Twitter (landscape), and LinkedIn without needing 3 separate versions.
*   **The "June Blitz"**:
    *   **Context**: We had a backlog of announcements in June.
    *   **Execution**: We executed a 6-step "Waterfall" over one week:
        1.  Save the Date
        2.  Call for LBD
        3.  Call for Music (Urgent deadline)
        4.  Call for Grants (Linked to Music)
        5.  LLM4Music (Satellite)
        6.  Other Satellites
    *   **Result**: High engagement without drowning out any single announcement.

### Virtual
*   **Zoom**: We used a dedicated "Virtual Chair" who manually generated and managed Zoom links for every session.
*   **Slack**: The primary community hub. We created channel-per-paper, which was automated but resulted in too many dead channels.

### Registration System
*   **Waivers**: Managed via codes for Grants, Volunteers, and Sponsors.
*   **Submission**: CMT (OpenReview recommended for future).
*   **Communication**: Slack.
*   **Streaming**: YouTube Live (manual moderation).
*   **Forms**: Google Forms used extensively for LBD, Industry, and Grants.

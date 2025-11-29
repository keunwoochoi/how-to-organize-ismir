# ISMIR Organization: General Guidelines

This document outlines the timeless guidelines, standard procedures, and best practices for organizing ISMIR. It is structured by work items rather than specific chair roles to encourage a holistic view of the conference organization.

## 1. Core Organization & Strategy

### Mental Models for Organizers
*   **The "Local vs. Global" Split**:
    *   **Concept**: Every major role (Grants, Volunteers, Music) needs a "Local" counterpart and a "Global" counterpart.
    *   **Why**: The "Global" chair understands the ISMIR culture and academic standards. The "Local" chair speaks the language, knows the venue constraints, and handles payments.
    *   **Failure Mode**: A single "Global" chair for Grants will drown in bank transfer paperwork they can't navigate. A single "Local" chair might reject valid applicants because they don't understand the "ISMIR vibe".
*   **The "Hidden Workload" Principle**:
    *   **Grants**: It's not just selecting people. It's 80% logistics (visas, bank transfers, hotel bookings).
    *   **Virtual**: It's not just "turning on Zoom". It's building a website (miniconf), managing Slack, and editing video. It is a full-time DevOps job.

### Overall Timeline & Milestones
*   **Month -12 to -9**:
    *   **Appoint General Chairs (GCs)**: Ideally 3 people. A mix of local and experienced ISMIR attendees is crucial.
    *   **Form Key Committees**: Scientific Program, Local Org, and Finance.
    *   **Venue & Budget**: Define high-level budget and venue strategy. On-campus venues are often cheaper and foster better attendance than scattered hotels.
*   **Month -8 to -6**:
    *   **PCO Contract**: Select and contract a Professional Conference Organizer (PCO) for non-core tasks (catering, registration, visas).
    *   **Venue Layout**: Plan room allocations for sessions, posters, and social events.
    *   **Dates**: Finalize conference dates to avoid conflicts with major holidays or related conferences.
*   **Month -6 to -4**:
    *   **Logistics**: Finalize shuttle schedules, food/catering plans (dietary needs are critical), and registration tiers.
    *   **Recruitment**: Launch volunteer calls (General and Local).
*   **Month -3 to -2**:
    *   **Tech Setup**: Configure miniconf, Slack, and AV systems.
    *   **Testing**: Conduct dry runs for WiFi, streaming, and hybrid interactions.
*   **Month -1 to 0**:
    *   **Operations**: Manage on-site logistics, live streams, and daily troubleshooting.
*   **Post-Conference**:
    *   **Wrap-up**: Debrief with all chairs, close finances, and archive materials (website, proceedings).

### Budget & Finance
*   **PCO Management**:
    *   **Role**: PCOs handle catering, visas, registration, and payments.
    *   **Warning**: Do not trust them blindly. ISMIR has higher standards for community care (e.g., dietary options, student support) than average corporate events. Micro-management is often necessary.
    *   **Negotiation**: Push back on initial quotes and suggestions if they don't align with ISMIR values (e.g., insufficient vegetarian options).
*   **Grant Strategy**:
    *   **Leadership**: Appoint Grant Chairs early. **Crucial**: Pair a local chair (logistics/payments) with an experienced attendee (selection).
    *   **Communication**: Ensure clear communication between Grant Chairs and PCO to avoid overworking the chairs with payment logistics.

### Venue & Local Logistics
*   **Venue Selection**:
    *   **Campus vs. Hotel**: On-campus venues (like KAIST) often provide fresh air, outdoor spaces, and budget savings. They also tend to keep attendees focused on the conference rather than exploring the city.
    *   **Capacity**: Ensure spaces can handle parallel sessions (if used) and large poster sessions (A0 boards).
*   **Catering**:
    *   **Ownership**: Local Chairs should own food decisions. Don't leave it entirely to the PCO.
    *   **Essentials**: Unlimited coffee/snacks all day are highly appreciated and keep energy levels high.
    *   **Diversity**: Provide robust options for various diets (vegan, gluten-free, halal, etc.).
*   **Transportation**:
    *   **Shuttles**: If the venue is isolated, provide shuttles from major hotel clusters.
    *   **Communication**: Publish schedules and maps early. Use apps or Slack for real-time updates.
*   **Crisis Management (The "Go-Bag")**:
    *   **Tech**: Have a dedicated "Emergency Tech Kit" with HDMI cables, dongles (USB-C to HDMI), and **at least one Windows laptop** (for compatibility testing).
    *   **Weather**: If using outdoor spaces, have a "Plan B" (indoor room) ready. Tents are often not enough for heavy rain.
*   **Volunteers**:
    *   **Structure**: One-day shifts are preferred over multi-day shifts to allow volunteers to enjoy the conference.
    *   **Local vs. General**:
        *   **Local Volunteers**: Essential for bridging communication with PCO (language/culture) and handling on-site tech (presentation materials).
        *   **General Volunteers**: Good for registration desk, session monitoring, and wayfinding.
    *   **Autonomy**: Give Volunteer Chairs autonomy to handle unexpected situations (e.g., no-shows) without needing GC approval for every small decision.

### Virtual/Hybrid Strategy
*   **Heuristic: "Async First"**:
    *   **Risk**: Real-time hybrid is high-risk (tech failure, empty rooms) and high-effort.
    *   **Safe Bet**: Prioritize async interaction (Slack, pre-recorded videos) and a robust archive.
*   **Platforms**:
    *   **Slack**: The primary hub for communication (organizers & attendees). Avoid creating per-paper channels; they usually have zero activity and clutter the workspace.
    *   **Zoom**: Standard for session delivery.
    *   **YouTube**: Use for live streaming and archiving.
*   **Streaming & Copyright**:
    *   **The Trap**: Live streaming music presentations often triggers YouTube's copyright bots, risking channel shutdown.
    *   **Mitigation**: Use a private stream or upload edited videos later. If live, have a "kill switch" to mute audio during music demos.
*   **Consent**:
    *   **Critical**: Obtain recording/sharing consent **BEFORE** the conference for all session types (Keynotes, Tutorials, Music, Papers).
    *   **Matrix**: Create a consent matrix to track permissions for each session (e.g., "Live Stream OK", "Archive OK", "No Recording").
*   **Staffing**:
    *   **Workload**: Virtual Chairs have a heavy workload (setup, monitoring, archiving).
    *   **Team Size**: Recommend 3 chairs.
    *   **Compensation**: Consider compensation (e.g., gift cards) for student chairs due to the high technical demand and lack of networking benefits compared to other roles.

## 2. Scientific Program

### Mental Models for SPCs
*   **The "Review Quality Firewall"**:
    *   **Concept**: Your primary job isn't just assigning papers; it's detecting and filtering out bad faith actors (LLM-generated reviews, fake citations).
    *   **Heuristic: "Trust Your Gut on LLM Reviews"**: If a review feels generic, lacks specific references to the paper's content, and uses "chatbot-like" prose, it is likely AI-generated.
    *   **Action**: Don't be afraid to confront the reviewer. Draft a stern email (with other SPCs) asking for a revision or explanation. Bad reviews damage the conference's reputation more than a delayed decision.
*   **The "Manual Safety" Principle**:
    *   **Context**: Conference management systems (CMT, OpenReview) often have confusing UI for bulk actions.
    *   **Rule**: For critical actions like "Accept/Reject" status changes, **do it manually one-by-one** (or in small batches) rather than trusting a "Select All" bulk action. The risk of sending a "Reject" email to an "Accept" author is too high.

### Call for Papers (CFP) & Review Process
*   **Review Model**:
    *   **Double-Blind**: Standard for ISMIR to reduce bias.
    *   **Open Review**: Consider "Open Review" models (e.g., opting out of anonymity) but ensure community consensus.
*   **Timeline**:
    *   **Jan-Feb**: Finalize CFP.
    *   **April**: Submission deadline.
    *   **May-June**: Review period.
    *   **July**: Decisions.
*   **Review Management**:
    *   **Desk Rejections**: Be rigorous. Check for **Fake Citations** (hallucinations). In 2025, a paper was desk rejected for citing 3 non-existent papers.
    *   **Meta-Reviewers**: Clarify their role. Their "recommendation" (Q22) is just that—a recommendation. The SPC Chairs make the final decision.
*   **Acceptance Rates**:
    *   **Target**: Historically around 35-40%.
    *   **Variance**: Be aware that acceptance rates vary wildly by topic (e.g., "Generative Tasks" might be 45%, while "Human-Centered MIR" might be 12%). Balance the program to ensure diversity of topics, not just raw scores.
*   **Program Structure**:
    *   **Sessions**: Integrate oral/poster sessions with tutorials and industry events.
    *   **Tracks**: Avoid parallel sessions if possible to ensure focus, though parallel tracks increase capacity.
    *   **Mixed Sessions**: Mixing topics can encourage cross-pollination, but themed sessions are easier for attendees to navigate.
*   **Author Support**:
    *   **Deliverables**: Provide clear instructions on deliverables (slides, posters, videos).
    *   **Chasing**: Be prepared to chase missing assets aggressively. Automated reminders from the submission system are helpful.

### Awards (Best Paper, Test of Time)
*   **Best Paper**:
    *   **Committee Formation**:
        *   **Selection**: Invite ~20 high-performing Meta-Reviewers.
        *   **Confidentiality**: Keep the committee membership confidential to avoid lobbying.
    *   **The "Conference Crunch"**:
        *   **Timing**: The committee work happens *during* the conference (viewing posters/talks).
        *   **Logistics**: You must send invitations and papers *immediately* before the conference. Voting usually closes on Thursday at 1 PM to allow for the ceremony preparation.
        *   **Workload**: It is intense. Ensure committee members know they need to read 8 papers in 2 days.
    *   **Process**: Coordinate early with Scientific Program Chairs (SPC) for nominations.
    *   **Selection**: Use a holistic review process (committee deliberation) rather than just raw reviewer scores.
    *   **Confidentiality**: Maintain strict confidentiality until the closing session announcement.
*   **Test of Time**:
    *   **Timing**: Start early (Month 5/6). This award requires digging into history and finding authors who may have moved on.
    *   **Nominations**: Open nominations to the community for transparency and to surface overlooked papers.
    *   **COI**: Strictly manage Conflicts of Interest (COI) within the committee.
    *   **Categories**: Consider multiple categories (e.g., "Classical" for older papers vs. "10-Year" for recent impact).

### Special Sessions
*   **Purpose**: Address emerging topics or community needs (e.g., "Music & AI Ethics", "Industry Trends").
*   **Planning**: Define scope and call for participation early (Month -6).
*   **Integration**: Schedule these to avoid conflicts with major keynotes or popular oral sessions.

### Publication & Proceedings
*   **Mental Model: "The 2-Month Sprint"**:
    *   **Concept**: Proceedings publication is not an "afterthought"; it is a major production phase that starts *during* the conference.
    *   **Timeline**: Pre-conf (Data Collection) -> Conf (Final Content) -> Post-conf Month 1 (Compilation) -> Post-conf Month 2 (Archival).
    *   **Goal**: Publish within 2 months. Delay kills momentum.
*   **Staffing**:
    *   **The "Tech + Content" Split**:
        *   **Tech Chair**: Handles LaTeX, Python scripts, Git, and Zenodo API.
        *   **Content Chair**: Chases committee members for bios, logos, and front matter.
    *   **Skillset**: At least one chair MUST be proficient in LaTeX and Python. This is not a role for non-technical organizers.
*   **Data Collection**:
    *   **Heuristic: "Collect While They're Captive"**:
        *   **Problem**: People ghost you after the conference.
        *   **Solution**: Collect the "Front Matter" (Welcome Message, Volunteer List, Awards) *during* the conference week. Schedule a 30-minute meeting to force this.
*   **Deliverables**:
    *   **Posters**: Confirm specifications early (usually A0 portrait). Communicate this clearly to authors to avoid printing issues.
    *   **Fun Facts**: Collecting "fun facts" from authors for session intros is a nice touch. Keep it simple (1-3 facts) to avoid overwhelming session chairs.
*   **Proceedings**:
    *   **Platform**: Ensure proceedings are indexed and available (e.g., Zenodo, ACL Anthology).
    *   **Metadata**: Verify author names and affiliations carefully. This is a common source of post-conference correction requests.

## 3. Events & Programming

### Music Program & Concerts
*   **Curatorial Focus**:
    *   **MIR Integration**: Emphasize MIR integration as central to artistic merit. Submissions should demonstrate how technology shapes the art, not just use it as a prop.
    *   **Lecture-Concert**: Encourage formats where artists explain their tech/process (1-2 mins) before performing.
*   **Format & Logistics**:
    *   **Duration**: Set strict duration limits (e.g., <8 mins) to accommodate more performances and keep the audience engaged.
    *   **Tech Support**: Provide clear tech support/resources (PA, projector, basic backline) to lower barriers for performers. Request tech riders early.
*   **Inclusivity**:
    *   **Grants**: Use grants to promote diversity (geography, experience, need).
    *   **Waivers**: Explicitly state waiver policies in the CFP. Don't leave it ambiguous; artists often assume waivers are automatic.
*   **Integration**: Consider integrating with other events like Jam Sessions or Rencon to increase visibility and cross-pollination.

### Tutorials
*   **Content Strategy**:
    *   **Theme**: Align with conference theme but encourage introductory and inclusive topics to broaden appeal.
    *   **Selection**: Use weighted criteria (relevance, diversity, clarity). Select 2+ chairs from different backgrounds (industry/academia) to ensure balanced selection.
*   **Hybrid Delivery**:
    *   **Guidelines**: Provide clear guidelines for hybrid setups. At least one presenter should ideally be in-person.
    *   **Tech**: Ensure the venue has adequate AV for hybrid interaction (screens, mics for remote Q&A).
*   **Consent & Archiving**:
    *   **Timing**: Obtain recording/sharing consent **DURING** the proposal phase. Retroactive consent gathering is slow and painful.
    *   **Distinction**: Distinguish between "recording for conference" and "public YouTube archiving".

### Late Breaking Demos (LBD)
*   **Format**: In-person poster session is the standard. It's a low-barrier entry for prototypes and early-stage work.
*   **Capacity**:
    *   **Calculation**: Define capacity based on venue limits (boards * density * safety margin). Don't just pick a number.
    *   **Overflow**: Have a plan for overflow (e.g., waitlist, second session).
*   **System**:
    *   **Transparency**: OpenReview is recommended for transparency.
    *   **Screening**: Choose between Rolling (smooths load) or Batch (concentrates load) screening. Rolling is better for managing capacity but requires constant attention.
*   **Deliverables**: Require Poster (A0) and Thumbnail. Video is optional but good for archiving.

### Unconference
*   **Format**: Participant-driven discussions on emerging topics.
*   **Process**:
    *   **Voting**: Use voting (dot-voting or digital) to select topics that the community actually cares about.
    *   **Facilitation**: Recruit facilitators or "secretaries" to capture notes.
*   **Logistics**:
    *   **Noise**: Separate rooms are crucial to reduce noise bleed between groups.
    *   **Timing**: Evening timing with food/drinks often improves engagement and "loosens" the atmosphere.
*   **Follow-up**: Capture summaries and continue discussions on Slack to give the ideas a life beyond the session.

### Industry & Sponsorship
*   **Sponsorship Strategy**:
    *   **Tiers**: Define clear tiers and benefits (registrations, booths, logo placement).
    *   **Coordination**: Coordinate closely with Industry Chairs. Often these roles overlap or require constant sync.
*   **Industry Events**:
    *   **Booths**: Use raffles for fair assignment if space is limited.
    *   **Job Boards**: Promote widely. Consider privacy (self-hosted PDFs vs. hosted platforms).
    *   **Presentations**: Standardize formats and lengths (e.g., 8 mins Platinum, 4 mins Silver) to simplify operations.
    *   **Lightning Talks**: Great for engagement (1-min, 1-slide). Keeps the energy high and gives visibility to many sponsors.

## 4. Community & Support

### Diversity, Equity, & Inclusion (DEI)
*   **Mental Model: "The Matchmaker Hack"**:
    *   **Problem**: You will always have more mentees than mentors.
    *   **Solution**: Don't limit yourself to the signed-up mentor pool. **Cold-email authors** of papers relevant to a mentee's interest. Most are flattered and willing to do a one-off chat.
    *   **Philosophy**: Mentoring doesn't always mean "Senior Professor teaching Student". "Peer Mentoring" (connecting two students working on similar topics) is highly valuable.
*   **Accessibility**:
    *   **Data Collection**: Ask for access needs *during registration*, not after.
    *   **Quiet Rooms**: Mandatory. Conferences are overwhelming.
*   **Core Practices**:
    *   **Code of Conduct (CoC)**: Publish a short, accessible CoC. Designate named contacts (at least 2, diverse genders) and an anonymous reporting form.
    *   **Photo Consent**: Use simple visual indicators (e.g., colored lanyards or stickers) for opt-out. Communicate this policy clearly to all attendees and photographers.
*   **Outreach**:
    *   **Coordination**: Coordinate with Newcomer and WIMIR organizers to ensure their events are supported and promoted.
    *   **Integration**: DEI is not a standalone event; it should be embedded in all aspects (e.g., accessible slides, diverse session chairs).

### Volunteers / Travel Grants
*   **The "Critical Path" Principle**:
    *   **Concept**: Not all volunteer shifts are equal. "Checking badges" is low-risk. "Managing Presentation Slides" is critical.
    *   **Action**: Assign your most **tech-savvy** and reliable volunteers to the Audio/Visual shifts. Do not randomize this assignment.
*   **Shift Management**:
    *   **The "Handover"**: Volunteers are doing this for the first time. Schedule a 15-minute overlap between shifts so Volunteer A can teach Volunteer B the ropes.
    *   **No-Shows**: Expect 10-20% drop-off. Over-recruit.

### Travel Grants
*   **Criteria & Scoring**:
    *   **Rubrics**: Establish transparent, weighted scoring rubrics (e.g., +1 for Student, +1 for LMIC, +1 for First-time). This reduces bias and makes decisions defensible.
    *   **Categories**: Consider separate pools for Authors, WIMIR, and Diversity to ensure balanced support.
*   **Logistics**:
    *   **Hotels**: Block rooms 6-8 months in advance. Prices skyrocket closer to the date.
    *   **Confirmation**: Use multi-stage confirmation (email + form + LinkedIn if needed) to avoid wasted grants. Ghosting is common.
    *   **Travel Booking**: Consider fixed-amount grants ("up to $N") rather than pre-purchasing tickets. Pre-purchasing is logistically complex and budget-unpredictable.
    *   **Accommodation**: Explicitly state that accommodation grants are for **shared twin rooms**. Manage pairings carefully (collect preferences).

### Newcomer Initiatives
*   **Mentoring**:
    *   **Recruitment**: Recruit experienced attendees as mentors.
    *   **Pairing**: Use simple pairing algorithms (e.g., by research interest or language). Don't overcomplicate it.
*   **Squads**:
    *   **Concept**: Small groups ("squads") of newcomers led by a mentor are often more effective than 1:1 mentoring.
    *   **Catalyst**: Providing a free meal (lunch) for squads is a high-impact, low-cost way to foster bonding. It lowers the barrier for meeting up.

### Volunteer Management
*   **Recruitment**:
    *   **Roles**: Use clear role descriptions (e.g., "Session Runner", "Registration Desk").
    *   **Selection**: Balance between local students (logistics) and general attendees (community).
*   **Shifts**:
    *   **Duration**: One-day shifts are often better than multi-day. It allows volunteers to be "on duty" for one day and "attendees" for the rest, preventing burnout.
*   **Training**:
    *   **Manuals**: Provide detailed manuals and checklists for each role.
    *   **Briefing**: Hold an on-site briefing before the conference starts.
*   **Benefits**:
    *   **Standard**: Free registration is the standard benefit.
    *   **Bonus**: Accommodation support is a nice bonus if the budget allows, but prioritize grants for those in need.

## 5. Communication & Operations

### Website
*   **Mental Model: "The Content Pipeline"**:
    *   **Problem**: Web Chairs are developers, not copywriters. They shouldn't be writing text.
    *   **Solution**: Chairs draft content in **Google Docs**. Once approved, it is handed to the Web Chair for implementation.
    *   **Heuristic**: "CSV for Tables". If you have a list of 20 tutorials, give the Web Chair a CSV, not a PDF or a Word doc.
*   **Design**:
    *   **The "Reference Principle"**: Don't reinvent the wheel. Copy the menu structure and page layout of the *previous year's* website. It is battle-tested.
    *   **Mobile First**: 50% of attendees will check the schedule on their phone while walking to the venue.
*   **Lifecycle Management**:
    *   **Pre-Conference**: Focus on "Call for Participation", "Submission", and "Registration".
    *   **During Conference**: Switch to "Live" mode (schedule, links, daily updates).
    *   **Post-Conference**: Plan the transition to "Archive" mode in advance. The site should shift to showing awards, proceedings, and videos within 1-2 weeks. Don't leave a "Welcome!" page up for months after the event.
*   **Analytics**: Use tools like Google Analytics to track usage. This helps justify budget for web design and informs future navigation improvements.

### Social Media
*   **Mental Model: "The Waterfall Strategy"**:
    *   **Problem**: Announcing everything at once (CFP, Grants, Tutorials) causes information overload.
    **Solution**: Release announcements sequentially over a week.
        1.  **Save the Date** (General awareness)
        2.  **Major Program** (Tutorials/Keynotes)
        3.  **Support** (Grants - critical for inclusion)
        4.  **Urgent Calls** (Music/LBD with upcoming deadlines)
*   **The "Linkage Rule"**:
    *   **Concept**: Every post should link to a related opportunity.
    *   **Example**: "Call for Music" post should *also* mention "Grant Applications Open" because artists often need funding.
*   **Strategy**:
    *   **Platforms**: Use a mix (Twitter/X, LinkedIn, Instagram, Facebook) to reach different demographics. LinkedIn is growing for professional networking; Instagram for visuals.
    *   **Scheduling**: Use event-based scheduling (deadlines, keynotes, awards) rather than daily filler. Quality > Quantity.
*   **Sponsors**:
    *   **Integration**: Collect sponsor handles early. Tagging them in relevant posts (e.g., "Thanks to our Platinum sponsors") adds value to their sponsorship.
*   **Design**:
    *   **Templates**: Create templates that work across all platforms (e.g., 4:3 ratio images often crop well on most feeds).

### Registration System
*   **Integration**:
    *   **Data Flow**: Ensure the registration system talks to the website and submission systems. You need to validate that authors have registered.
*   **Waivers**:
    *   **Coordination**: Coordinate closely with Grants and Volunteer chairs. Manage waiver codes centrally to prevent abuse or double-dipping.

### Tech Stack & Tools
*   **Submission**:
    *   **OpenReview**: Preferred for transparency and modern interface.
    *   **CMT**: A robust alternative, often cheaper, but less user-friendly.
*   **Communication**:
    *   **Slack**: The standard for ISMIR. Create separate workspaces for "Organizers" (planning) and "Attendees" (conference).
*   **Virtual**:
    *   **Zoom**: Reliable for sessions.
    *   **YouTube**: Best for streaming and archiving due to familiarity and "DVR" features.

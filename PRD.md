Product Requirements Document (PRD)
FoundIt: A Campus Lost and Found Platform

Group name: Silver
Department / Group: Software Engineering, Group D
Course: COS209
Submitted by: Olukokun Temiloluwa David
Version: 0.1 
Status: Draft for review

Contents
Executive Summary
Problem Statement
Background and Context
How We Researched It
What We Found
Who Is Affected
What People Do Now
Goals and Success Metrics
Our Proposed Solution
The MVP
Functional Requirements
Non-Functional Requirements
Assumptions, Constraints and Risks
Open Questions
Rollout and Testing Plan
Technology Choice (Later)

1. Executive Summary

Almost everyone on campus has lost something at some point. Phones, ID cards, calculators, power banks, keys, bags, textbooks, wallets: they go missing in lecture halls, the library and the cafeteria every week. When it happens, getting the item back mostly comes down to luck. People post in WhatsApp groups, ask around, or check with security, and the person who found the item often has no idea who it belongs to or where to take it.

This document explains the problem, who it affects, how people deal with it today and why that does not work well. It then lays out our idea for a fix and the smallest first version of it (the MVP), along with the requirements, risks and a plan to test it.

We have not chosen a programming language or any technology yet. We want to be sure we understand the problem properly first.

2. Problem Statement

Who: Students, lecturers and staff who lose things, and the students, security staff and hall or hostel staff who find them
What: Lost items often never get back to their owners because there is no single place that everyone knows and trusts for lost and found reports
Where and when: Lecture halls, libraries, cafeterias, hostels, sports grounds, shuttle stops and walkways. It happens all semester but gets worse during exams and events
Impact: Money spent replacing phones, ID cards and calculators; missed exams when an ID card is gone; lost documents; stress; and items that finders would gladly return but cannot

In one sentence:

When something is lost or found on campus, there is no reliable, central way for the owner and the finder to find each other.

3. Background and Context
3.1 Our campus

Our campus is a residential university where most students live in hostels on or close to the school grounds, so a typical day involves moving between the hostel, lecture halls, the library, the cafeteria and sports areas. Students from different levels share these spaces, and lectures for a single class are often held in different halls on different days. That means students are constantly carrying things such as phones, calculators, ID cards, power banks and books from place to place, and things get left behind easily, especially when a class ends quickly or people rush to the next one.

Security posts are placed around the campus, and porters keep watch at the hostels and some buildings. As far as we could tell, there is no official lost and found desk that students widely know about. When something goes missing, students mostly post in class and hostel WhatsApp groups, ask coursemates, or check with security or the nearest office. Nothing connects these channels, so an item found in one place is rarely linked to someone searching in another.

3.2 What we observed ourselves

9 Nov 2026
Place: 200L class WhatsApp group
What we saw: Three "lost" posts in one afternoon (a calculator, a flash drive and an ID card). Each was buried under assignment and timetable messages within the hour.
What happened: None of the three posts got a reply. Two owners reposted the next day.
12 Nov 2026
Place: Porters' desk at a hostel
What we saw: A porter showed us a small box of items left with him by students, including a phone charger, a flash drive and a water bottle, with no list of who left what.
What happened: He said he only returns things when someone happens to ask, and has no way of telling who the real owner is.
16 Nov 2026
Place: Security post
What we saw: A paper register with a handful of items handed in over the past weeks, including two phones and several ID cards.
What happened: Staff said most items stay unclaimed because owners do not know to ask.
4. How We Researched It

4.1 Questions we wanted answered
How often do students lose things, and what do they lose most?
What do they do straight after they notice something is missing?
How often do they get it back, and how?
When someone finds an item, what do they do, and what stops them from returning it?
How do security staff and offices deal with found items, and what is hard about it?
What already exists, and where does it fall short?
4.2 Methods
Observation: Look at notice boards, security desks and group chats (with permission)
Survey: At least 20 to 30 students, using a Google Form or paper
Interviews: At least 3 students (one who lost something, one who found something), 1 security officer or porter, and an administrator if possible
Review of what exists: WhatsApp groups, notice boards, the security desk and any lost and found apps
4.3 Survey questions
What level are you? (100 / 200 / 300 / 400 / other)
Have you lost something on campus in the last year? (Yes / No)
What was it? (phone, ID card, calculator, bag, keys, wallet, laptop, books, other)
Where did you lose it? (lecture hall, library, cafeteria, hostel, other)
What did you do to find it? (tick all: asked around, posted in WhatsApp, went to security, checked a notice board, other)
Did you get it back? (Yes / No / Partly) How long did it take?
Have you ever found something that belonged to someone else? What did you do with it?
If you found something, what stopped you from returning it, if anything? (did not know who to give it to, afraid of being accused, no time, did not know the owner, other)
Do you know where to report a lost or found item on campus? (Yes / No)
How much did losing it cost you in money or time? (open answer)
Would you use a simple campus tool to report and search for lost and found items? (Yes / No / Maybe) What would make you trust it?
4.4 Interview guide
Student who lost something: Tell us about the last time you lost something. What happened in the first hour? The first day? Who did you tell? How did it end? What would have helped most?
Student who found something: What did you find and what did you do with it? How did you know who to give it to? Were you worried about returning it?
Security officer or porter: How do you handle and record found items? How do you check that someone is the real owner? What ends up unclaimed? What would make your work easier?
Administrator (optional): Is there an official lost and found policy? What happens to items nobody claims?

5. What We Found
5.1 Survey results

24 respondents (simulated). By level: 100L: 3, 200L: 10, 300L: 9, 400L: 2.

Lost something on campus in the past year: 17 of 24 (71%)
What was lost most (among those 17): ID cards 6, calculators 4, phones 3, power banks 2, keys 1, other 1
Where it was lost: Lecture halls 8, library 4, cafeteria 3, hostel 2
Got the item back fully: 5 of 17 (29%); partly 3 (18%); not at all 9 (53%)
Average time to get it back: About 3 days
Know where to report lost or found items: 7 of 24 (29%)
Found someone else's item: 15 of 24 (63%)
Of those 15, could not return it: 9 (60%)
Why finders could not return items: Did not know who to give it to (5), afraid of being accused (2), no time (2)
How owners searched: WhatsApp group posts (14), asking around (10), security (4), notice board (2)
Would use a dedicated tool: Yes 20 (83%), Maybe 3 (13%), No 1 (4%)
5.2 Interview notes
R3, 200L student (lost a calculator): Posted in four class WhatsApp groups before a test, but the messages got buried within minutes. Never found out if anyone picked it up.
R9, 300L student (lost an ID card): Needed it for an exam. Spent two days going from office to office. Had no idea a security post might be holding it.
R14, 200L student (found a phone): Had no idea whose it was. Posted in a group, and several people claimed it. Stopped replying because they were scared of giving it to the wrong person.
R18, 300L student (found a power bank): Left it with a coursemate, who later could not remember where it went.
S1, security officer: Keeps a paper register of items handed in. Many stay unclaimed because owners do not know to ask. Hard to tell who the real owner is.
5.3 What this tells us
Information is scattered. Owners depend on WhatsApp posts that disappear in busy groups, and only 29% of students know where to report a lost or found item.
Few people get their things back. Only about 3 in 10 owners fully recover what they lost, and it takes days.
Finders want to help but do not know how. Most do not know who to give the item to, or they worry about false claims and blame.
Proving ownership is the missing piece. Finders and security staff both struggle to confirm who the real owner is. This is why our MVP includes a verification step.
People want it. 83% said they would use a dedicated tool.
6. Who Is Affected
Owner (main user)
What they want: Get the item back fast, or at least know it was found
What frustrates them: Does not know where to report; group posts get buried; cannot tell if anyone found it
Limits they work under: Stressed and in a hurry (for example, needs an ID card for an exam); limited data
Finder (main user)
What they want: Return the item without hassle or suspicion
What frustrates them: Does not know the owner or where to take the item; worried about blame or wasted time
Limits they work under: Short on time
Security officers, porters and office staff
What they want: Record found items properly and give them to the right person
What frustrates them: Paper registers, unclear ownership, unclaimed items piling up
Limits they work under: Heavy workload, so the process must be simple
Student affairs / administration
What they want: A safer campus with fewer complaints and disputes
What frustrates them: Ends up handling disputes with little information
Limits they work under: Needs oversight and approval
Example user

Ada, 200-level student. She left her calculator and ID card in a lecture hall before a test. She posted in three WhatsApp groups and visited two offices, and still had no idea whether anyone had found them. A coursemate had actually picked them up but did not know whose they were.

7. What People Do Now (and Why It Does Not Work)
WhatsApp or Telegram groups
What is good about it: Fast, free, everyone uses it
Why it falls short: Messages get buried, reach is limited, no structure, and no way to check a claim
Notice boards
What is good about it: Visible and official
Why it falls short: Only people who walk past see them; they go out of date; you cannot search them
Security desk or porters' lodge
What is good about it: Items are kept safely
Why it falls short: Records are on paper, owners do not know to go there, and there is no clear way to verify them
Asking friends
What is good about it: Quick
Why it falls short: Small reach and unreliable

The gap: There is no single place where owners can search for what has been found, finders can report it in seconds, and ownership can be checked safely.

8. Goals and Success Metrics
8.1 Goals
Get more lost items back to their owners.
Cut the time between losing something and getting it back.
Make it easy and safe for finders to report what they find.
Reduce false claims.
8.2 How we would measure success (in a pilot)
Lost items fully recovered
Where we start (from our research): 29% (simulated survey)
Target: +30 percentage points
Average time to get an item back
Where we start (from our research): About 3 days (simulated survey)
Target: Under 48 hours
Students who know where to report
Where we start (from our research): 29% (simulated survey)
Target: 80%
Found items reported per week in the pilot
Where we start (from our research): n/a
Target: 15
Fraudulent claims
Where we start (from our research): Not measured
Target: Close to zero
8.3 What we are not doing (in version 1)
No payments or rewards.
It is not a crime or security reporting tool.
No tracking of items with GPS or tags.
9. Our Proposed Solution

FoundIt is a simple campus platform with two main actions: "I lost something" and "I found something."

An owner posts a lost item report. A finder posts what they found, with a photo and where it is being kept (for example, at a security post). The system then suggests likely matches. Because public listings can be abused, we hide the details that prove ownership, such as a serial number, a distinguishing mark or what is inside a bag. The owner has to supply those details before anything is handed over.

Principles we are designing around
Posting should take less than a minute.
It should work on low data and basic phones.
Handovers should be safe, with ownership verified and a security post as the preferred meeting point.
Keep personal details private by default.
10. The MVP (Version 1)
10.1 What is in
1. Report a lost item: Category, description, location, date, optional photo and a way to contact the owner
2. Report a found item: Category, description, photo and where the item is being kept
3. Browse and search: Search found items by category, location and date
4. Match suggestions: Points out likely matches between lost and found reports
5. Claim with verification: A claimant answers a hidden question set by the finder, and the finder or staff approve before any contact details are shared
6. Status tracking: Open, matched, returned or closed (expired)
7. Staff account: Security staff log items handed in and mark them as returned
10.2 What is left out for now

In-app chat, rewards, automatic image recognition, a link to the school ID database and live GPS maps.

10.3 User stories
US1: As an owner, I want to report a lost item quickly so that people know to look for it. Done when a report can be submitted in under a minute.
US2: As a finder, I want to post a found item with a photo and where it is kept so that the owner can find it. Done when the post shows the photo, category, location and drop-off point.
US3: As an owner, I want to search found items so that I can check whether mine was found. Done when search filters by category, location and date.
US4: As an owner, I want to claim an item safely so that nobody else can take it. Done when the claim needs the right answer to a hidden verification detail.
US5: As a finder, I want to approve or reject a claim so that the item goes to the right person. Done when contact details are shared only after approval.
US6: As a member of security staff, I want to log items handed in and mark returns so that our records are accurate. Done when staff can add items and set the status to returned.
US7: As an owner or finder, I want to get notified of a possible match so that I do not have to keep checking. Done when a notification is sent when a likely match is posted.
11. Functional Requirements
FR1: Users can create an account using their school email or matric number (Priority: Must; Story: All)
FR2: Users can post a lost item report (Priority: Must; Story: US1)
FR3: Users can post a found item report with a photo and drop-off location (Priority: Must; Story: US2)
FR4: Users can search and filter found items (Priority: Must; Story: US3)
FR5: The system suggests matches between lost and found reports (Priority: Should; Story: US7)
FR6: A claim flow with hidden verification details (Priority: Must; Story: US4)
FR7: Contact details are shared only after a claim is approved (Priority: Must; Story: US5)
FR8: Staff accounts can log found items and mark them as returned (Priority: Must; Story: US6)
FR9: Posts expire or are archived after a set time (for example, 60 days) (Priority: Should; Story: n/a)
FR10: Users can report suspicious or fake posts (Priority: Should; Story: n/a)
FR11: Notifications for matches and claim updates (Priority: Should; Story: US7)
12. Non-Functional Requirements
Ease of use: A first-time user can post an item in under a minute without help
Low data use: Photos are compressed and the app works on slow connections
Privacy and security: Hide sensitive item details and contact info until verified, protect passwords and store as little data as possible
Trust and safety: Moderation, a way to report suspicious posts, and a recommendation to hand items over at secure locations
Availability: Reliable during the working day, and shows saved listings when offline
Accessibility: Easy to read on small screens, in plain language
Growth: Starts with one campus or faculty but can grow
13. Assumptions, Constraints and Risks

What we are assuming

Students have a smartphone or can get to a computer.
Security staff are willing to take part.
Most finders will return items if it is easy enough.

Limits we are working within

A student project timeline and a small budget.
Unreliable network and power.
We would need campus approval to use security posts.

Risks

People just keep using WhatsApp
Likelihood: High
Impact: High
How we would handle it: Launch with security staff and class reps, and make it easy to share posts into existing groups
False claims or theft
Likelihood: Medium
Impact: High
How we would handle it: Hidden verification details, staff-assisted handover and a way to report suspicious claims
Privacy worries about photos and contacts
Likelihood: Medium
Impact: High
How we would handle it: Show minimal info and share contacts only after approval
Not enough found items get posted
Likelihood: Medium
Impact: High
How we would handle it: Make posting very fast and work with security desks
Spam or fake posts
Likelihood: Medium
Impact: Medium
How we would handle it: Verified accounts, moderation and reporting
Poor connectivity
Likelihood: High
Impact: Medium
How we would handle it: Light pages, compressed images and caching
14. Open Questions
Does the school already have an official lost and found process or office?
Where should found items be physically kept (security post or student affairs)?
Will security staff agree to log items and verify claims?
How long should unclaimed items be kept, and what happens to them afterwards?
15. Rollout and Testing Plan
1. Test the idea: Show paper or clickable mockups to 5 students and 1 security officer and collect feedback
2. Pilot: Run it for 3 to 4 weeks in one hostel, faculty or group of lecture halls, with a security post as the drop-off point
3. Measure: Compare the results with the numbers in Section 8.2
4. Decide: Improve it, expand it or change direction based on what we learn
16. Technology Choice (Later)

We have not picked a programming language, framework or platform. We will decide that after this PRD has been checked, based on the requirements above: low data use, photo uploads, notifications, privacy, our skill level and cost.
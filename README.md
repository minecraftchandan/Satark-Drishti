# Satark Drishti Authority

Build a modern, professional, trustworthy and visually impressive React.js frontend for a project called:

SATARK DRISHTI

Smart Real-Time Monitoring & Inspection Platform

Satark Drishti is a smart inspection and monitoring platform designed to make NGO/organization inspections more transparent, reliable and difficult to manipulate.

The frontend I am responsible for is the Authority Dashboard, which will be used by authorized officials to monitor organizations, inspections and inspection evidence.

CORE IDEA

Unlike conventional inspection-management systems that mainly store reports and records, Satark Drishti focuses on establishing whether an inspection is genuine and actually happened at the claimed location.

The system uses:

Random/unpredictable inspection scheduling

Live photo capture

GPS-based inspector presence verification

Inspection timestamps

Digital inspection records

Offline inspection and later synchronization

Live video monitoring when required

The frontend should communicate these concepts clearly without making unsupported claims about competitors.

DESIGN DIRECTION

Create a premium government-tech / modern SaaS dashboard.

The interface should feel:

Trustworthy

Secure

Professional

Modern

Clean

Reliable

Easy to understand

Suitable for an SIH (Smart India Hackathon) project presentation

Avoid making it look like a generic admin dashboard.

Use a clean visual hierarchy, elegant cards, subtle animations, rounded corners, modern typography, meaningful icons and excellent spacing.

Use a professional color system centered around deep navy/blue with white surfaces and subtle green indicators for verified/success states.

Include both light and dark visual elements where appropriate, but keep the overall interface highly readable.

Use Lucide React icons or another modern icon library.

AUTHORITY DASHBOARD

Create the main Authority Dashboard with:

Header

Satark Drishti logo/name

"Authority Portal"

Search

Notifications

Authority profile

Logout option

Sidebar Navigation

Include:

Dashboard

Organizations

Inspections

Random Schedule

Live Monitoring

Inspection Records

Evidence Verification

Offline Sync

Reports

Settings

The sidebar should collapse responsively.

DASHBOARD HOME

Create an attractive dashboard overview.

At the top:

Good Morning, Authority Officer 👋

Subtitle:

"Monitor inspections, verify evidence and maintain transparent organizational oversight."

Display important statistics in attractive cards:

Total Organizations

Example: 248

Inspections This Month

Example: 86

Verified Inspections

Example: 72

Pending Verification

Example: 9

Flagged Inspections

Example: 5

Offline Sync Pending

Example: 3

Use icons and subtle status indicators.

INSPECTION OVERVIEW

Create a large inspection analytics section.

Show:

Inspections over time

Verified vs pending inspections

Random inspections conducted

Flagged inspections

Use clean charts.

Include filters:

Today

This Week

This Month

Custom Range

RECENT INSPECTIONS

Create a professional table/card view showing:

Inspection ID

Organization

Inspector

Date

Time

GPS Status

Photo Status

Verification Status

Sync Status

Action

Example statuses:

🟢 Verified
🟡 Pending
🔴 Flagged
🔵 Synced
🟠 Offline Sync Pending

Each inspection should have a "View Details" button.

INSPECTION DETAILS PAGE

This is one of the most important pages.

When an authority official opens an inspection, show a complete evidence-oriented view.

Display:

Inspection Information

Inspection ID

Organization name

Inspector name

Scheduled time

Actual inspection time

Inspection duration

Inspection status

LOCATION VERIFICATION

Create a visually impressive map section.

Show:

Organization location

Inspector's captured GPS location

Verification radius/boundary

Distance between inspector and organization

GPS verification status

Example:

GPS VERIFIED

"Inspector was detected within the authorized inspection boundary."

Do not claim that GPS alone proves identity; present it as one layer of inspection evidence.

LIVE PHOTO EVIDENCE

Create a photo evidence section.

Display:

Captured inspection photo

Capture timestamp

GPS coordinates

Evidence ID

Add a clear badge:

LIVE CAPTURE

Also show:

"Captured during inspection"

instead of suggesting that the system can magically prove that an image has never been manipulated.

Include a fullscreen image viewer/modal.

EVIDENCE TIMELINE

Create a beautiful chronological timeline:

Random inspection scheduled

Inspector notified

Inspector reached location

GPS detected

Live photo captured

Inspection completed

Evidence synchronized

Authority reviewed record

This should visually communicate how Satark Drishti establishes an inspection trail.

RANDOM INSPECTION PAGE

Create a dedicated page explaining the random inspection system.

Show:

Random Inspection Engine

"Inspection timings are generated unpredictably to reduce the possibility of organizations preparing specifically for an inspection."

Include:

Upcoming randomized inspections

Completed random inspections

Inspection frequency

Schedule status

Organization

Assigned inspector

Time window

Use a visual "Randomized" indicator.

ORGANIZATIONS PAGE

Create a searchable organization directory.

Each organization card/table row should contain:

Organization name

Registration ID

Location

Last inspection

Next inspection status

Verification status

Risk/attention indicator

Number of inspections

Clicking an organization should open its profile.

ORGANIZATION PROFILE

Show:

Organization information

Address

Registration information

Location map

Inspection history

Verification history

Evidence records

Flagged events

Last inspection

Total inspections

Create a clean timeline of previous inspections.

LIVE MONITORING PAGE

Create a professional live-monitoring interface.

Show camera cards for organizations:

Organization name

Camera location

Online/Offline status

Last active time

Live indicator

Clicking a camera opens a larger video-monitoring interface.

Include:

LIVE badge

Timestamp

Camera name

Organization

Fullscreen button

Add a clear note:

"Live monitoring is available only to authorized officials."

OFFLINE SYNC PAGE

Create a page showing inspection data that was collected while offline.

Display:

Pending uploads

Successfully synchronized inspections

Failed synchronization

Last synchronization time

Connection status

Example:

3 inspections waiting for synchronization

Create a progress indicator.

When connection is restored, show:

Synchronization Complete ✓

This should visually communicate that inspections can continue even when connectivity is poor.

EVIDENCE VERIFICATION PAGE

Create a dedicated verification workspace.

Show an inspection's:

Photo

GPS location

Timestamp

Inspector

Organization

Inspection ID

Synchronization status

At the top, display an overall evidence status:

VERIFICATION STATUS: VERIFIED

Break the evidence into individual components:

✓ Location evidence
✓ Timestamp recorded
✓ Live photo captured
✓ Inspection record synchronized

Do not use exaggerated claims such as "100% fraud-proof."

REPORTS PAGE

Create a reporting dashboard with:

Total inspections

Verified inspections

Pending inspections

Flagged inspections

Organizations inspected

Random inspections

Offline inspections

Synchronization statistics

Allow filtering by:

Date

Organization

Inspector

Verification status

Include an Export Report button.

IMPORTANT UI FEATURE

Create a reusable Inspection Evidence Card component.

It should visually combine:

📍 GPS
📸 Photo
⏱ Timestamp
👤 Inspector
🏢 Organization
☁ Sync Status

The purpose is to communicate the central idea of Satark Drishti:

"Inspection evidence should tell the complete story, not just provide a report."

RESPONSIVE DESIGN

The entire website must be responsive.

Desktop:

Full sidebar

Large dashboard

Tables

Charts

Maps

Tablet:

Collapsible sidebar

Responsive cards

Mobile:

Bottom navigation or collapsible menu

Stacked cards

Mobile-friendly inspection evidence

Responsive maps and photos

MICRO-INTERACTIONS

Add subtle professional animations:

Card hover effects

Smooth page transitions

Sidebar transitions

Loading skeletons

Success animations

Verification animation

GPS verification indicator

Sync progress animation

Toast notifications

Do NOT overuse animations.

The website should feel like a serious professional monitoring platform rather than a flashy marketing website.

DEMO DATA

Use realistic dummy data for the frontend.

Example organizations:

Seva Foundation

Udaan Welfare Society

Jan Kalyan Trust

Shakti Rural Development Centre

Hope Community Foundation

Use fictional inspectors and fictional GPS coordinates.

Clearly treat all data as demonstration data.

TECHNICAL REQUIREMENTS

Use:

React.js

React Router

Tailwind CSS

Lucide React icons

Recharts for charts

Leaflet or another suitable map library

Reusable React components

Clean component architecture

Responsive design

Mock JSON/local state for demonstration data

Structure the project cleanly with reusable components such as:

Sidebar

Header

StatCard

InspectionTable

InspectionEvidenceCard

VerificationBadge

OrganizationCard

GPSVerificationCard

PhotoEvidence

InspectionTimeline

LiveCameraCard

SyncStatus

MapView

Charts

Keep the code modular and easy to connect to a backend/API later.

BRANDING

Project name:

SATARK DRISHTI

Tagline:

"Verify. Monitor. Trust."

Alternative supporting line:

Smart Real-Time Monitoring & Inspection

Use a simple eye/shield/location-inspired logo concept.

The overall visual identity should communicate:

Transparency + Verification + Technology + Trust

MOST IMPORTANT REQUIREMENT

The website should immediately communicate what makes Satark Drishti different.

The central message should be:

Conventional systems primarily manage inspection information.

Satark Drishti focuses on strengthening the authenticity of inspection evidence.

Visually emphasize these four differentiators:

🎲 Random Inspection Scheduling
📸 Live Photo Capture
📍 GPS-Based Presence Verification
📡 Offline Inspection + Automatic Synchronization

Build the frontend as if it will be demonstrated to an SIH jury.

The result should look like a real deployable authority monitoring platform, not a basic student CRUD project.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```

# Understand It Brief: SBFH Twitter Content Selection Experience

**Date:** 2026-03-13  
**Author:** Product Agent  
**Scenario Owner:** SBFH  
**Trigger:** Odoo Card #40400000005

---

## Problem Statement

SBFH (content manager) wants to share engaging content on Twitter to maximize visibility and engagement, but the current Nextcloud experience creates significant friction in identifying, selecting, and preparing the right assets for publishing.

## User & Context

- **Primary User:** SBFH (content manager)
- **Goal:** Publish Twitter content that has potential to go viral and fits the brand story
- **Current Tool:** Nextcloud (with embedded editing capabilities)
- **Content Type:** Images, including iOS Live Photos

## Key Pain Points (Observed)

### 1. Discovery & Selection Friction
- **Live Photo Preview Issue:** iOS Live Photos display a large play icon instead of thumbnails, preventing quick visual scanning
- **Comparison Difficulty:** User must switch back and forth between similar images to evaluate options
- **Decision Paralysis:** Uncertainty about which image will resonate most ("He thinks which one of these pictures will buzz?")

### 2. Editing Limitations
- **Linear Workflow Only:** Can only apply one edit step at a time (e.g., rotate → save → crop as separate steps)
- **No Visual Feedback:** Edit outputs are not visible until page refresh
- **Mental Model Break:** User fears losing files ("Where's my file????") during multi-step edits
- **State Management:** Need to save intermediate versions manually

### 3. Asset Tracking & Audit
- **Download Confusion:** After selecting and downloading multiple files, user cannot recall which ones were chosen ("I just uploaded two of these but i don't even know which ones anymore?")
- **No Version/Selection History:** No clear audit trail of selected/downloaded assets

## Opportunity

Build a streamlined content curation workflow for Twitter that enables:
1. **Better Visual Discovery:** Proper thumbnail rendering for all image types (including Live Photos)
2. **Multi-Image Comparison:** Side-by-side or carousel view for rapid comparison
3. **Non-Destructive Multi-Step Editing:** Preview edit results in real-time without page refresh
4. **File State Assurance:** Clear visual feedback that files are preserved during editing
5. **Selection Tracking:** Persistent tracking of selected/downloaded assets with ability to review choices

## Success Metrics

- **Selection Time:** Reduce time from opening folder to selecting final assets
- **Edit Abandonment:** Decrease fear-related drops during multi-step editing
- **Asset Clarity:** User can recall which files were selected within 1 hour post-selection (reduction in confusion)
- **Publication Confidence:** User reports higher confidence that chosen content fits viral potential

## Scope

### In Scope (for MVP)
- Thumbnail rendering improvements for iOS Live Photos
- Side-by-side image comparison view
- Real-time preview of edit operations
- Visual indicators that edited files are preserved
- Simple selection history/tracking view

### Out of Scope (for now)
- Viral prediction algorithms
- Full social media scheduling integration
- Advanced collaborative editing

## Assumptions

1. The "Nextcloud" environment supports custom UI components or integrations for the product team to build upon
2. iOS Live Photos are a significant portion of the user's content library
3. Twitter is the primary publishing channel for this user segment
4. The user has moderate technical comfort but values speed and certainty over granular control

## Open Questions

1. What is the typical batch size of images users evaluate before publishing to Twitter?
2. What edit operations are most commonly requested (crop, rotate, filters, etc.)?
3. Is this a one-time content manager (SBFH) or are there multiple users with similar needs?
4. Are there existing metrics on Live Photo adoption rates in the user base?
5. What is the current file format compatibility with Twitter's upload requirements?

## Next Steps

1. **Research:** Validate pain points with additional users (target: 5-8 content managers)
2. **Design:** Create low-fidelity mockups for improved thumbnail display and multi-step editing
3. **Prototype:** Build a quick prototype for Live Photo thumbnail rendering
4. **Testing:** Conduct usability tests comparing current vs. proposed workflows
5. **Roadmap:** Define MVP feature set and timeline

## References

- Odoo Card #40400000005 (original trigger)
- Product Repository: roger-rorobot/product-base

---

**Status:** Draft - Ready for stakeholder review  
**Priority:** High (directly impacts user ability to publish content)
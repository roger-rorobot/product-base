# SBFH Twitter Content Selection and Management

## Problem or Opportunity

SBFH (Small Business Founder/Owner) needs to share content on Twitter to gain visibility and engagement, but faces significant pain points during content selection and publishing:

1. **Poor visual feedback when selecting content**: Unable to see thumbnails properly (especially for iOS Live Photos which show a large play icon instead), making it difficult to identify the right content.
2. **Cumbersome multi-step editing**: The editor only allows one edit step at a time, requiring users to save after each operation and refresh to see results.
3. **Lack of file tracking and history**: After edits and operations, users lose track of which files they've uploaded or published.
4. **No persistent favorites system**: Users discover favorites only after the fact, with no integrated workflow to mark content for future use.

## Who benefits

- **Small business owners/managers** who need to regularly publish social media content
- **Content marketers** managing multiple assets across platforms
- **Users with iOS devices** who rely on Live Photos and need better visual previews
- **Anyone who needs to quickly identify, edit, and publish engaging content**

## Why this matters

Solving these issues will:
- **Reduce cognitive load** and time spent selecting content for social media
- **Prevent data loss anxiety** by providing immediate visual feedback and clear file status
- **Enable efficient multi-step editing** workflows without intermediate saves
- **Improve content performance** by making it easier to identify and select high-potential content
- **Provide auditability** so users know exactly what they've published

## Desired outcomes

1. **Faster content selection**: Users can quickly browse and identify suitable content through improved visual previews (thumbnails for regular photos, proper live photo handling).
2. **Seamless multi-step editing**: Users can apply multiple edits in sequence without intermediate saves or page refreshes, with all changes visible in real-time.
3. **Clear content tracking**: Users can immediately see what content has been uploaded/published and maintain a record of their publishing history.
4. **Better content discovery**: Integrated "Favorite" functionality allows users to flag promising content early in the workflow.

## Success metrics

- **Selection time reduction**: 50% reduction in time spent browsing and selecting content for Twitter
- **Edit completion rate**: 100% of multi-step edit sequences completed without user-perceived data loss
- **Published content tracking**: 90% of users can correctly identify what content they've published within 5 minutes
- **Live photo preview success rate**: 100% of Live Photos display appropriate preview (not just play icon)

## Proposed approach

1. **Enhanced preview system**: Implement thumbnail generation for all image types, with special handling for iOS Live Photos to show representative frames rather than just a play icon.

2. **Multi-step editing with live preview**: Allow users to queue multiple edit operations (rotate, crop, filter, etc.) and see the cumulative result in real-time without intermediate saves. Only save upon final confirmation.

3. **File status and history tracking**: Add a persistent view showing:
   - Recent uploads and their status (published, scheduled, draft)
   - Edit history for each file
   - Favorites marked for quick access

4. **Integrated favorites workflow**: Make the "Favorite" button visible and accessible from the beginning of the workflow, not as a discovery feature.

## Stakeholders

- **Product team**: Owner of content management features
- **Engineering team**: Implementation of editing and preview improvements
- **Design team**: UX improvements for visual browsing and editing
- **Customer Success**: Supporting users during transition
- **SBFH users**: Primary beneficiaries

## Dependencies and blockers

- **Dependencies**:
  - iOS Live Photo handling from media library team
  - Backend support for persistent edit session state
  - Frontend improvements to preview rendering
  - Database schema updates for favorites and publishing history
  
- **Blockers**:
  - Current editor architecture limitations requiring page refreshes
  - No existing thumbnail generation pipeline for Live Photos
  - Lack of centralized content state tracking

## Complexity

High ⚖️ Detailed rationale: This involves multiple subsystems (media preview, editing engine, file state management, user history tracking) and requires coordinated changes across frontend and backend. The editing workflow change is particularly complex as it requires stateful session management.

## Next steps

1. Conduct user research to validate specific pain points with current workflow
2. Design mockups for improved preview and editing interfaces
3. Technical spike on multi-step editing architecture
4. Prioritize Live Photo thumbnail fix as quick win
5. Define API contracts for content state tracking

## Assumptions

- The "SBFH" user persona represents small business owners managing their own social media
- iOS Live Photos represent a significant portion of user content (based on the user's complaint)
- Users are currently using Nextcloud as their content management platform
- The current editor is a Nextcloud app with single-operation limitation
- Twitter publishing is the primary use case but improvements should benefit other platforms
- Users have basic image editing needs (rotate, crop, filter) rather than advanced editing

## Open questions

1. What other platforms beyond Twitter need to be supported?
2. Are there specific Live Photo handling requirements from iOS/Apple guidelines?
3. What is the expected scale of users who perform multi-step edits?
4. Should edit history be version-controlled (allowing rollback) or just sequential?
5. What integration points exist with Twitter's publishing API?

## Quality bar

A good answer is:
- Grounded in the provided context of user pain points
- Useful without being overly speculative about technical implementation
- Explicit about the multi-system nature of the solution
- Structured so it can be stored directly in the product repo as an actionable brief

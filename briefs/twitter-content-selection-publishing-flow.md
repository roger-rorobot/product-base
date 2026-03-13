# Twitter Content Selection and Publishing Flow - SBFH Persona

## Problem or opportunity
SBFH (Social Media Content Manager) needs to select engaging content from their media library for Twitter posting but struggles with:
- Poor visual feedback when browsing images (especially iOS Live Photos), where thumbnails are obscured by play icons
- Limited non-destructive editing capabilities (can only apply one edit step at a time, requiring sequential saves)
- Unclear file status after edits (fears losing files, no visible outputs until page refresh)
- Lack of tracking which images have already been published, leading to potential duplicate posts

## Who benefits
- Social media managers who need to quickly identify and publish engaging content
- Content creators who want to experiment with edits without losing original files
- Teams managing multi-platform content strategies

## Why this matters
The current workflow creates significant friction in content publishing decisions. SBFH spends excessive time trying to preview thumbnails and perform basic edits, leading to:
- Reduced productivity and increased frustration
- Risk of publishing duplicate content (unable to track what's already posted)
- Missed opportunities for timely, engaging content due to poor tool UX
- Potential file loss anxiety affecting decision-making confidence

## Desired outcomes
- SBFH can quickly preview all available content including iOS Live Photos with clear thumbnails
- Seamless multi-step editing with visible results and undo capabilities
- Clear tracking of published vs. unpublished content to prevent duplicates
- Streamlined workflow for immediate posting and scheduling within the same interface

## Success measures
- Time-to-publish metric: Reduce average content selection to publish time from current state to under 3 minutes
- Editor satisfaction score: 80%+ of users report confidence they haven't lost their file after edits
- Duplicate rate: Zero instances of accidentally publishing the same content twice in a given week

## Proposed approach
1. **Enhanced thumbnail preview**: Replace play icon overlay with visible thumbnail preview for all media types including Live Photos
2. **Non-destructive multi-step editing**: Implement real-time editing with visible step-by-step results and automatic save history
3. **Publication tracking system**: Add "Published" status indicators and searchable history of recently published content
4. **Unified workflow**: Combine content selection, editing, preview, and publishing/scheduling in a single coherent interface

## Stakeholders
- Social Media Team (primary users)
- Content Management Team
- Engineering (product implementation)
- UX Design

## Dependencies and blockers
- Dependencies:
  - Nextcloud API capabilities for media preview and editing
  - Backend infrastructure for real-time edit previews and file versioning
  - Twitter API integration for posting and scheduling
- Blockers:
  - Current editor limitations may require refactoring to support non-linear editing
  - Need clarification on file storage architecture to implement proper tracking

## Complexity
High — Requires changes to multiple system components (media viewer, editor, publication tracking) and potential backend refactoring for real-time state management.

## Next steps
1. Conduct user research with SBFH persona to validate pain points and gather specific requirements
2. Prototype new thumbnail preview behavior for iOS Live Photos
3. Define technical approach for non-destructive multi-step editing
4. Create wireframes for unified content publishing workflow

## Assumptions
- The user mentioned (SBFH) represents a specific persona of social media content managers
- The current Nextcloud instance is the primary content repository for social media assets
- Twitter is the target platform for this initial workflow improvement
- Users may not distinguish between "publishing" and "scheduling" operations
- File loss anxiety is a UX issue rather than an actual data integrity problem

## Open questions
- Are there other social platforms besides Twitter that this workflow should support?
- What is the typical volume of content being managed per week?
- Are there brand guidelines or approval processes that need to be integrated?
- What is the current timeline for Twitter API rate limits that might affect batch operations?

## Quality bar
A good answer is:
- grounded in the provided context,
- useful without being overlong,
- explicit about uncertainty,
- structured so it can be stored directly in the product repo.

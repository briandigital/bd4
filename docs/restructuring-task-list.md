# Jekyll Portfolio Restructuring - Task List

## Project Overview
Restructure the existing Jekyll portfolio site to move the professional summary to the home page and reorganize navigation, while maintaining all visual styling and case study pages.

## Current vs Proposed Structure

**Current Structure:**
- Home (blog index) → 2 blog posts
- About (standalone)
- Portfolio (professional summary + links) → 6 case studies + Resume

**Proposed Structure:**
- Home (professional summary) → Resume + 6 case studies
- About (unchanged)

## Phase 1: Content Migration and Structure Changes
**Check-in Point 1:** After completing all content migration tasks

### Task 1.1: Move Professional Summary to Home Page
- Copy the professional summary content from `portfolio/index.md` 
- Replace the current blog index content in `index.html` with this professional summary
- Update the front matter to reflect it's now a home page, not a blog index

### Task 1.2: Remove Blog Functionality
- Delete the two blog posts in `_posts/` directory
- Remove blog-related includes from the index layout (pagination, post loops)
- Update `_config.yml` to remove blog-related settings (paginate, etc.)

### Task 1.3: Update Navigation Structure
- Modify the sidebar navigation to reflect new structure
- Home should link to the new professional summary page
- About should remain as is
- Portfolio section should be removed (since case studies will be under Home)

## Phase 2: Case Study Integration
**Check-in Point 2:** After completing case study integration

### Task 2.1: Integrate Case Studies Under Home
- Update the home page layout to include links to all 6 case studies
- Ensure case study pages remain as individual pages with their current URLs
- Update any internal navigation that references the old portfolio structure

### Task 2.2: Add Resume Link
- Add resume link to the home page navigation
- Ensure resume page remains accessible at its current URL

## Phase 3: Cleanup and Testing
**Check-in Point 3:** After completing cleanup and before final testing

### Task 3.1: Remove Portfolio Collection
- Remove portfolio-specific layouts that are no longer needed
- Clean up any portfolio-specific includes or templates
- Update any remaining references to the old portfolio structure

### Task 3.2: Test Site Structure
- Verify all pages are accessible
- Check that navigation works correctly
- Ensure no broken links remain

## Technical Constraints
- **No visual changes** - maintain current Hydeout theme exactly as is
- **No CSS modifications** unless absolutely necessary for functionality
- **Preserve all existing URLs** for case studies and resume
- **Keep About page unchanged** in both content and navigation
- **Focus only on content reorganization and navigation updates**

## Check-in Protocol
At each check-in point, Cursor should:
1. Show you the specific files that were changed
2. Explain what was done in simple terms
3. Ask if you want to review the changes before proceeding
4. Wait for your approval before moving to the next phase

## Files to be Modified
- `index.html` - Convert from blog index to professional summary
- `_config.yml` - Remove blog-related settings
- `_layouts/index.html` - Update layout for new home page content
- `_includes/` - Update navigation includes
- `_posts/` - Remove blog posts
- `portfolio/index.md` - Content will be moved to home page

## Files to be Preserved
- All case study pages in `portfolio/` directory
- `about.md` - No changes
- `resume.md` - No changes
- All theme files in `_sass/` and `assets/` - No visual changes 
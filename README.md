# EODHD Trump Trade Analysis Implementation Guide

This README contains instructions for implementing the visualization hub for your EODHD Trump Trade Analysis project.

## Files Created

1. `index.html` - Main navigation page with cards for each visualization
2. `combined.html` - Single page that displays all visualizations using iframes

## Implementation Steps

### 1. Upload the HTML Files

Upload the two HTML files (`index.html` and `combined.html`) to your GitHub repository:
- https://github.com/andrewpaulavets/EODHD_Trump/

### 2. Check for Cross-Origin Issues with iFrames

The `combined.html` file uses iframes to display all visualizations. If you encounter any cross-origin issues (which is unlikely since everything is hosted on the same GitHub Pages domain), you may need to adjust your GitHub Pages settings.

### 3. Test the Pages

Once uploaded, test your pages at:
- Main page: https://andrewpaulavets.github.io/EODHD_Trump/index.html
- Combined view: https://andrewpaulavets.github.io/EODHD_Trump/combined.html

### 4. Alternative Implementation (No iFrames)

If you prefer not to use iframes in the combined view, you would need to:

1. Extract the main content from each HTML file
2. Combine them into a single HTML file
3. Deduplicate any JavaScript libraries they share
4. Ensure each visualization has a unique ID to prevent conflicts

This is more complex and would require a custom script to properly extract and combine the visualization code. The iframe approach is simpler and provides better isolation between visualizations.

## Making Updates

When you add new visualizations:

1. Update the `index.html` file by adding new card entries
2. Update the `combined.html` file by adding new section and navigation entries

## Set as Default Page

To make `index.html` your repository's default page, either:
- Rename it to `index.html` at the root level
- Configure GitHub Pages settings to use it as the default page

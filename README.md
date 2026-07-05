# Frontend-Assignment-Convert-Figma-Design-to-HTML-CSS-
Sport World - Frontend Landing Page

[cite_start]A semantic, responsive, and framework-free sports news landing page built entirely with vanilla HTML5 and CSS3[cite: 10, 21]. [cite_start]The project translates a structured sports platform design into a fluid web experience optimized for desktop, tablet, and mobile displays[cite: 4, 27].



<img width="1342" height="3909" alt="_C__Users_Codeline%20Comp_Desktop_convert%20figma%20to%20HTML%20 %20CSS_index html" src="https://github.com/user-attachments/assets/723976a7-834c-442f-92c5-1f53fe31627b" />
## 🚀 How to Run the Project

Follow these steps to initialize and review the project locally:
1. **Verify Folder Hierarchy**
   [cite_start]Ensure your local workspace matches the required assignment folder structure[cite: 43]:
   ```text
   project/
   ├── index.html
   ├── css/
   │   └── style.css
   ├── images/
   │   ├── logo1.webp
   │   ├── sport1.webp
   │   ├── football.webp
   │   ├── basketball.webp
   │   ├── Tennis.webp
   │   ├── sport_now.webp
   │   ├── world_cup.webp
   │   ├── Summer_Mercato.webp
   │   ├── Lamin Yamal.webp
   │   ├── Neymar.webp
   │   └── Kylian Mbappe.webp
   └── README.md

   🛠️ Challenges Faced & Core Solutions1.
   Cascade Redundancy & Conflicting @media RulesChallenge: The stylesheet contained duplicated, overlapping definitions for the 768px tablet view breakpoint. This created ordering issues where flex directions for .site-footer and container rules conflicted with each other during responsive downscaling.Solution: Cleaned and unified the cascading layout rules inside the CSS architecture. Consolidated duplicate blocks under a single @media (max-width: 768px) umbrella to maintain an expected code sequence and predictable inheritance behavior.  2. Aspect Ratio Drift Across Differing Card ContentsChallenge: Varying paragraph sizes for different sports cards (e.g., Football vs. Basketball) caused container boxes to stretching unevenly, breaking row alignment.  Solution: Applied strict wrapper constraints utilizing CSS properties (aspect-ratio: 1 / 1 for small content thumbnails and 16 / 9 for widescreen panels) combined with object-fit: cover. This isolates image rendering mechanics completely from raw text lengths, keeping components consistent.  3. Preserving Avatar Proportions Inside Circular FramesChallenge: Player portraits extracted from source assets scaled irregularly when bound to circular layout borders (border-radius: 50%), causing distortion.Solution: Defined explicit square bounding parameters (width: 40px; height: 40px;) while declaring object-fit: cover directly on the avatar elements. This locks the image positioning context inside the element dimensions, keeping avatars circular across device screen widths.



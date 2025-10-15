# Week 01 — Project (Author + Front-End)

**Theme:** Setup • WordPress + GitHub Foundations  
*Goal:* Produce a single, reviewable outcome that integrates this week’s authoring and front-end work. Follow the steps exactly and submit via Pull Request.

---

## Prerequisites
- You completed `week01/exercise.md` on a feature branch.
- Your LocalWP site is running and reachable.

---

## PART A — Authoring (do all steps)

1) Build the target page(s)
   - Target: **About Us** page + one sample **Post** (with Tags/Categories).
   - Insert required blocks exactly as specified in `week01/exercise.md`.
   - Save as **Draft** first.

2) Apply metadata & taxonomy
   - Set **Featured Image** where required.
   - For each image on the page(s), add **ALT text**.
   - Ensure **Category** and **Tags** match this week’s instructions.

3) Publish & verify
   - Click **Publish** → **Publish**.
   - Open the public URL(s) and confirm all content renders and links work.

**Acceptance criteria (Authoring)**
- [X] Required blocks present and in correct order  
- [X] Featured Image set; images have ALT text  
- [X] Correct Category + Tags  
- [X] Published and reachable; required links work

---

## PART B — Front-End (do all steps)

1) Locate and adjust files
   - Open folder: Theme or plugin folder where your changes live (document exact path).
   - Edit files as needed (e.g., `style.scss`, `edit.js`, `save.js`) to support the project goal.

2) Build assets (if applicable)
   - **Windows (Jeff)**
     ```bat
     cd C:\Users\<yourname>\Local Sites\aem-lab\app\public\wp-content
     ```
     (cd further into your theme/plugin; then:)
     ```
     npm install
     npm run build
     ```
   - **macOS (Mattie & Melanie)**
     ```bash
     cd ~/Local\ Sites/aem-lab/app/public/wp-content
     ```
     (cd further into your theme/plugin; then:)
     ```
     npm install
     npm run build
     ```

3) Validate changes
   - Hard-refresh the page(s) (Windows: Ctrl+F5; macOS: Cmd+Shift+R).
   - Confirm visual and/or behavioral changes are visible.

**Acceptance criteria (Front-End)**
- [X] File(s) edited with clear, minimal changes  
- [X] Build runs without errors and updates are visible  
- [X] A concrete visual/a11y/perf improvement is demonstrated

---

## PART C — Integration & QA

1) Integration test
   - Confirm authoring and front-end outputs work together (no broken styles, attributes applied, layout correct).

2) Quick QA
   - Check semantic headings (H1 → H2 → H3).  
   - Verify link targets and button labels are descriptive.  
   - Re-test keyboard tab order across the page(s).

**Acceptance criteria (Integration & QA)**
- [X] No layout breaks or console errors  
- [X] Semantic heading order  
- [X] Descriptive links/buttons  
- [X] Logical keyboard flow

---

## PART D — Documentation

1) Author Notes (add to this file)
   - Steps for creating and publishing pages in WordPress.  
   - How to add ALT text and Featured Images.

2) Developer Notes (add to this file)
   - Local WP path: `C:\Users\Jeff\Local Sites\aem-lab\app\public\`  
   - Repo path: `aem-jeff-course/week01/`  
   - GitHub flow: commit → push → PR → merge.

**Acceptance criteria (Docs)**
- [X] Author Notes: clear and task-oriented  
- [X] Developer Notes: exact paths + commands + rationale

---

## Deliverables (save files here)

- Screenshots in `week01/screenshots/`:
1. `screenshots/week01_project_localwp-running_jeff.png` — LocalWP app showing site running  
2. `screenshots/week01_project_wp-dashboard_jeff.png` — WP Admin Dashboard  
3. `screenshots/week01_project_repo-folder_jeff.png` — Local repo in Explorer/Finder  
4. `screenshots/week01_project_pr-page_jeff.png` — Pull Request on GitHub

---

## Git & Submission (no abbreviations)

1) **Branch**
   - `jeff/week-01-project`  
2) **Commit**
   - `Week 01 Project: Environment verification and workflow test`  
3) **Pull Request**
   - Title: `[JEFF][WEEK01] Project Submission`  
   - Description: link to published About Us page + screenshots 

4) Submit the **PR URL** in the course thread.

**Acceptance criteria (Submission)**
- [X] Branch named correctly  
- [X] Commit message descriptive  
- [X] PR title and description follow the format  
- [X] PR URL posted

---

## 🧠 AEM Alignment Summary

| Area | WordPress / Front-End Activity | AEM Equivalent | Concept Demonstrated |
|------|-------------------------------|----------------|----------------------|
| Environment | LocalWP + GitHub setup | Author + Cloud Manager | Platform foundation |
| Authoring | About Us page + taxonomy | Templates + Tags | Structured authoring |
| Version control | Commit + PR | Code promotion | Workflow alignment |
| Documentation | Author + Dev notes | Runbooks / Author Guides | Governance |

---

## ✅ Final Checklist
- [ ] PART A complete  
- [ ] PART B complete  
- [ ] PART C complete  
- [ ] PART D complete  
- [ ] 4 screenshots saved with exact names  
- [ ] Branch pushed, PR opened, URL posted

---

### 📝 Narrative (3–6 sentences)
This project validated my entire environment from LocalWP through GitHub.  
I confirmed I could create, publish, and tag content locally while tracking changes in a remote repository.  
Committing through a branch and submitting a Pull Request mirrored how AEM teams manage code promotion.  
Having both author and developer notes in one file reinforced the collaboration expected in AEM workflows.

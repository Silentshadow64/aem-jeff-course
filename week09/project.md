# Week 09 — Project (Author + Front-End)

**Theme:** Performance • Images, Lazy Loading, Structure  
*Goal:* Produce a single, reviewable outcome that integrates this week’s authoring and front-end work. Follow the steps exactly and submit via Pull Request.

---

## Prerequisites
- You completed `week09/exercise.md` on a feature branch.
- Your LocalWP site is running and reachable.

---

## PART A — Authoring (do all steps)

1) Build the target page(s)
   - Target: A page with **optimized images** and cleaned **DOM structure**.
   - Insert required blocks exactly as specified in `week09/exercise.md`.
   - Save as **Draft** first.

2) Apply metadata & taxonomy
   - Set **Featured Image** where required.
   - For each image on the page(s), add **ALT text**.
   - Ensure **Category** and **Tags** match this week’s instructions.

3) Publish & verify
   - Click **Publish** → **Publish**.
   - Open the public URL(s) and confirm all content renders and links work.

**Acceptance criteria (Authoring)**
- [ ] Required blocks present and in correct order  
- [ ] Featured Image set; images have ALT text  
- [ ] Correct Category + Tags  
- [ ] Published and reachable; required links work

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
- [ ] File(s) edited with clear, minimal changes  
- [ ] Build runs without errors and updates are visible  
- [ ] A concrete visual/a11y/perf improvement is demonstrated

---

## PART C — Integration & QA

1) Integration test
   - Confirm authoring and front-end outputs work together (no broken styles, attributes applied, layout correct).

2) Quick QA
   - Check semantic headings (H1 → H2 → H3).  
   - Verify link targets and button labels are descriptive.  
   - Re-test keyboard tab order across the page(s).

**Acceptance criteria (Integration & QA)**
- [ ] No layout breaks or console errors  
- [ ] Semantic heading order  
- [ ] Descriptive links/buttons  
- [ ] Logical keyboard flow

---

## PART D — Documentation

1) Author Notes (add to this file)
   - Step-by-step authoring instructions (edit, update, reuse).  
   - Guardrails (content limits, image ratios, naming).

2) Developer Notes (add to this file)
   - File paths edited and why.  
   - Build steps and any attribute mappings used.

**Acceptance criteria (Docs)**
- [ ] Author Notes: clear and task-oriented  
- [ ] Developer Notes: exact paths + commands + rationale

---

## Deliverables (save files here)

- Screenshots in `week09/screenshots/`:
  1. `week09_project_editor_<yourname>.png` — editor view  
  2. `week09_project_published_<yourname>.png` — published page  
  3. `week09_project_pr_<yourname>.png` — Pull Request page  
  4. `week09_project_structure_<yourname>.png` — file/folder view showing edited files

---

## Git & Submission (no abbreviations)

1) Branch
   - Name: `<yourname>/week-09-project`

2) Commit
   - Message: `Week 09 Project: <short description>`

3) Push and Pull Request
   - Title: `[<YourName>][Week09] Project Submission`
   - Description: public URL(s) + bullet list of changes (authoring + front-end).

4) Submit the **PR URL** in the course thread.

**Acceptance criteria (Submission)**
- [ ] Branch named correctly  
- [ ] Commit message descriptive  
- [ ] PR title and description follow the format  
- [ ] PR URL posted

---

## 🧠 AEM Alignment Summary

| Area | WordPress / Front-End Activity | AEM Equivalent | Concept Demonstrated |
|------|-------------------------------|----------------|----------------------|
| Authoring | Pages/blocks + metadata | AEM Pages + Dialogs | Structured authoring |
| Front-End | Edit `style.scss` / `edit.js` / `save.js`; build | AEM Clientlibs / HTL | Presentation & behavior |
| Integration & QA | Combined checks + a11y | AEM Quality gates | Governance & standards |
| DevOps | Branch → PR → Review | Cloud Manager pipeline | Collaboration & control |

---

## OS-Specific Paths

- **Windows (Jeff):** `C:\Users\<yourname>\Local Sites\aem-lab\app\public\`  
- **macOS (Mattie & Melanie):** `~/Local Sites/aem-lab/app/public/`

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
What you integrated, what you improved, and how this mirrors AEM’s Sites + Assets + Clientlibs flow.

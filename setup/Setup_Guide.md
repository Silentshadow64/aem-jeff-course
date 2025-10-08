# Setup Guide — WordPress (LocalWP) + GitHub (Desktop, CLI, Web)

This guide includes **Windows** and **macOS** instructions. Please follow every step carefully.

---

## Part A — Install WordPress locally with LocalWP

### A1. Download and Install LocalWP
**Windows (10/11):**
1. Open your web browser and go to: https://localwp.com
2. Click **Download**. Choose **Windows**.
3. Run the downloaded installer. Accept the defaults.
4. When installation finishes, launch **Local** (the app name).

**macOS (Intel or Apple Silicon):**
1. Open your web browser and go to: https://localwp.com
2. Click **Download**. Choose **macOS** (Apple Silicon if you have M1/M2/M3).
3. Drag **Local** to **Applications** if prompted.
4. Open **Local** from **Applications**.

### A2. Create Your First Local WordPress Site
1. Open the **Local** app.
2. Click **Create a new site** (or the plus **+**).
3. Site name: `aem-lab`
4. Choose **Preferred** environment (default). Click **Continue**.
5. Create WordPress Admin:
   - **Username:** `admin`
   - **Password:** `Admin123!` (or choose your own and write it down)
   - **Email:** your email
6. Click **Add Site**. Wait until the site is created.
7. Click **Open site** to view it. Click **WP Admin** to access the dashboard.
8. Log in with your admin username and password.

### A3. Verify Gutenberg (Block Editor)
1. In WP Admin, go to **Posts → Add New**.
2. The editor you see is **Gutenberg** (the block editor).
3. Add a **Paragraph** block and type **Hello Gutenberg**.
4. Click **Publish → Publish**.
5. View the post to confirm it appears.

---

## Part B — Install GitHub Tools and Create Your Repo

You will learn **three ways** to work with GitHub: **Web**, **Desktop**, and **Command Line**. Choose one or mix them.

### B1. Create a GitHub Account
1. Open https://github.com in your browser.
2. Click **Sign up** and create your account.
3. Choose a **Private** profile if you prefer.

### B2. Install GitHub Desktop
**Windows:**
1. Download https://desktop.github.com
2. Run the installer and sign in to GitHub when prompted.

**macOS:**
1. Download https://desktop.github.com (macOS version).
2. Drag the app to **Applications** and open it.
3. Sign in to GitHub when prompted.

### B3. (Optional) Install Git and GitHub CLI
**Windows (PowerShell):**
1. Install Git: https://git-scm.com/download/win (use defaults).
2. Install GitHub CLI: https://cli.github.com (download and install).
3. Verify:
   ```powershell
   git --version
   gh --version
   ```

**macOS (Terminal):**
1. Install Homebrew if you do not have it:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
2. Install Git and GitHub CLI:
   ```bash
   brew install git gh
   ```
3. Verify:
   ```bash
   git --version
   gh --version
   ```

### B4. Create Your Course Repository (Private)
**Using GitHub Web (easiest):**
1. Go to https://github.com → click **+** → **New repository**.
2. **Repository name:** `aem-no-sdk-course`
3. **Visibility:** **Private**
4. Do **not** add any files yet (no README). Click **Create repository**.

**Clone with GitHub Desktop (Windows or macOS):**
1. In GitHub Desktop: **File → Clone repository**.
2. Select the `aem-no-sdk-course` repo and choose a local path (for example, `Documents/aem-no-sdk-course`).
3. Click **Clone**.

**Or Clone from Command Line:**

Windows (PowerShell):
```powershell
cd $env:USERPROFILE\Documents
git clone https://github.com/YOUR-USERNAME/aem-no-sdk-course.git
cd aem-no-sdk-course
```

macOS (Terminal):
```bash
cd ~/Documents
git clone https://github.com/YOUR-USERNAME/aem-no-sdk-course.git
cd aem-no-sdk-course
```

### B5. Add Course Starter Files from the ZIP
1. Download the ZIP we provided for you (see main chat).
2. Extract it.
3. Copy **all folders and files** into your cloned `aem-no-sdk-course` directory.
4. Stage and commit the files:

**GitHub Desktop:**
- You will see changed files. Enter summary: `Add course starter files`. Click **Commit to main**.
- Click **Push origin** to upload to GitHub.

**Command Line:**

Windows (PowerShell):
```powershell
git add .
git commit -m "Add course starter files"
git push -u origin main
```

macOS (Terminal):
```bash
git add .
git commit -m "Add course starter files"
git push -u origin main
```

---

## Part C — Node.js for Gutenberg Block Development

### C1. Install Node.js (LTS) and npm
**Windows:**
1. Go to https://nodejs.org
2. Download **LTS** for Windows.
3. Run the installer and accept defaults.
4. Verify in **PowerShell**:
   ```powershell
   node -v
   npm -v
   ```

**macOS:**
1. Go to https://nodejs.org
2. Download **LTS** for macOS (Intel or Apple Silicon).
3. Run the installer.
4. Verify in **Terminal**:
   ```bash
   node -v
   npm -v
   ```

### C2. Where Your WordPress Code Lives
- Your LocalWP sites usually live in a folder like:
  - **Windows:** `C:\Users\YOURNAME\Local Sites\aem-lab\app\public\wp-content\`
  - **macOS:** `/Users/YOURNAME/Local Sites/aem-lab/app/public/wp-content/`
- You will create:
  - `wp-content/plugins/aem-blocks/` — custom blocks plugin (version-controlled)
  - `wp-content/themes/aem-lab/` — custom theme (optional, version-controlled)

> Tip: Keep a **copy** of your `aem-blocks` plugin **inside this course repo** under `wp/` so it is version-controlled. When you update the plugin, copy it into LocalWP.

---

## Part D — Submitting Work Each Week (Step-by-Step)

You can submit via **GitHub Desktop** or **Command Line**. Always push your branch and open a **Pull Request**.

### D1. Create a new branch for the week
**GitHub Desktop:**
1. Click **Current branch → New Branch**.
2. Name it like: `jeff/week-01` or `mattie/week-05`.
3. Click **Create branch**.

**Command Line (Windows PowerShell or macOS Terminal):**
```bash
git checkout -b jeff/week-01
```

### D2. Do your work
- Edit files in the current week folder (for example, `week01/`).
- Add screenshots to `week01/screenshots/`.
- Save your changes.

### D3. Commit your work
**GitHub Desktop:**
- Enter a commit summary, for example: `Complete Week 01 quiz and exercise`.
- Click **Commit to jeff/week-01**.

**Command Line:**
```bash
git add .
git commit -m "Complete Week 01 quiz and exercise"
```

### D4. Push and Open a Pull Request
**GitHub Desktop:**
- Click **Push origin**.
- Click **Create Pull Request** from GitHub Desktop or go to GitHub Web and click **Compare & pull request**.

**Command Line:**
```bash
git push -u origin jeff/week-01
```
- Go to GitHub Web, open the repository, and click **Compare & pull request**.

### D5. Ask for TA Help (any time)
- On GitHub, click **Issues → New issue** → choose **Request TA Help**.
- Fill out the form and submit.

### D6. Submit for Grading
- On GitHub, click **Issues → New issue** → choose **Ready for Grading**.
- Fill in your name, week number, and link to the Pull Request.

The Professor will review the PR, leave comments, and record a **numeric (0–100)** and **letter grade (A–F)** in `grading/gradebook.xlsx`.

---

**You are ready to start Week 01 in this repository.**

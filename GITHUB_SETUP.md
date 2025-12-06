# GITHUB SETUP GUIDE
## Step-by-Step Instructions to Deploy KIRBY v ASDA Case Manager

---

## Quick Start (5 Minutes)

### Prerequisites
- GitHub account (free at github.com)
- Git installed on your computer (optional but recommended)
- The files from this case manager

---

## Option 1: GitHub Web Interface (Easiest)

### Step 1: Create Repository
1. Go to **github.com** and log in
2. Click **+** icon (top right) → **New repository**
3. Fill in details:
   - **Repository name:** `kirby-asda-tribunal-case`
   - **Description:** `Employment Tribunal Case Manager - KIRBY v ASDA STORES LIMITED - Interactive case brief with 7 claims, 24 evidence files, damages analysis`
   - **Visibility:** Choose **Public** (or **Private** if confidential)
   - **Initialize with:** Check "Add a README.md"
4. Click **Create repository**

### Step 2: Upload Files
1. In your new repository, click **Add file** → **Upload files**
2. Upload these files:
   - `index.html` (main case manager)
   - `README.md` (overview)
   - `EVIDENCE_GUIDE.md` (evidence documentation)
   - `LEGAL_BASIS.md` (if created)
   - `.gitignore` (file structure)

3. Click **Commit changes**

### Step 3: Enable GitHub Pages (Make it Live Online)
1. Go to repository **Settings**
2. Scroll to **Pages** section (left sidebar)
3. Under "Source", select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**
5. Wait 30 seconds, refresh
6. You'll see: "Your site is published at https://[username].github.io/kirby-asda-tribunal-case/"

**Your case manager is now live!** Anyone with the link can access it.

---

## Option 2: Command Line (Most Professional)

### Step 1: Create Repository on GitHub
Same as Option 1, Step 1 above

### Step 2: Clone to Your Computer
```bash
cd Documents
git clone https://github.com/[YOUR-USERNAME]/kirby-asda-tribunal-case.git
cd kirby-asda-tribunal-case
```

### Step 3: Add Your Files
Copy these files into the directory:
- `index.html`
- `README.md`
- `EVIDENCE_GUIDE.md`
- `.gitignore`

### Step 4: Commit and Push
```bash
# Check status
git status

# Stage all files
git add .

# Commit with message
git commit -m "Add KIRBY v ASDA case manager - tribunal ready brief"

# Push to GitHub
git push origin main
```

### Step 5: Enable GitHub Pages
Same as Option 1, Step 3 above

---

## Repository File Structure

After uploading, your GitHub repository will look like this:

```
kirby-asda-tribunal-case/
├── index.html                    # Main interactive case manager
├── README.md                     # Case overview and quick reference
├── EVIDENCE_GUIDE.md             # Detailed evidence file descriptions
├── LEGAL_BASIS.md                # Legal references (if created)
├── .gitignore                    # Git configuration
├── LICENSE                       # Optional: add MIT or CC BY-NC-SA
└── docs/                         # Optional: folder for additional docs
    ├── CASE_STRENGTHS.md
    ├── DAMAGES_CALCULATION.md
    └── TIMELINE_DETAILS.md
```

---

## After GitHub Setup

### Access Your Case Manager

**Online URL (After GitHub Pages enabled):**
```
https://[YOUR-USERNAME].github.io/kirby-asda-tribunal-case/
```

**Example:**
```
https://georgekirby.github.io/kirby-asda-tribunal-case/
```

### Share the Link
- Send to your barrister
- Share with legal team
- Use in tribunal preparation
- Include in case documentation

---

## Customization Options

### Add Repository Description
1. Go to repository **Settings**
2. Edit description field:
   ```
   Employment Tribunal Case Manager | KIRBY v ASDA STORES LIMITED | 
   Case Ref: 60402852/2025 | 7 Claims | 24 Evidence Files | £55k-£70k Damages
   ```
3. Add website URL (if GitHub Pages enabled)
4. Add topics: `employment-law`, `tribunal`, `case-management`

### Add License (Recommended)
1. Click **Add file** → **Create new file**
2. Name: `LICENSE`
3. Add content:
   ```
   All rights reserved - George Kirby & Legal Team
   This case manager is confidential and prepared for tribunal purposes only.
   Unauthorized distribution prohibited.
   ```
4. Commit

### Make Repository Private (If Confidential)
1. Go to **Settings**
2. Scroll to "Danger Zone"
3. Click **Change repository visibility**
4. Select **Private**
5. Only people you invite can access

---

## Updating Your Case Manager

### Via Web Interface
1. Click on file to edit (e.g., `index.html`)
2. Click pencil icon (✎ Edit)
3. Make changes
4. Click **Commit changes**

### Via Command Line
```bash
cd kirby-asda-tribunal-case
# Edit your files
# Then commit:
git add .
git commit -m "Update evidence guide - clarify File 03"
git push origin main
```

---

## Sharing & Collaboration

### Get Shareable Link
- **Public repository:** Anyone with link can view
- **Private repository:** Only invited people can view

### Invite Team Members
1. Go to repository **Settings**
2. Click **Collaborators** (left sidebar)
3. Click **Add people**
4. Enter email/username
5. Choose role: **View**, **Edit**, or **Admin**

### Track Changes
- All edits are automatically tracked in **Commits** section
- See who changed what and when
- Revert to previous versions if needed

---

## Best Practices

### Organization
✓ Keep `index.html` in root directory (for GitHub Pages)  
✓ Use `README.md` for overview and quick navigation  
✓ Organize supporting docs in comments or separate file  
✓ Use `.gitignore` to exclude unnecessary files  

### Naming Conventions
✓ Descriptive file names: `EVIDENCE_GUIDE.md` not `guide.md`  
✓ Use UPPERCASE for documentation: `README.md`, `LICENSE`  
✓ Use lowercase for code files: `index.html`  

### Version Control
✓ Commit after each significant change  
✓ Write clear commit messages: "Add Appleby discrimination analysis"  
✓ Don't commit sensitive client data  
✓ Review changes before pushing  

### Documentation
✓ Update README when adding new sections  
✓ Link between related files  
✓ Keep evidence guide current with new files  

---

## Troubleshooting

### GitHub Pages Not Showing
1. Check **Settings** → **Pages**
2. Verify branch is set to `main` and folder is `/`
3. Wait 1-2 minutes and refresh
4. Check for errors in repository activity

### Files Not Uploading
1. Check file size (GitHub limit: 100 MB per file)
2. Verify .gitignore not blocking files
3. Use web interface instead of command line if issues persist

### Private Repository Showing Error
1. Ensure you're logged in
2. Check collaborator access
3. Try clearing browser cache

### Cannot Edit File
1. Ensure you have **Edit** permissions (not just View)
2. Check if repository is private/public
3. Contact repository owner

---

## Command Line Reference

```bash
# Clone repository
git clone https://github.com/[USERNAME]/kirby-asda-tribunal-case.git

# Navigate to folder
cd kirby-asda-tribunal-case

# Check status
git status

# Add all files
git add .

# Add specific file
git add index.html

# Commit changes
git commit -m "Description of changes"

# Push to GitHub
git push origin main

# Pull latest version
git pull origin main

# View commit history
git log

# Revert to previous commit
git revert [COMMIT-HASH]
```

---

## Final Steps Checklist

- [ ] Repository created on GitHub
- [ ] Files uploaded (index.html, README.md, etc.)
- [ ] GitHub Pages enabled
- [ ] Repository is public/private as intended
- [ ] Test URL works in browser
- [ ] Shared link with team/barrister
- [ ] Added description and topics
- [ ] Considered adding license
- [ ] Tested all tabs in case manager
- [ ] Verified all evidence links work

---

## Support Resources

**GitHub Help:**
- https://docs.github.com/en/pages
- https://docs.github.com/en/repositories

**Tribunal Case Management:**
- Refer to README.md for case overview
- Use EVIDENCE_GUIDE.md for evidence details
- Check main case manager (index.html) for claims analysis

---

## Version Information

- **Setup Guide:** 6 December 2025
- **GitHub Case Manager Status:** PRODUCTION READY
- **Case Reference:** 60402852/2025
- **Case Strength:** 90-95% across 7 claims

---

**Your KIRBY v ASDA case manager is now GitHub-ready and tribunal-ready!**

Next step: Share the URL with your barrister and legal team.

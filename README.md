# Deepesh Bagora - Professional Profile Repository

Personal website and resume repository managed with HTML/CSS for reliable, version-controlled profile management.

## 📁 Structure

```
/Users/deepeshbagora/Drive/info/
├── resume.html              # Master resume (1-2 pages, print-optimized)
├── index.html               # Portfolio website (detailed showcase)
├── css/
│   ├── resume.css           # Print-optimized resume styles
│   └── website.css          # Website styles (optional)
├── pdfs/                    # Generated PDF resumes (gitignored)
├── CLAUDE_CODE_GUIDE.md     # Guide for using with Claude Code
└── README.md                # This file
```

## 🎯 Philosophy

**Master Format**: HTML/CSS
- ✅ Full formatting control
- ✅ Easy PDF generation (browser print)
- ✅ Claude can edit perfectly
- ✅ 1-2 page enforcement via CSS
- ✅ Version control friendly

**Two Versions**:
- `resume.html` → Concise (1-2 pages, job applications)
- `index.html` → Detailed (unlimited, portfolio showcase)

## 📄 Resume (resume.html)

**Purpose**: Job applications
**Length**: Strictly 1-2 pages
**Content**: 
- Professional summary
- Top achievements only
- 3-5 most relevant projects
- Concise bullets (2-3 per role)

**Generate PDF**:
```bash
# Open in browser
open resume.html

# Then: Cmd+P → Save as PDF
```

## 🌐 Website (index.html)

**Purpose**: Portfolio showcase  
**Published**: https://deepeshbagora.github.io/info
**Content**:
- Extended project descriptions
- All projects with demos/screenshots
- Detailed experience narratives
- More comprehensive than resume

## 🔄 Workflow

### With Claude Desktop (Desktop Commander)

```
"Add P-serve to my resume and website"
"Update my professional summary"
"Sync resume and website"
```

### With Claude Code

```bash
cd /Users/deepeshbagora/Drive/info
claude-code

# Then in chat:
"Add [project] to resume and website"
"Create tailored resume for [Company]"
"Commit these changes"
```

### Manual Updates

1. Edit `resume.html` or `index.html`
2. Preview in browser
3. Generate PDF if needed (Cmd+P)
4. Commit to git
5. Push to GitHub

## 🎨 Styling

**CSS Organization**:
- `resume.css` → Print-optimized (1-2 pages enforcement)
- `website.css` → Web-optimized (if separate)

**Print Features**:
```css
@page { size: letter; margin: 0.75in; }
@media print { /* Print-specific styles */ }
```

## 📦 Version Control

**Current Branch**: main
**Remote**: https://github.com/deepeshbagora/info

**Common Commands**:
```bash
# See changes
git status
git diff resume.html

# Commit
git add resume.html index.html
git commit -m "Add P-serve experience"

# Push (updates live website)
git push origin main
```

## 🎯 Content Strategy

### Resume vs Website

| Aspect | Resume | Website |
|--------|--------|---------|
| Length | 1-2 pages | Unlimited |
| Projects | Top 3-5 | All projects |
| Detail | Bullets | Narratives |
| Focus | Job apps | Portfolio |

### Synchronization

**Core Info** (must match):
- Work experience (companies, roles, dates)
- Skills
- Education
- Certifications

**Different Levels** (intentional):
- Resume: Concise bullets
- Website: Extended descriptions

## 🛠️ Tools & Integration

**Profile Manager Skill**: Handles updates automatically
- Updates both resume and website
- Ensures 1-2 page limit
- Maintains sync
- Git integration

**Claude Code**: Repository management
- Multi-file updates
- Git workflow
- Project analysis

**Claude Desktop**: Quick edits
- Single file changes
- PDF automation
- Script execution

## 📋 Common Tasks

### Add New Experience
```
"Add [Company] as current employer with [achievements]"
```

### Add New Project
```
"Add my [project] from ~/Projects/[repo] to resume and website"
```

### Tailor Resume
```
"Create tailored resume for [Company] [Role]"
```

### Generate PDF
```bash
open resume.html
# Cmd+P → Save as PDF → pdfs/Deepesh_Resume_[Company]_[Date].pdf
```

### Sync Content
```
"Sync resume and website - check for differences"
```

## 📊 Current Status

**Resume**: Up to date with all experience through February 2025
**Website**: Portfolio with detailed project showcase
**CSS**: Optimized for 1-2 page print
**Repository**: Clean, version controlled

## 🚀 Quick Start

### For New Updates

**Claude Desktop**:
```
Open Claude Desktop → "Add [content] to my resume and website"
```

**Claude Code**:
```bash
cd /Users/deepeshbagora/Drive/info
claude-code
# "Add [content] to resume and website"
```

**Manual**:
```bash
# Edit files
code resume.html

# Preview
open resume.html

# Commit
git add -A
git commit -m "Update [section]"
git push
```

## 📚 Documentation

- `CLAUDE_CODE_GUIDE.md` - Using with Claude Code
- `resume.html` - Resume source  
- `css/resume.css` - Print styles

## 🔗 Links

- **Website**: https://deepeshbagora.github.io/info
- **LinkedIn**: https://www.linkedin.com/in/deepesh-bagora
- **Email**: deepeshb88@gmail.com

---

**Last Updated**: December 2024  
**Maintained By**: Deepesh Bagora  
**Tools**: HTML, CSS, Git, Claude (Desktop & Code)

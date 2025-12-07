# Using Profile Manager Skill in Claude Code

## Overview

The **profile-manager** skill works seamlessly in both **Claude Desktop** (with Desktop Commander) and **Claude Code** (agentic coding from terminal).

## In Claude Code

### What Claude Code Can Do

When working in your `/Users/deepeshbagora/Drive/info` repository:

```bash
# From terminal
cd /Users/deepeshbagora/Drive/info
claude-code
```

**Example Commands in Claude Code:**

1. **Update Resume**: "Add P-serve Pvt. Ltd. as my current employer to resume.html"
2. **Update Website**: "Add the PowerfulID project to index.html portfolio"
3. **Sync Both**: "Sync resume.html and index.html"
4. **Tailor Resume**: "Create tailored resume for Google ML Engineer - save as resume_Google_20241207.html"

### How It Works

Claude Code has access to:
- ✅ File reading/writing (can edit HTML directly)
- ✅ Git operations (can commit changes)
- ✅ Project context (understands repo structure)
- ✅ Skill system (profile-manager patterns)

**Workflow Example:**

```
You: Add my new AI project to resume and website

Claude Code:
- Reads resume.html and index.html
- Adds project to resume (concise, 3 bullets)
- Adds project to website (detailed)
- Ensures resume stays 1-2 pages
- Shows diff for review
- Commits: "Add AI project to resume and portfolio"
```

## File Structure Claude Code Will Manage

```
/Users/deepeshbagora/Drive/info/
├── resume.html           # Master resume (1-2 pages)
├── index.html            # Portfolio website
├── css/
│   ├── resume.css        # Resume print styles
│   └── website.css       # Website styles
├── pdfs/                 # Generated PDFs (gitignored)
└── README.md
```

## Skill Commands in Claude Code

The skill responds to natural language:

**Resume Updates:**
- "Update professional summary to emphasize ML skills"
- "Add [technology] to technical skills"
- "Fix education date capitalization"

**Project Management:**
- "Add [project] from ~/Projects/[repo]"
- "Update PowerfulID description"  
- "Remove old [project]"

**Sync:**
- "Check if resume and website synced"
- "Sync experience section"
- "Ensure all skills in both files"

**Tailoring:**
- "Create tailored resume for [Company] [Role]"
- "Emphasize [skills] in resume"
- "Reorder projects to highlight [type] work"

## Git Integration

Claude Code handles git automatically:

**Commands:**
- "Commit with message 'Add P-serve'"
- "Show diff before committing"
- "Create branch for updates"
- "Push to GitHub"

## PDF Generation in Claude Code

Claude Code can't generate PDFs directly but guides you:

**You**: "Need PDF of this resume"

**Claude Code**: 
```
To generate PDF:
1. Open resume.html in browser
2. Cmd+P (or Ctrl+P)
3. Select "Save as PDF"
4. Save to: pdfs/Deepesh_Resume_[Company]_[Date].pdf

Command: open /Users/deepeshbagora/Drive/info/resume.html
```

## Example Session

```
You: Add P-serve as current employer

Claude Code: 
Adding P-serve to resume.html and index.html...

Changes:
+ Resume: P-serve at top (3 achievements, 3 responsibilities)
+ Website: P-serve with detailed description
✓ Resume still 1-2 pages

Commit message: "Add P-serve experience"
Ready to commit?

You: yes

Claude Code: ✓ Committed. Run `git push` to update live site.
```

## Claude Desktop vs Claude Code

| Feature | Claude Desktop | Claude Code |
|---------|---------------|-------------|
| File Editing | ✅ Full | ✅ Full |
| Git Operations | ✅ Commands | ✅ Integrated |
| PDF Generation | ✅ Can automate | ⚠️ Manual |
| Project Analysis | ✅ Scripts | ✅ Built-in |
| Multi-file | ✅ Sequential | ✅ Parallel |
| **Best for** | Ad-hoc updates | Repo management |

## When to Use What

**Use Claude Code for:**
- Multiple file updates
- Git workflow integration
- Website repo management
- Batch resume/website updates

**Use Claude Desktop for:**
- Quick single edits
- PDF automation
- Custom scripts
- File system tasks

## Quick Reference

### Start Claude Code
```bash
cd /Users/deepeshbagora/Drive/info
claude-code
```

### Common Commands
```
"Add [experience/project/skill] to resume and website"
"Sync resume and website"
"Create tailored resume for [Company]"
"Show diff"
"Commit changes"
```

### Skill Auto-Activates
Just mention resume/website naturally:
- "Update my resume..." → Skill activates
- "Add to website..." → Skill activates  
- "Sync resume and website..." → Skill activates

## Tips for Best Results

1. **Be Specific**
   - Good: "Add P-serve with 40% API optimization achievement"
   - Bad: "Update resume"

2. **Review Diffs**
   - Check changes before committing
   - Verify page count (1-2 pages)

3. **Use Separation**
   - resume.html → Concise (jobs)
   - index.html → Detailed (portfolio)

4. **Keep CSS Separate**
   - Easier styling updates
   - Can share common styles

5. **Commit Frequently**
   - Small focused commits
   - Clear messages
   - Easy to revert

## Troubleshooting

**"Cannot find skill"**  
→ In Claude Code, just describe naturally. Skill patterns activate automatically.

**"Resume exceeds 2 pages"**  
→ "Shorten project descriptions to fit 2 pages"

**"Out of sync"**  
→ "Compare resume.html and index.html, show differences"

## What Was Created

✅ `/Users/deepeshbagora/Drive/info/resume.html` - Your resume
✅ `/Users/deepeshbagora/Drive/info/css/resume.css` - Print-optimized styles

**Next Steps:**
1. Open resume.html in browser to preview
2. Generate PDF: Cmd+P → Save as PDF
3. Start using Claude Code for updates!

Ready! 🚀

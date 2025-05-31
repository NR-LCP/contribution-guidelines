# Numerical Relativity Learning Collaboration Program (NR-LCP)
## Contribution and Collaboration Guidelines

Welcome to the **Numerical Relativity Learning Collaboration Program**! This document will guide you through our collaborative workflow using GitHub's powerful features.

---

## Table of Contents

1. [Git and GitHub Basics](#git-and-github-basics)
2. [GitHub Features Overview](#github-features-overview)
3. [Our Collaboration Workflow](#our-collaboration-workflow)
4. [Feature Usage Examples](#feature-usage-examples)
5. [Best Practices](#best-practices)
6. [Getting Started Checklist](#getting-started-checklist)

---

## Git and GitHub Basics

### What is Git?
**Git** is a distributed version control system that tracks changes in files and coordinates work among multiple people. Think of it as a sophisticated "save" system that:
- Keeps a complete history of all changes
- Allows multiple people to work on the same project simultaneously
- Enables you to revert to previous versions if needed
- Tracks who made what changes and when

### What is GitHub?
**GitHub** is a web-based platform that hosts Git repositories and provides additional collaboration tools. It's like a social network for code and documentation, offering:
- Cloud storage for your Git repositories
- Web interface for managing projects
- Collaboration tools (issues, pull requests, discussions)
- Project management features
- Documentation hosting (wikis, README files)

---

## GitHub Features Overview

### 1. **Repositories**
- Central storage for all project files, code, and documentation
- Contains the complete history of changes
- Can be public (visible to everyone) or private (restricted access)

### 2. **Issues**
- Track tasks, bugs, feature requests, and general discussions
- Can be assigned to specific people
- Support labels, milestones, and project boards
- Perfect for managing weekly assignments and questions

### 3. **Pull Requests (PRs)**
- Propose changes to the repository
- Enable code review and discussion before merging changes
- Maintain quality control and collaborative decision-making
- Essential for submitting assignments and collaborative work

### 4. **Wiki**
- Built-in documentation system
- Perfect for maintaining course materials, references, and guides
- Supports markdown formatting and collaborative editing
- Searchable and version-controlled

### 5. **Discussions**
- Forum-like feature for general conversations
- Organized by categories (Q&A, General, Ideas, etc.)
- Great for open-ended questions and community building
- Less formal than issues

### 6. **Projects**
- Kanban-style project management boards
- Track progress across multiple repositories
- Organize tasks by status (To Do, In Progress, Done)
- Link to issues and pull requests

---

## Our Collaboration Workflow

### Weekly Cycle
1. **Assignment Release** (Monday)
   - Supervisor creates new issue with weekly task
   - Issue includes reading materials, problem sets, or coding tasks
   - Participants get notified automatically

2. **Work Period** (Monday-Friday)
   - Participants work on assignments individually
   - Use Discussions for questions and clarification
   - Create draft pull requests for work-in-progress sharing

3. **Submission** (Friday)
   - Submit completed work via pull request
   - Include detailed description of approach and findings
   - Link to relevant issues and discussions

4. **Review Period** (Weekend)
   - Peer review of submissions
   - Supervisor feedback and suggestions
   - Collaborative improvement of solutions

### Monthly Presentations
- Mature work presented in online sessions
- Presentation materials stored in dedicated repository folder
- Recording and slides shared via wiki

---

## Feature Usage Examples

### Example 1: Weekly Assignment Management with Issues

**Supervisor Creates Assignment:**
```markdown
Title: Week 3: Einstein Toolkit Initial Setup

## Assignment Description
This week, you'll set up the Einstein Toolkit on your local machine and run your first simulation.

## Tasks
- [ ] Download and compile Einstein Toolkit
- [ ] Run the "HelloWorld" thorn
- [ ] Document any compilation issues encountered
- [ ] Submit a brief report on your setup experience

## Resources
- [Einstein Toolkit Documentation](https://einsteintoolkit.org/)
- [Installation Guide](link-to-guide)

## Deliverables
- Setup report (markdown file)
- Screenshot of successful compilation
- List of any errors and solutions

**Due Date:** Friday, [Date]
**Estimated Time:** 4-6 hours

## Discussion
Use the comments below for questions about this assignment.
```

**Participant Response:**
```markdown
@sajad-aghapour I'm encountering a compilation error with the Cactus build system. 
The error message is: [error details]

My system: Ubuntu 22.04, GCC 11.2

Has anyone else seen this issue?
```

### Example 2: Submitting Work via Pull Request

**PR Title:** `Week 3 Assignment: Einstein Toolkit Setup - [Your Name]`

**PR Description:**
```markdown
## Assignment Completion Report

**Week:** 3
**Topic:** Einstein Toolkit Initial Setup
**Student:** [Your Name]

### Summary
Successfully installed Einstein Toolkit v2024.05 on Ubuntu 22.04 system. 
Encountered and resolved dependency issues with HDF5 library.

### Files Added
- `reports/week3/setup-report-[yourname].md` - Detailed setup experience
- `reports/week3/screenshots/` - Compilation success screenshots
- `scripts/setup-helpers/install-deps.sh` - Helper script for dependencies

### Key Findings
1. Default HDF5 version incompatible - needed v1.12.1
2. OpenMPI configuration required specific flags
3. Compilation time: ~45 minutes on 8-core system

### Questions for Review
- Is the HDF5 version issue common? Should we add it to troubleshooting guide?
- Performance benchmarks - should I include timing results?

**Closes:** #15 (Week 3 Assignment Issue)

### Checklist
- [x] All files properly organized in designated folders
- [x] Markdown formatting follows style guide
- [x] Screenshots included and properly sized
- [x] No sensitive information (paths, credentials) exposed
- [x] Assignment requirements fully addressed
```

### Example 3: Using Discussions for Community Learning

**Discussion Category:** Q&A
**Title:** "Best Practices for Mesh Refinement in Black Hole Simulations"

```markdown
I'm working on binary black hole simulations and struggling with optimal mesh refinement strategies. 

**My Current Approach:**
- 7 refinement levels
- AMR based on truncation error
- Buffer zones of 2 grid points

**Questions:**
1. How do you balance computational cost vs. accuracy?
2. Any rules of thumb for refinement level selection?
3. Experiences with different AMR criteria?

**What I've Tried:**
- Berger-Oliger AMR - works but expensive
- Fixed mesh refinement - faster but less adaptive

Would love to hear others' experiences and strategies!

**Tags:** #mesh-refinement #black-holes #performance
```

### Example 4: Wiki Organization Structure

```
Home
├── Course Information
│   ├── Syllabus
│   ├── Weekly Schedule
│   └── Assessment Criteria
├── Technical Resources
│   ├── Software Installation Guides
│   ├── Numerical Methods References
│   └── Computational Resources
├── Assignment Archives
│   ├── Week 1: GR Review
│   ├── Week 2: Finite Differences
│   └── Week 3: Einstein Toolkit
├── Best Practices
│   ├── Code Style Guidelines
│   ├── Report Writing Standards
│   └── Collaboration Etiquette
└── Troubleshooting
    ├── Common Installation Issues
    ├── Debugging Techniques
    └── Performance Optimization
```

### Example 5: Project Board Setup

**Project: "12-Week NR Learning Program"**

**Columns:**
1. **Backlog** - Future assignments and ideas
2. **This Week** - Current active assignments
3. **In Progress** - Work being done by participants
4. **Review** - Submitted work awaiting feedback
5. **Completed** - Finished and approved work

**Card Example:**
```
Week 5: Gravitational Wave Extraction
- Assigned to: All participants
- Due: Friday, [Date]
- Labels: assignment, gravitational-waves
- Linked Issues: #23, #24
- Linked PRs: #45, #46, #47
```

---

## Best Practices

### Repository Organization
```
nr-lcp-2024/
├── assignments/
│   ├── week01-gr-review/
│   ├── week02-finite-differences/
│   └── ...
├── reports/
│   ├── week01/
│   │   ├── student1-report.md
│   │   └── student2-report.md
│   └── ...
├── code/
│   ├── shared-utilities/
│   ├── visualization-tools/
│   └── student-projects/
├── presentations/
│   ├── week04-presentation/
│   └── final-presentations/
├── resources/
│   ├── references/
│   ├── software-guides/
│   └── datasets/
└── docs/
    ├── collaboration-guidelines.md
    ├── style-guide.md
    └── troubleshooting.md
```

### Issue Management
- **Use descriptive titles**: "Week 3: Einstein Toolkit Setup" not "Assignment 3"
- **Apply relevant labels**: `assignment`, `question`, `bug`, `enhancement`
- **Set due dates** for assignments using milestones
- **Reference related issues** using #issue-number
- **Close issues** when completed using "Closes #X" in PR descriptions

### Pull Request Etiquette
- **One PR per assignment** - don't mix different weeks' work
- **Descriptive titles and descriptions** - help reviewers understand your work
- **Small, focused changes** - easier to review and discuss
- **Respond to feedback** promptly and constructively
- **Test your changes** before submitting

### Discussion Guidelines
- **Use appropriate categories**: Q&A for questions, General for discussions
- **Search before posting** - avoid duplicate topics
- **Be specific** in your questions - include error messages, system info
- **Help others** - answer questions when you can
- **Stay on topic** - keep discussions relevant to numerical relativity

### Wiki Maintenance
- **Keep pages current** - update information as needed
- **Use consistent formatting** - follow established style
- **Link between pages** - create a connected knowledge base
- **Include examples** - make abstract concepts concrete

---

## Getting Started Checklist

### For New Participants
- [ ] Accept GitHub repository invitation
- [ ] Read collaboration guidelines (this document)
- [ ] Set up Git on your local machine
- [ ] Configure SSH keys for GitHub access
- [ ] Introduce yourself in Discussions (General category)
- [ ] Review current week's assignment in Issues
- [ ] Explore the Wiki for background materials
- [ ] Join the project board to track progress

### For First Assignment Submission
- [ ] Fork or clone the repository
- [ ] Create a new branch for your work
- [ ] Complete the assignment in appropriate folder
- [ ] Write clear commit messages
- [ ] Create pull request with detailed description
- [ ] Respond to review feedback
- [ ] Celebrate your first contribution! 🎉

### Weekly Routine
- [ ] Check Issues for new assignments
- [ ] Review others' pull requests when possible
- [ ] Participate in Discussions
- [ ] Update project board with your progress
- [ ] Submit work via pull request by deadline

---

## Additional Resources

### Learning Git and GitHub
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

### Numerical Relativity Resources
- Links to key papers, textbooks, and online courses
- Software documentation and tutorials
- Community forums and mailing lists

---

## Contact and Support

**Program Supervisor:** Dr. Sajad Aghapour
- GitHub: @SajadAghapour
- Institution: Max Planck Institute for Gravitational Physics

**Technical Support:** Amir H. Ebrahimnezhad
- GitHub: @ThisismeAmir
- Email: thisismeamir@outlook.com
- Telegram: t.me/thisismeamir

**For Technical Issues:**
- Create an issue with the `technical-support` label
- Use Discussions Q&A category for general questions
- Check troubleshooting wiki pages first

**For Program Questions:**
- Use Discussions General category
- Direct message supervisor for private matters
- Check weekly assignment issues for specific guidance

---

*This document is living and will be updated based on program needs and participant feedback. Suggestions for improvements are always welcome!*

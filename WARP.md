# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Repository Overview

This is an **Obsidian vault** - a personal knowledge management system focused on cognitive science, learning frameworks, and productivity. The vault uses a structured approach to organize notes, templates, and automation scripts for knowledge work.

## Key Architecture

### Folder Structure
- **0.DailyNotes/**: Daily notes and periodic reviews
- **2.Sphere/Digital Garden/**: Core knowledge articles on cognitive science, learning theory, and mindset
- **4.Pipeline/**: Task management and workflow coordination (Todolist.md)
- **5.Misc/copilot-custom-prompts/**: AI writing assistants and custom prompts
- **Atlas/**: Navigation and indexing system
  - **Index/**: Dataview queries for analytics and discovery
  - **MOCs.md**: Map of Contents linking to all index files
  - **kanban/**: Project management boards
- **Extras/**: Utilities, templates, and automation scripts

### Core Technologies
- **Obsidian**: Primary knowledge management platform
- **Dataview Plugin**: Used extensively for dynamic queries and analytics
- **Python**: Utility scripts for file processing (`merge_md.py`)
- **Markdown**: Primary content format with extensive cross-linking

### Key Frameworks Implemented
- **FCPM Learning Framework**: A diagnostic framework for learning bottlenecks (Factual, Conceptual, Procedural, Meta-cognitive deficits)
- **Digital Garden Methodology**: Progressive knowledge building with interconnected notes
- **Task Management**: Dataview-driven todo system with completion tracking

## Common Development Tasks

### Working with Notes
```bash
# Search for specific content patterns
grep -r "概念" "2.Sphere/" --include="*.md"

# Find all TODO items
grep -r "\- \[ \]" . --include="*.md"

# Find files with specific tags
grep -r "#Learning-Framework" . --include="*.md"
```

### Running Python Scripts
```bash
# Merge markdown files in DailyNotes
cd "Extras"
python merge_md.py
```

### Dataview Queries
The vault uses complex Dataview queries for analytics. Key patterns:
- Task completion tracking: `WHERE !completed`
- File age calculations: `date(today)-(file.mtime)`
- Folder-specific filtering: `FROM "2.Sphere"`
- Tag-based queries: `FROM #todo`

## Important Files and Templates

### Core Navigation
- **0.HomePage.md**: Main dashboard with vault statistics and quick navigation
- **Atlas/MOCs.md**: Master index of all content areas
- **4.Pipeline/Todolist.md**: Primary task management interface

### Template System
- **Extras/Template/Rules/**: Documentation templates for different content types
- **5.Misc/copilot-custom-prompts/**: AI assistant configurations
- The vault uses a sophisticated templating system with Copilot custom prompts for writing assistance

### Analytics System
The vault tracks extensive metrics:
- Total days using Obsidian
- File creation statistics
- Tag usage analytics
- Task completion rates
- Recent activity patterns

## Content Philosophy

The vault follows a "求实原则" (pragmatic principle): "少讲大道理，少戴大帽子" (less grand theories, more practical applications). Content focuses on:

1. **Actionable frameworks** rather than abstract concepts
2. **Diagnostic tools** for identifying specific learning problems
3. **Targeted strategies** for different types of knowledge work
4. **Evidence-based approaches** to productivity and learning

## Working with This Vault

### When Adding Content
- Use the FCPM framework to categorize learning-related content
- Include Dataview frontmatter for analytics tracking
- Cross-link extensively using [[wikilinks]]
- Tag appropriately for discoverability

### When Modifying Structure
- Update relevant index files in Atlas/
- Maintain the folder structure for Dataview queries
- Preserve the Chinese-English bilingual nature of content
- Keep the pragmatic, action-oriented tone

### Understanding Cross-References
The vault uses extensive internal linking. Key link patterns:
- `[[filename]]`: Basic wikilink
- `[[folder/filename|display]]`: Folder reference with custom display
- `#tags`: Categorical organization
- Dataview queries: Dynamic content aggregation

This vault represents a sophisticated personal knowledge management system with strong automation and analytical capabilities, designed for continuous learning and productivity optimization.
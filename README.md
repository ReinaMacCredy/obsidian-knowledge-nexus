# Knowledge Nexus - Obsidian PKM System

A comprehensive Personal Knowledge Management (PKM) system built in Obsidian, combining PARA and Zettelkasten methodologies for effective learning, project tracking, and knowledge development.

## 📌 Introduction

This Obsidian vault serves as an integrated system for **personal knowledge management**, **project tracking**, and **continuous learning**. Built upon a hybrid framework that merges action-oriented organization with idea-centric knowledge development, it provides a comprehensive environment for capturing, processing, and retrieving information.

The vault was originally based on a structured PKM template, extensively customized to enhance:
- **Knowledge synthesis** through interconnected notes and structured hierarchies
- **Project management** with status tracking and priority assignment
- **Information retrieval** via powerful searching and dynamic dashboards
- **Temporal organization** through daily, weekly, and monthly reflection cycles

Key benefits of this setup include:
- **Modularity**: Each component serves a specific purpose while remaining connected to the whole
- **Scalability**: The structure grows organically with your knowledge and projects
- **Flexibility**: Adapts to different types of content and knowledge domains
- **Efficiency**: Streamlined capture and retrieval processes reduce friction

## 🗂️ Folder Structure

The vault is organized into five core components, each serving distinct but interconnected purposes:

| Folder     | Purpose                                                                         |
|------------|---------------------------------------------------------------------------------|
| `HUB`      | Central navigation and dashboards for accessing all vault components            |
| `PARA`     | Action-oriented content organized by projects, areas, resources, and archives   |
| `ZETA`     | Idea-centric content using Zettelkasten methodology for knowledge development   |
| `DAILY`    | Temporal organization with daily, weekly, monthly, quarterly and yearly notes   |
| `SYSTEM`   | Technical components including templates, scripts, assets, and design elements  |

### Detailed Structure

#### HUB
- **Homepage.md**: Central dashboard with progress tracking and quick navigation
- **Map of Content.md**: Dynamic index of all notes with filtering capabilities
- **Mail Box.md**: Task management system with completion tracking

#### PARA (Projects, Areas, Resources, Archives)
- **PROJECTS**: Time-bound initiatives with defined objectives and deadlines
- **AREAS**: Ongoing responsibilities and domains requiring continuous attention
- **RESOURCES**: Reference materials including documentation, contacts, and concept maps
- **ARCHIVES**: Completed projects and inactive materials for historical reference

#### ZETA (Zettelkasten)
- **PERMANENT**: Refined, standalone ideas with well-established connections
- **LITERATURE**: Notes from books, articles, research papers, and other learning materials
- **FLEETING**: Quick thought captures for later processing
- **CLIPPINGS**: External content collected from various sources

#### DAILY
- **DAILY**: Day-to-day notes, tasks, and reflections
- **WEEKLY**: Weekly reviews, planning, and summaries
- **MONTHLY**: Monthly goal setting and achievement tracking
- **QUARTERLY**: Strategic planning and periodic reviews
- **YEARLY**: Annual goals, reflections, and long-term planning

#### SYSTEM
- **TEMPLATE**: Structured formats for consistent note creation
- **ASSETS**: Media files, documents, and other resources
- **DESIGN**: Visual elements and aesthetic components
- **SCRIPT**: Utility scripts and automated processes

## 🔌 Plugins Used

This vault leverages several carefully selected plugins to enhance functionality:

| Plugin                   | Purpose                                                              | Configuration Notes                                |
|--------------------------|----------------------------------------------------------------------|---------------------------------------------------|
| **Datacore/Dataview**    | Dynamic content queries and dashboard creation                       | Powers Map of Content and project tracking         |
| **Templater**            | Advanced templating with variables and dynamic content               | Used for all note templates with custom scripts    |
| **QuickAdd**             | Rapid note creation and command execution                            | Configured with macros for common workflows        |
| **Iconic**               | Enhanced icon support for visual organization                        | Used with status tracking and task management      |
| **Folder Notes**         | Create overview pages for folders                                    | Improves navigation through folder hierarchies     |
| **Calendar**             | Temporal navigation and planning                                     | Integrated with daily notes workflow               |
| **Tasks**                | In-note task management with due dates                               | Displays tasks across notes in central dashboards  |
| **Style Settings**       | Theme customization and visual adjustments                           | Optimized for reading comfort and visual hierarchy |
| **Kanban**               | Visual project management boards                                     | Used for workflow visualization in projects        |
| **Hover Editor**         | Inline note editing and preview                                      | Enhances cross-note reference and editing          |
| **Obsidian Git**         | Version control and backup                                          | Configured for automated commits and syncing       |
| **Meta Bind**            | Create interactive elements in notes                                 | Used for dynamic controls in dashboards            |

## ⚙️ Workflows & Usage Patterns

### Daily Workflow

1. **Morning Routine**
   - Open the Homepage via the quick access button
   - Click "Open Daily Note" to generate or access today's note
   - Review "Due Today" and "Overdue" tasks
   - Plan the day's priorities in the "Daily Notes" section

2. **Capture Process**
   - Quick ideas go to Fleeting Notes
   - Meeting notes use the appropriate meeting template
   - Project work is documented in respective project notes
   - Learning material is processed through Literature Notes

3. **Evening Review**
   - Check off completed tasks in the daily note
   - Process any fleeting notes that need refinement
   - Update project statuses as needed
   - Prepare preliminary tasks for tomorrow

### Project Management Flow

1. **Project Initiation**
   - Create project using project template
   - Define scope, objectives, and deadlines
   - Set priority level and initial status

2. **Project Execution**
   - Update status as project progresses (To Do → In Progress → Completed)
   - Link relevant resources and reference materials
   - Track tasks and deadlines via Homepage dashboard

3. **Project Completion**
   - Change status to "Completed"
   - Review project outcomes
   - Archive when no longer actively referenced

### Knowledge Development Cycle

1. **Capture** - Initial information gathering
   - Create Fleeting Notes for quick ideas
   - Create Literature Notes when consuming content

2. **Process** - Refining and connecting
   - Develop Permanent Notes from refined ideas
   - Establish connections between related concepts
   - Organize into concept maps when appropriate

3. **Retrieve** - Finding and using knowledge
   - Use Map of Content for navigation
   - Leverage connections for lateral exploration
   - Apply knowledge in projects and areas

### Linking Strategy

- **Direct Links**: Connect explicitly related notes
- **Unlinked References**: Track implicit connections
- **Tags**: Categorize by themes and domains
- **Connections Metadata**: Track relationships in frontmatter

## 📅 Templates & Note Types

This vault includes numerous templates for consistent note creation:

### Core Templates

| Template Type            | Purpose                                           | Key Components                                     |
|--------------------------|---------------------------------------------------|---------------------------------------------------|
| **Daily Note**           | Day-to-day tracking and task management           | Tasks, meetings, notes, and daily progress tracking |
| **Project Note**         | Structured project documentation                  | Status, priority, due date, and progress tracking   |
| **Area Note**            | Ongoing responsibility documentation              | Goals, resources, and related projects              |
| **Meeting Note**         | Structured meeting documentation                  | Attendees, agenda, decisions, and action items      |
| **Literature Note**      | Notes on consumed content                         | Source reference, key ideas, and personal insights  |
| **Permanent Note**       | Refined, standalone ideas                         | Connections, references, and developed concepts     |
| **Fleeting Note**        | Quick thought capture                             | Datestamp and basic idea structure                  |

### Template Syntax Examples

**Project Note Frontmatter**:
```yaml
---
type: project_note
Status: "1 To Do"
Priority_Level: "A"
Due_Date: 2023-12-31
connections:
  - [[Related Note 1]]
  - [[Related Note 2]]
---
```

**Daily Note Structure**:
```markdown
# Daily Note
```calendar-nav
```

# Tasks
- Due Today (tasks query)
- Overdue (tasks query)
- Completed (tasks query)

# Daily Notes
(Content here)

# Overview
- Meetings (dataview query)
- Projects (dataview query)
- Areas (dataview query)
```

## ⏳ Roadmap & Future Improvements

- [ ] Enhance mobile experience with optimized mobile templates
- [ ] Implement spaced repetition system for learning materials
- [ ] Create advanced dashboards for specific knowledge domains
- [ ] Develop automated weekly and monthly review processes
- [ ] Refine tagging system for more precise knowledge retrieval
- [ ] Integrate better visual thinking tools (diagrams, mindmaps)
- [ ] Implement additional data visualization for project analytics
- [ ] Create custom CSS snippets for enhanced reading experience
- [ ] Establish better integration between daily notes and projects
- [ ] Develop advanced search strategies using dataview

## 📄 Credits & License

This vault was built upon the PARA-Zettelkasten hybrid framework concept, with inspiration from:

- The PARA method by Tiago Forte
- The Zettelkasten method by Niklas Luhmann
- Various PKM systems from the Obsidian community

This vault is also adapted and customized based on the work of [@ProudBenzene](https://github.com/ProudBenzene) from the repository [Reverse1999Wiki-in-Obsidian](https://github.com/ProudBenzene/Reverse1999Wiki-in-Obsidian). Credit is due for the structural inspiration and visual dashboard concepts.

**License**: This vault structure and templates are shared under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license, allowing for non-commercial sharing and adaptation with attribution.

---

Built with ❤️ using Obsidian and a carefully curated set of plugins. Designed to grow and evolve with your knowledge journey.

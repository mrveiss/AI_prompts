# Universal Agent Collaboration Framework

A systematic approach to engineering problem-solving using specialist agents coordinated by Claude as an engineering manager.

## Overview

This framework transforms Claude from a single problem-solver into an **engineering manager** that coordinates specialist agents to ensure comprehensive, high-quality solutions to complex technical problems.

## Directory Structure

```
project-root/
├── agents/                          # Specialist agent definitions (11 agents)
│   ├── frontend-engineer.md         # Frontend development specialist
│   ├── database-engineer.md         # Database optimization specialist
│   ├── devops-engineer.md           # Infrastructure/deployment specialist
│   ├── performance-engineer.md      # Performance optimization specialist
│   ├── ai-ml-engineer.md           # AI/ML integration specialist
│   ├── multimodal-engineer.md      # Multi-modal processing specialist
│   ├── testing-engineer.md         # Test strategy/QA specialist
│   ├── security-auditor.md         # Security assessment specialist
│   ├── code-reviewer.md            # Code quality specialist
│   ├── project-manager.md          # Planning/coordination specialist
│   └── documentation-engineer.md   # Documentation specialist
├── CLAUDE.md                       # Project development notes + framework
├── README.md                       # Project documentation
└── task-progress/                  # Task tracking (separate from CLAUDE.md)
    ├── current-tasks.md            # Active task tracking
    ├── completed-tasks.md          # Completed task history
    └── agent-coordination-log.md   # Agent interaction logs
```

## Installation

### For New Projects

1. **Create directory structure:**
   ```bash
   mkdir -p agents task-progress
   ```

2. **Copy universal agent files:**
   ```bash
   # Copy all 11 agent .md files to agents/ directory
   cp path/to/universal-agents/*.md agents/
   ```

3. **Initialize CLAUDE.md:**
   - Copy the Universal CLAUDE.md Template
   - Customize agent roster for your specific technology stack
   - Add your project-specific status section

4. **Initialize task tracking:**
   ```bash
   touch task-progress/current-tasks.md
   touch task-progress/completed-tasks.md
   touch task-progress/agent-coordination-log.md
   ```

### For Existing Projects

1. **Add framework to existing project:**
   ```bash
   mkdir -p agents task-progress
   cp path/to/universal-agents/*.md agents/
   ```

2. **Update existing CLAUDE.md:**
   - Keep your existing project history at the top
   - Append the Universal Agent Collaboration Framework at the bottom

3. **Initialize task tracking files**

## Customization for Different Technologies

The framework is designed to be technology-agnostic. Customize agents for your specific stack:

### Web Applications
- **@frontend-engineer**: React, Vue.js, Angular, vanilla JavaScript
- **@database-engineer**: PostgreSQL, MySQL, MongoDB, Redis
- **@devops-engineer**: Docker, Kubernetes, AWS, Azure

### Mobile Applications
- **@frontend-engineer**: React Native, Flutter, Swift, Kotlin
- **@database-engineer**: SQLite, Firebase, Realm
- **@devops-engineer**: App Store deployment, Firebase, mobile CI/CD

### Desktop Applications
- **@frontend-engineer**: Electron, Qt, WPF, JavaFX
- **@database-engineer**: Local databases, sync mechanisms
- **@devops-engineer**: Application packaging, distribution

### AI/ML Projects
- **@ai-ml-engineer**: TensorFlow, PyTorch, scikit-learn
- **@multimodal-engineer**: Computer vision, NLP, audio processing
- **@performance-engineer**: GPU optimization, model efficiency

### Enterprise Systems
- **@database-engineer**: Oracle, SQL Server, enterprise data warehouses
- **@security-auditor**: Compliance, enterprise security standards
- **@devops-engineer**: Enterprise deployment, monitoring solutions

## Usage

### Basic Agent Coordination

When Claude encounters any technical issue, it will automatically:

1. **Analyze the problem domain**
2. **Select appropriate specialist agents**
3. **Delegate specific tasks** with clear scope and deliverables
4. **Coordinate findings** between agents
5. **Synthesize comprehensive solution** validated by all relevant agents

### Task Progress Tracking

**Critical**: Task progress is tracked separately from CLAUDE.md to keep development notes clean.

#### Current Tasks (`task-progress/current-tasks.md`)
- Active task tracking with agent assignments
- Progress checkboxes and status updates
- Dependencies and blockers documentation

#### Completed Tasks (`task-progress/completed-tasks.md`)
- Historical record of completed work
- Solution summaries and outcomes
- Lessons learned and agent performance

#### Agent Coordination Log (`task-progress/agent-coordination-log.md`)
- Detailed agent interaction logs
- Coordination timeline and decision points
- Performance analysis and improvement opportunities

## Mandatory Development Guidelines

**CRITICAL RULES** that Claude must follow:

**Investigation & Problem Solving:**
- Ignore any assumptions and reason from facts only
- Use agents and all available MCPs to work on project solutions
- Maintain codebase structure and organize code systematically
- Investigate problems across all related areas, not just reported issues
- Work on one problem at a time, leaving no stone unturned
- Check ALL logs for clues when something isn't working

**Solution Standards:**
- Timeout is NOT a solution to problems
- Temporary function disable is NOT a solution
- Look for existing solutions before creating new ones
- Avoid hardcodes at all costs
- Never restart processes without user consent

**Error Resolution:**
- Fix errors properly until they are gone forever
- Investigate ALL related logs and components
- Trace errors full path across system boundaries
- Update installation scripts when adding dependencies

## Quality Gates

### Before Implementation
1. **@project-manager**: Architecture and approach validation
2. **@security-auditor**: Security vulnerability assessment
3. **@performance-engineer**: Performance impact analysis
4. **@testing-engineer**: Test strategy definition
5. **@documentation-engineer**: Documentation requirements

### During Implementation
- Continuous agent coordination and status updates
- Cross-validation of changes across affected systems
- Regular progress tracking in task-progress/ files

### After Implementation
- **@testing-engineer**: Functionality validation
- **@performance-engineer**: Performance regression check
- **@documentation-engineer**: Documentation updates
- All agents sign off on successful completion

## Agent Coordination Examples

### Performance Issue
```
Problem: Application slow response times

Agents: @performance-engineer, @database-engineer, @frontend-engineer
Coordination: Systematic analysis across all performance layers
Solution: Multi-layered optimization with validation
```

### Security Vulnerability
```
Problem: Authentication security issue discovered

Agents: @security-auditor, @code-reviewer, @database-engineer, @testing-engineer
Coordination: Comprehensive security assessment and remediation
Solution: Security patches with testing and documentation
```

### New Feature Development
```
Feature: Add real-time notifications

Agents: @project-manager, @frontend-engineer, @database-engineer, @devops-engineer
Coordination: Full-stack feature development with testing and deployment
Solution: Complete feature with monitoring and documentation
```

## Benefits

✅ **Systematic Problem-Solving**: Comprehensive coverage of all system aspects  
✅ **Quality Assurance**: Multi-agent validation prevents regressions  
✅ **Knowledge Transfer**: Documented coordination builds team knowledge  
✅ **Technology Agnostic**: Works across different tech stacks and domains  
✅ **Professional Standards**: Mimics real engineering team coordination  
✅ **Scalable Framework**: Grows with project complexity  
✅ **Clean Documentation**: Separated task tracking keeps CLAUDE.md focused  

## Troubleshooting

### Framework Not Working
- Verify agents/ directory contains all 11 agent files
- Check CLAUDE.md includes the collaboration framework
- Ensure task-progress/ directory exists with template files

### Agent Coordination Issues
- Review agent specifications for role clarity
- Check task delegation follows proper format
- Verify dependencies are clearly documented

### Task Tracking Problems
- Confirm task-progress/ files are being updated
- Check separation between development notes and task tracking
- Verify agent coordination is being logged

## Template Files

You need these files to implement the framework:

1. **Universal CLAUDE.md Template** - Core framework with development guidelines
2. **11 Universal Agent Files** - Specialist agent definitions
3. **Task Progress Templates** - Tracking file templates
4. **This README.md** - Implementation and usage guide

## Support

For framework customization:
1. Modify agent specifications in agents/ directory
2. Update coordination examples for your technology stack
3. Adjust quality gates for your project requirements
4. Customize development guidelines for your team standards

---

**Remember**: This framework ensures systematic, collaborative problem-solving using specialist agents as senior engineers. The goal is comprehensive, high-quality solutions through professional coordination, not single-point-of-failure problem solving.
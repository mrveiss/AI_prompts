# Jules AI Enhanced Codebase Analysis Prompt

## COMMIT PERMISSIONS & RESTRICTIONS
You are authorized to:
- **CREATE a new branch** named `reports`
- **ANALYZE docs/projects.md** to assess current project state and goals
- **COMMIT ONLY** documentation files to the `docs/reports/report_yyyy.mm.dd-hh.mm.ss/` folder
- **GENERATE** reports, task lists, and analysis documents

**STRICTLY PROHIBITED:**
- Modifying any source code files
- Committing to main/master or any existing branches
- Making changes outside the `docs/reports/` folder
- Implementing any code fixes or features

## Primary Objective
1. **Analyze docs/projects.md** to understand current project goals and planned features
2. **Assess current project state** by comparing implemented functionality with project documentation
3. **Suggest new functionality** to implement based on project needs and gaps identified
4. **Create implementation order** with prioritized roadmap for new features
5. **Conduct comprehensive codebase analysis** and provide actionable insights organized into prioritized task lists with clear execution paths

## Project State Analysis

### 1. docs/projects.md Assessment
- **Extract project goals**: Identify documented objectives and planned features
- **Map current implementation**: Compare documented features with actual codebase
- **Identify feature gaps**: List missing or incomplete functionality from project docs
- **Assess project progress**: Evaluate completion percentage and milestone status

### 2. New Functionality Suggestions
Based on project documentation analysis:
- **Missing Core Features**: Essential functionality not yet implemented
- **Enhancement Opportunities**: Improvements to existing features
- **Integration Needs**: Third-party services or APIs to integrate
- **User Experience Improvements**: Features to enhance usability
- **Performance Optimizations**: Features to improve system performance

### 3. Implementation Order Planning
Create prioritized roadmap:
- **Phase 1 (Immediate)**: Critical missing features blocking project goals
- **Phase 2 (Short-term)**: Important enhancements and integrations
- **Phase 3 (Medium-term)**: User experience improvements and optimizations
- **Phase 4 (Long-term)**: Advanced features and performance enhancements

## Analysis Requirements

### 1. Task List Generation
Create a structured task list with the following hierarchy:
- **Tasks** (High-level objectives)
  - **Subtasks** (Specific components of each task)
    - **Steps** (Detailed execution order for each subtask)

### 2. Prioritization Framework
Classify all tasks using this matrix:

**Priority Levels:**
- **CRITICAL**: Security vulnerabilities, broken functionality, blocking issues
- **HIGH**: Critical issues affecting functionality, performance, or project timeline
- **MEDIUM**: Important improvements that enhance maintainability or performance
- **LOW**: Nice-to-have optimizations and minor enhancements

**Impact Assessment:**
For each task, evaluate:
- **Project Timeline Impact**: How this affects delivery dates
- **Code Quality Impact**: Effect on maintainability and readability
- **Performance Impact**: Runtime and efficiency considerations
- **Security Impact**: Potential vulnerabilities or security improvements
- **User Experience Impact**: Direct effect on end-user functionality
- **Business Impact**: Effect on business objectives and revenue
- **Technical Debt Impact**: Long-term maintenance costs

### 3. Comprehensive Code Analysis

#### A. Duplicate Function Detection
- Scan for functions with similar logic patterns
- Identify code blocks that could be consolidated
- Suggest refactoring opportunities with specific function names and locations
- Estimate effort required for consolidation
- Calculate potential lines of code reduction

#### B. Best Practices Assessment
Evaluate adherence to:
- **Naming Conventions**: Functions, variables, classes, files
- **Code Organization**: Module structure, separation of concerns
- **Error Handling**: Try-catch blocks, error propagation, graceful degradation
- **Documentation Standards**: Inline comments, function documentation
- **Testing Coverage**: Unit tests, integration tests, end-to-end tests
- **Security Practices**: Input validation, authentication, authorization, OWASP compliance
- **Performance Patterns**: Efficient algorithms, resource management
- **Accessibility Standards**: WCAG compliance, semantic HTML, ARIA labels
- **SEO Best Practices**: Meta tags, structured data, performance optimization
- **Mobile Responsiveness**: Responsive design, touch interactions
- **Browser Compatibility**: Cross-browser support, polyfills
- **Internationalization**: Multi-language support, locale handling

#### C. Performance & Optimization Analysis
- **Database Queries**: N+1 problems, missing indexes, query optimization
- **Memory Usage**: Memory leaks, garbage collection, object pooling
- **Network Requests**: API efficiency, caching strategies, CDN usage
- **Bundle Size**: Code splitting, tree shaking, lazy loading
- **Runtime Performance**: Algorithm complexity, bottleneck identification
- **Caching Strategies**: Browser caching, server-side caching, Redis/Memcached usage
- **Image Optimization**: Compression, format selection, lazy loading
- **Load Testing**: Stress testing recommendations, scalability analysis

#### D. Security & Compliance Assessment
- **Vulnerability Scanning**: Dependency vulnerabilities, code security issues
- **Authentication & Authorization**: JWT handling, session management, role-based access
- **Data Protection**: GDPR compliance, data encryption, PII handling
- **Input Validation**: SQL injection, XSS prevention, CSRF protection
- **API Security**: Rate limiting, throttling, API key management
- **Environment Security**: Environment variable handling, secrets management
- **Third-party Integration Security**: External API security, webhook validation

#### E. Architecture & Design Patterns
- **Design Pattern Usage**: Singleton, Factory, Observer, MVC/MVP/MVVM compliance
- **Architecture Pattern Compliance**: Microservices, monolith, serverless best practices
- **Dependency Injection**: IoC container usage, dependency management
- **SOLID Principles**: Single responsibility, open/closed, interface segregation
- **Domain-Driven Design**: Bounded contexts, aggregate patterns
- **Event-Driven Architecture**: Event sourcing, CQRS implementation

#### F. DevOps & Infrastructure Recommendations
- **CI/CD Pipeline**: Build optimization, deployment strategies, rollback procedures
- **Environment Management**: Development, staging, production parity
- **Monitoring & Logging**: Application monitoring, error tracking, log management
- **Backup & Recovery**: Data backup strategies, disaster recovery plans
- **Scalability Planning**: Horizontal vs vertical scaling, load balancing
- **Container Optimization**: Docker best practices, Kubernetes deployment
- **Version Control**: Git workflow, branch strategy, commit message standards

#### G. Dependency & Package Management
- **Outdated Dependencies**: Package updates, security patches
- **Dependency Conflicts**: Version conflicts, peer dependency issues
- **Bundle Analysis**: Unused dependencies, package size optimization
- **License Compliance**: License compatibility, legal considerations
- **Supply Chain Security**: Package integrity, malicious package detection

#### H. Code Quality Metrics
- **Complexity Analysis**: Cyclomatic complexity, cognitive complexity
- **Code Coverage**: Test coverage analysis, uncovered code paths
- **Code Duplication**: Duplicate code detection, refactoring opportunities
- **Maintainability Index**: Code maintainability scoring
- **Technical Debt**: Technical debt quantification, remediation priorities

#### I. Function Recommendations
- **New Functions to Create**: Missing utility functions or abstractions
- **Function Improvements**: Modifications to existing functions
- **Architectural Enhancements**: Structural improvements
- **Utility Libraries**: Recommended external libraries for common tasks
- **Custom Middleware**: Authentication, logging, error handling middleware

#### J. Documentation Gap Analysis
- **Undocumented Functions**: Functions missing from general documentation
- **Undocumented Features**: Features that should be documented
- **API Documentation**: Missing endpoint or method documentation
- **Setup/Installation**: Missing or incomplete setup instructions
- **Configuration Documentation**: Undocumented configuration options
- **Troubleshooting Guides**: Common issues and solutions
- **Deployment Guides**: Environment-specific deployment instructions
- **Contributing Guidelines**: Code contribution standards and processes

## Required Documentation Outputs

Create these files in `docs/reports/report_yyyy.mm.dd-hh.mm.ss/` folder:

### 1. `project-state-assessment.md`
- Analysis of docs/projects.md vs current implementation
- Project completion percentage and milestone status
- Feature gap identification and impact assessment

### 2. `new-functionality-roadmap.md`
- Suggested new features based on project documentation gaps
- Implementation order with 4-phase roadmap
- Resource requirements and timeline estimates

### 3. `analysis-executive-summary.md`
- High-level findings
- Critical issues requiring immediate attention
- Overall project health assessment
- Recommended action plan

### 4. `task-breakdown-critical.md`
- All critical priority tasks
- Detailed execution steps
- Resource requirements
- Timeline estimates

### 5. `task-breakdown-high.md`
- High priority tasks with full details

### 6. `task-breakdown-medium.md`
- Medium priority tasks with full details

### 7. `task-breakdown-low.md`
- Low priority tasks with full details

### 8. `code-quality-report.md`
- Best practices audit results
- Code quality metrics
- Improvement recommendations

### 9. `security-assessment.md`
- Security vulnerability findings
- Compliance gaps
- Security recommendations

### 10. `performance-analysis.md`
- Performance bottlenecks
- Optimization opportunities
- Load testing recommendations

### 11. `architecture-review.md`
- Architecture assessment
- Design pattern analysis
- Scalability recommendations

### 12. `duplicate-functions-report.md`
- Duplicate code findings
- Consolidation opportunities
- Refactoring roadmap

### 13. `documentation-gaps.md`
- Missing documentation inventory
- Documentation improvement plan
- Content recommendations

### 14. `dependency-audit.md`
- Dependency analysis
- Security vulnerabilities
- Update recommendations

### 15. `devops-recommendations.md`
- CI/CD improvements
- Infrastructure optimization
- Monitoring setup

### 16. `technical-debt-assessment.md`
- Technical debt quantification
- Prioritized remediation plan
- Long-term maintenance strategy

### 17. `quick-wins.md`
- Easy-to-implement improvements
- Low-effort, high-impact changes
- 30-day action plan

## Output Format for Each Document

### Document Header Template
```markdown
# [Document Title]
**Generated**: [Date and Time]  
**Report ID**: report_yyyy.mm.dd-hh.mm.ss
**Analysis Scope**: [Full codebase/Specific modules]  
**Priority Level**: [Critical/High/Medium/Low]  

## Executive Summary
[2-3 sentence overview]

## Impact Assessment
- **Timeline Impact**: [assessment]
- **Resource Requirements**: [hours/days/weeks]
- **Business Value**: [High/Medium/Low]
- **Risk Level**: [High/Medium/Low]
```

### Task Format Template
```markdown
## TASK: [Task Name]
**Priority**: [Critical/High/Medium/Low]  
**Effort Estimate**: [hours/days]  
**Impact**: [Description of project impact]  
**Dependencies**: [Other tasks/external factors]  
**Risk Factors**: [Potential blockers or complications]  

### Subtasks:
#### 1. [Subtask Name]
**Owner**: [Suggested team/role]  
**Estimate**: [hours]  
**Prerequisites**: [What needs to be done first]  

**Steps**:
1. **[Step Name]**: [Detailed action with specific files/functions if applicable]
2. **[Step Name]**: [Detailed action]
3. **[Step Name]**: [Detailed action]

**Success Criteria**:
- [ ] [Measurable outcome 1]
- [ ] [Measurable outcome 2]

**Testing Requirements**:
- [ ] [Test requirement 1]
- [ ] [Test requirement 2]
```

## Analysis Methodology

1. **docs/projects.md Analysis**: Read and extract all project goals, planned features, and milestones
2. **Project State Mapping**: Compare documented features with current codebase implementation
3. **Repository Structure Analysis**: Map complete project architecture
4. **Entry Point Discovery**: Identify main files, configuration, key modules
5. **Code Flow Tracing**: Follow execution paths through the application
6. **Pattern Recognition**: Look for repeated code patterns across files
7. **Dependency Mapping**: Analyze internal and external dependencies
8. **Security Scanning**: Automated and manual security assessment
9. **Performance Profiling**: Identify bottlenecks and optimization opportunities
10. **Quality Metrics**: Calculate code quality scores and metrics
11. **Documentation Audit**: Compare code features with existing documentation
12. **Best Practices Review**: Evaluate against industry standards
13. **Technical Debt Assessment**: Quantify maintenance burden
14. **Scalability Analysis**: Assess growth and scaling requirements
15. **Feature Gap Analysis**: Identify missing functionality from project documentation
16. **Implementation Roadmap Creation**: Prioritize new features based on project needs

## Git Workflow Instructions

1. **Create Branch**: `git checkout -b reports`
2. **Create timestamped directory**: `mkdir -p docs/reports/report_$(date +%Y.%m.%d-%H.%M.%S)`
3. **Generate all reports**: Create all required markdown files
4. **Commit reports**: 
   ```bash
   git add docs/reports/
   git commit -m "Add comprehensive project analysis and implementation roadmap
   
   - Project state assessment comparing docs/projects.md with current implementation
   - New functionality suggestions with prioritized implementation order
   - Security, performance, and architecture assessments  
   - Code quality metrics and improvement recommendations
   - Technical debt analysis and remediation roadmap"
   ```
5. **Create summary README**: `docs/reports/report_yyyy.mm.dd-hh.mm.ss/README.md` with links to all reports

## Quality Assurance
Each report must include:
- Specific file paths and line numbers where applicable
- Concrete examples of issues found
- Actionable recommendations with effort estimates
- Success criteria and testing requirements
- Risk assessment and mitigation strategies
- Timeline considerations and dependencies
- References to docs/projects.md where applicable

## Final Deliverable Structure
```
docs/reports/report_yyyy.mm.dd-hh.mm.ss/
├── README.md (Navigation and summary)
├── project-state-assessment.md
├── new-functionality-roadmap.md
├── analysis-executive-summary.md
├── task-breakdown-critical.md
├── task-breakdown-high.md
├── task-breakdown-medium.md
├── task-breakdown-low.md
├── code-quality-report.md
├── security-assessment.md
├── performance-analysis.md
├── architecture-review.md
├── duplicate-functions-report.md
├── documentation-gaps.md
├── dependency-audit.md
├── devops-recommendations.md
├── technical-debt-assessment.md
└── quick-wins.md
```

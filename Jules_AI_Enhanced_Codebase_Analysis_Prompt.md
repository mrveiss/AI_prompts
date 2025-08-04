# Jules AI Enhanced Codebase Analysis Prompt

## COMMIT PERMISSIONS & RESTRICTIONS
You are authorized to:
- **CREATE a new branch** named `analysis-report-[timestamp]` (e.g., `analysis-report-20240803`)
- **COMMIT ONLY** documentation files to the `docs/` folder
- **GENERATE** reports, task lists, and analysis documents

**STRICTLY PROHIBITED:**
- Modifying any source code files
- Committing to main/master or any existing branches
- Making changes outside the `docs/` folder
- Implementing any code fixes or features

## Primary Objective
Conduct a comprehensive analysis of the codebase and provide actionable insights organized into prioritized task lists with clear execution paths, documented in the `docs/` folder.

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

Create these files in `docs/` folder:

### 1. `analysis-executive-summary.md`
- High-level findings
- Critical issues requiring immediate attention
- Overall project health assessment
- Recommended action plan

### 2. `task-breakdown-critical.md`
- All critical priority tasks
- Detailed execution steps
- Resource requirements
- Timeline estimates

### 3. `task-breakdown-high.md`
- High priority tasks with full details

### 4. `task-breakdown-medium.md`
- Medium priority tasks with full details

### 5. `task-breakdown-low.md`
- Low priority tasks with full details

### 6. `code-quality-report.md`
- Best practices audit results
- Code quality metrics
- Improvement recommendations

### 7. `security-assessment.md`
- Security vulnerability findings
- Compliance gaps
- Security recommendations

### 8. `performance-analysis.md`
- Performance bottlenecks
- Optimization opportunities
- Load testing recommendations

### 9. `architecture-review.md`
- Architecture assessment
- Design pattern analysis
- Scalability recommendations

### 10. `duplicate-functions-report.md`
- Duplicate code findings
- Consolidation opportunities
- Refactoring roadmap

### 11. `documentation-gaps.md`
- Missing documentation inventory
- Documentation improvement plan
- Content recommendations

### 12. `dependency-audit.md`
- Dependency analysis
- Security vulnerabilities
- Update recommendations

### 13. `devops-recommendations.md`
- CI/CD improvements
- Infrastructure optimization
- Monitoring setup

### 14. `technical-debt-assessment.md`
- Technical debt quantification
- Prioritized remediation plan
- Long-term maintenance strategy

### 15. `quick-wins.md`
- Easy-to-implement improvements
- Low-effort, high-impact changes
- 30-day action plan

## Output Format for Each Document

### Document Header Template
```markdown
# [Document Title]
**Generated**: [Date and Time]  
**Branch**: analysis-report-[timestamp]  
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

1. **Repository Structure Analysis**: Map complete project architecture
2. **Entry Point Discovery**: Identify main files, configuration, key modules
3. **Code Flow Tracing**: Follow execution paths through the application
4. **Pattern Recognition**: Look for repeated code patterns across files
5. **Dependency Mapping**: Analyze internal and external dependencies
6. **Security Scanning**: Automated and manual security assessment
7. **Performance Profiling**: Identify bottlenecks and optimization opportunities
8. **Quality Metrics**: Calculate code quality scores and metrics
9. **Documentation Audit**: Compare code features with existing documentation
10. **Best Practices Review**: Evaluate against industry standards
11. **Technical Debt Assessment**: Quantify maintenance burden
12. **Scalability Analysis**: Assess growth and scaling requirements

## Git Workflow Instructions

1. **Create Branch**: `git checkout -b analysis-report-[timestamp]`
2. **Create docs directory**: `mkdir -p docs/analysis`
3. **Generate all reports**: Create all required markdown files
4. **Commit reports**: 
   ```bash
   git add docs/
   git commit -m "Add comprehensive codebase analysis reports
   
   - Executive summary and priority task breakdown
   - Security, performance, and architecture assessments  
   - Code quality metrics and improvement recommendations
   - Technical debt analysis and remediation roadmap"
   ```
5. **Create summary README**: `docs/README.md` with links to all reports

## Quality Assurance
Each report must include:
- Specific file paths and line numbers where applicable
- Concrete examples of issues found
- Actionable recommendations with effort estimates
- Success criteria and testing requirements
- Risk assessment and mitigation strategies
- Timeline considerations and dependencies

## Final Deliverable Structure
```
docs/
├── README.md (Navigation and summary)
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

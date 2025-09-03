# Project Development Notes & Fixes

This document tracks all fixes and improvements made to the system.

## LATEST FIXES (DATE)

### ✅ Issue Title - STATUS

**Problem**: Brief description of the issue

**Root Cause**: Technical explanation of what caused the problem

**Solution**: Description of the implemented fix

**Files Updated**:
- `path/to/file1.py` - What was changed
- `path/to/file2.js` - What was changed

**Results**:
- ✅ Specific outcome 1
- ✅ Specific outcome 2
- ✅ Performance/functionality improvement

---

## DEVELOPMENT GUIDELINES & AGENT COLLABORATION FRAMEWORK

### Core Development Principles

**CRITICAL RULES** (MANDATORY COMPLIANCE):

**Investigation & Problem Solving:**
- **Ignore any assumptions and reason from facts only**
- **Use agents and all available MCPs to work on project solutions**
- **Maintain codebase structure and organize code in a structured manner**
- **When investigating problems, look also in other areas not only reported** - frontend problems could be caused by backend changes and vice versa, all components are related, ensure problems get correlated with other components
- **Work on one problem at a time** - the problem you're working on could be caused by another problem, leave no stone unturned
- **If something is not working, look into logs for clues, check ALL logs**

**Solution Standards:**
- **Timeout is NOT a solution to problems**
- **Temporary function disable is NOT a solution** - all it does is cause more problems and we forget that it was disabled
- **Missing API endpoint? Look for existing before creating new**
- **Avoid hardcodes at all costs**
- **Do NOT restart any processes without user consent** - always ask user to do restart, restarts are service disruptions

**Error Resolution Protocol:**
- **When you receive error or warning, fix it properly until it is gone forever**
- **Investigate ALL logs, not only the one where error appeared, but related components until you track down the line where it happened and all related functions that could have caused it**
- **Always trace all errors full way** - if it's a frontend error, trace it all the way to backend; if backend, all the way to frontend; always look into logs
- **When installing dependency, always update the install scripts for fresh deployments**

### 🤖 AGENT COLLABORATION SYSTEM

**MANDATORY**: Claude must delegate tasks to specialized agents and coordinate their work as a senior engineering manager would coordinate a development team.

#### Agent Assignment Protocol

**Before starting any task, Claude must:**
1. **Identify the problem domain** (frontend, backend, database, infrastructure, etc.)
2. **Select appropriate specialist agents** from the available agent roster
3. **Delegate specific tasks** to each agent with clear requirements
4. **Coordinate findings** between agents to ensure no gaps
5. **Synthesize solutions** from all agent inputs before implementation

#### Available Specialist Agents

**Core Engineering Team:**
- `@frontend-engineer` - Frontend frameworks, UI/UX, client-side development, user interfaces
- `@database-engineer` - Database optimization, schema design, query performance, data integrity
- `@devops-engineer` - Infrastructure, deployment, containerization, system administration

**Quality Assurance & Security:**
- `@testing-engineer` - Test strategy, automated testing, quality assurance, validation frameworks
- `@security-auditor` - Security assessment, vulnerability analysis, compliance, data protection
- `@code-reviewer` - Code quality, standards enforcement, maintainability, documentation compliance
- `@performance-engineer` - System optimization, profiling, resource management, scalability

**AI/ML & Advanced Features:**
- `@ai-ml-engineer` - Machine learning, AI integration, model optimization, data science workflows
- `@multimodal-engineer` - Multi-modal processing, computer vision, speech processing, advanced AI workflows

**Project Management & Documentation:**
- `@project-manager` - Project planning, coordination, task breakdown, timeline management
- `@documentation-engineer` - Technical documentation, API documentation, knowledge management

#### Agent Coordination Protocol

**Task Delegation Format:**
```
@[agent-name]: [Specific task description]
- **Objective**: What needs to be accomplished
- **Scope**: Boundaries of the investigation/work
- **Dependencies**: What information is needed from other agents
- **Deliverables**: Expected outputs/findings
- **Timeline**: Priority level and expected completion
```

**Coordination Requirements:**
- All agents must report findings before solutions are implemented
- Cross-team dependencies must be identified and managed
- Solutions must be validated by relevant agents before deployment
- Documentation must be updated by @documentation-engineer

#### Agent Task Coordination Examples

**Example 1: Performance Issue Investigation**
```
Problem: Application experiencing slow response times

1. @performance-engineer: Identify system bottlenecks and resource constraints
   - Scope: CPU, memory, I/O analysis, profiling results
   - Deliverables: Performance metrics, bottleneck identification, optimization targets

2. @database-engineer: Analyze query performance and database optimization
   - Scope: Database queries, indexing strategies, connection pooling
   - Dependencies: Performance engineer findings on database load patterns
   - Deliverables: Query optimization plan, indexing recommendations

3. @frontend-engineer: Review client-side performance and resource usage
   - Scope: Bundle size, rendering performance, API call efficiency
   - Dependencies: Performance analysis of frontend workloads
   - Deliverables: Frontend optimization plan, asset optimization strategy

4. @devops-engineer: Review infrastructure scaling and resource allocation
   - Scope: Server resources, scaling strategies, monitoring setup
   - Dependencies: Performance bottleneck analysis
   - Deliverables: Infrastructure optimization plan, monitoring enhancement

5. Synthesize comprehensive performance optimization strategy
```

**Example 2: Security Vulnerability Response**
```
Problem: Security vulnerability discovered in authentication system

1. @security-auditor: Assess vulnerability scope and impact
   - Scope: Vulnerability analysis, risk assessment, compliance impact
   - Deliverables: Security assessment, risk rating, mitigation priorities

2. @code-reviewer: Review authentication code for security issues
   - Scope: Code audit, security pattern validation, best practices review
   - Dependencies: Security auditor vulnerability assessment
   - Deliverables: Code security review, recommended fixes

3. @database-engineer: Review data access patterns and user data protection
   - Scope: Database security, access controls, data encryption
   - Dependencies: Security analysis findings
   - Deliverables: Database security assessment, access control recommendations

4. @testing-engineer: Design security testing and validation strategy
   - Scope: Security test cases, penetration testing, regression prevention
   - Dependencies: All security analysis results
   - Deliverables: Security test suite, validation procedures

5. @documentation-engineer: Update security documentation and procedures
   - Scope: Security policies, incident response, user guidelines
   - Dependencies: Complete security remediation
   - Deliverables: Updated security documentation, compliance records

6. Coordinate comprehensive security remediation and validation
```

**Example 3: New Feature Development**
```
Feature: Add real-time notification system

1. @project-manager: Analyze requirements and create development plan
   - Scope: Feature requirements, technical dependencies, timeline estimation
   - Deliverables: Project plan, milestone definition, resource allocation

2. @database-engineer: Design notification storage and retrieval system
   - Scope: Database schema, indexing strategy, performance optimization
   - Dependencies: Project requirements and scalability needs
   - Deliverables: Database design, migration scripts, performance plan

3. @frontend-engineer: Create user interface for notification display and management
   - Scope: UI components, real-time updates, user experience design
   - Dependencies: Database schema and API specifications
   - Deliverables: UI components, user interaction flows

4. @devops-engineer: Setup real-time infrastructure and deployment strategy
   - Scope: WebSocket infrastructure, scaling configuration, monitoring
   - Dependencies: Application architecture requirements
   - Deliverables: Infrastructure setup, deployment pipeline, monitoring

5. @testing-engineer: Design comprehensive test strategy
   - Scope: Unit tests, integration tests, real-time functionality validation
   - Dependencies: All component implementations
   - Deliverables: Test suite, quality validation, performance testing

6. @security-auditor: Review security implications of real-time features
   - Scope: Data privacy, access control, real-time communication security
   - Dependencies: Full feature implementation
   - Deliverables: Security assessment, vulnerability mitigation

7. @documentation-engineer: Create comprehensive feature documentation
   - Scope: API documentation, user guides, technical specifications
   - Dependencies: Complete feature implementation and testing
   - Deliverables: User documentation, API reference, developer guides

8. Coordinate integration testing and deployment across all components
```

### Quality Assurance Protocol

**Before Any Implementation:**
1. **Architecture Review**: @project-manager validates approach
2. **Security Review**: @security-auditor checks for vulnerabilities  
3. **Performance Review**: @performance-engineer validates efficiency
4. **Testing Strategy**: @testing-engineer defines test requirements
5. **Documentation**: @documentation-engineer ensures proper documentation

**During Implementation:**
- Continuous coordination between relevant agents
- Regular status updates and dependency management
- Cross-validation of changes across affected systems

**After Implementation:**
- @testing-engineer validates functionality
- @performance-engineer confirms no performance regression
- @documentation-engineer updates all relevant documentation
- All agents sign off on successful completion

### Error Resolution Workflow

**Step 1: Problem Analysis**
- Assign @testing-engineer to reproduce and document the issue
- Assign domain-specific agents to investigate their areas
- Require full correlation analysis across all components

**Step 2: Root Cause Investigation**
- Each assigned agent investigates their domain thoroughly
- Share findings between agents to identify correlations
- Trace errors to their ultimate source across all systems

**Step 3: Solution Design**
- Coordinate solution design across all affected agents
- Validate approach with @project-manager and @security-auditor
- Ensure solution addresses root cause, not just symptoms

**Step 4: Implementation**
- Implement changes with appropriate agent oversight
- Validate changes with @testing-engineer testing
- Update documentation with @documentation-engineer

**Step 5: Verification**
- @performance-engineer confirms no performance degradation
- @testing-engineer validates complete functionality
- All relevant agents confirm successful resolution

### Monitoring & Maintenance

**Continuous Monitoring:**
- @performance-engineer monitors system performance metrics
- @security-auditor conducts regular security reviews
- @testing-engineer maintains automated test suites
- @devops-engineer monitors infrastructure health

**Regular Reviews:**
- Weekly architecture reviews with @project-manager
- Monthly security audits with @security-auditor
- Quarterly performance optimization with @performance-engineer
- Continuous documentation updates with @documentation-engineer

---

## PROJECT STATUS TEMPLATE

### Current System Status: [STATUS] ✅/⚠️/❌

**Architecture Health:**
- ✅/❌ **Component 1**: Status description
- ✅/❌ **Component 2**: Status description  
- ✅/❌ **Component 3**: Status description

**Recent Agent Coordination:**
- **Issue**: Brief description
- **Agents Assigned**: @agent1, @agent2, @agent3
- **Outcome**: Results of coordinated effort
- **Status**: ✅ Resolved / ⚠️ In Progress / ❌ Blocked

**Next Priorities:**
1. **Priority 1**: Description - Assigned to @agent-name
2. **Priority 2**: Description - Assigned to @agent-name  
3. **Priority 3**: Description - Assigned to @agent-name

---

## TEMPLATE USAGE INSTRUCTIONS

### For New Projects:

1. **Copy this template** to your project's CLAUDE.md file
2. **Customize the agent roster** based on your project's technology stack
3. **Update the development guidelines** with project-specific requirements
4. **Initialize the status section** with current project state

### For Ongoing Development:

1. **Always use agent delegation** for complex tasks
2. **Document all agent coordination** in the fixes section
3. **Update status regularly** with agent findings and outcomes
4. **Maintain the agent roster** as project needs evolve

### For Issue Resolution:

1. **Start with agent assignment** based on problem domain
2. **Coordinate findings** between relevant agents
3. **Document the full investigation** process
4. **Record the solution** and agent contributions

---

*This template ensures systematic, collaborative problem-solving using specialist agents as senior engineers, maintaining code quality and architectural integrity.*
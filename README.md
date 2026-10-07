# prompt-engineering-assignment-
Prompt engineering assignment
# 10 Engineering Prompts with Outputs

## 1. API Performance Analyzer

### Prompt

Analyze the following API performance data and identify bottlenecks. Suggest practical improvements for response time, database queries, caching, and scalability. Present the findings in a clear engineering report.

### Output

# API Performance Analysis

## Findings

- Average response time: 850 ms
- Database queries account for approximately 60% of request time.
- Several repeated queries can be cached.
- The API has limited connection pooling.

## Recommendations

1. Add Redis caching for frequently requested data.
2. Optimize slow database queries and add appropriate indexes.
3. Increase database connection-pool efficiency.
4. Introduce pagination for large responses.
5. Add performance monitoring and latency alerts.

## Expected Result

- Reduced database load
- Lower API latency
- Better scalability under high traffic


---

## 2. Automated Backup System

### Prompt

Design a reliable automated backup system for a web application. Include backup frequency, storage strategy, retention policy, encryption, monitoring, and disaster recovery.

### Output

# Backup System Design

## Backup Schedule

- Database: Every 6 hours
- Application files: Daily
- Full system backup: Weekly

## Storage

- Primary backup: Separate storage server
- Secondary backup: Cloud object storage

## Security

- Encrypt backups at rest and during transfer.
- Restrict backup access using role-based permissions.

## Retention

- Daily backups: 14 days
- Weekly backups: 8 weeks
- Monthly backups: 12 months

## Recovery

- Perform monthly restoration tests.
- Maintain documented recovery procedures.

## Expected Result

A secure and recoverable backup architecture with minimal data loss.


---

## 3. CI/CD Pipeline

### Prompt

Create a CI/CD pipeline design for a web application using GitHub. Include testing, code quality checks, security scanning, build, deployment, and rollback.

### Output

# CI/CD Pipeline

```text
Developer
   ↓
Git Push
   ↓
GitHub Actions
   ↓
Unit Tests
   ↓
Linting & Code Quality
   ↓
Security Scan
   ↓
Build Application
   ↓
Deploy to Staging
   ↓
Integration Tests
   ↓
Deploy to Production
   ↓
Health Check
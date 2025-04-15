# GuardDuty Baseline Module

## File Overview
Configures AWS GuardDuty threat detection service with managed protection lists and CloudTrail integration. Enables continuous monitoring for malicious activity and unauthorized behavior.

## Resources
### aws_guardduty_detector (security_baseline)
- **Purpose**: Activates GuardDuty with optimized security settings
- **Parameters**:
  - `enable`: true
  - `finding_publishing_frequency": "SIX_HOURS"
- **Relationships**: Integrates with CloudTrail, VPC Flow Logs, and DNS logs

## Use Cases
- Detect compromised EC2 instances
- Identify suspicious API activity patterns

```mermaid
graph LR
  A[GuardDuty Detector] --> B[Findings]
  B --> C[CloudWatch Events]
  C --> D[SNS Alerts]
  D --> E[Security Team]
```

## Dependencies
- CloudTrail configuration from `cloudtrail-baseline`
- IAM roles from `iam-baseline` module
- SNS topics for alert notifications
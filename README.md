# AWS-SOC-Cybersecurity-Analytics-Platform

AWS Native Security Services:
| Amazon GuardDuty
Data Type: Findings
Key Information Provided: Malicious activity, unauthorized behavior, compromised resources (instances, accounts, S3)
SOC Relevance: Threat Detection, Incident Alerting 

| AWS Security Hub
Data Type: Findings (Aggregated)
Key Information Provided: Centralized view of security alerts, compliance
status checks
SOC Relevance: Alert Management, Compliance Monitoring, Security Posture Overview

| AWS CloudTrail
Data Type: Logs
Key Information Provided: API call history, user activity, resource changes SOC Relevance: Forensics, Auditing,Compliance, Incident Investigation

| AWS Config 
Data Type: Configuration, Logs (Changes) 
Key Information Provided: Resource inventory, configuration history,
compliance checks
SOC Relevance: Compliance Monitoring, Security Posture Assessment, Change
Management

| VPC Flow Logs
Data Type: Logs 
Key Information Provided: IP traffic metadata (source/dest IP, port, protocol, packets, bytes,action) 
SOC RelevanceL Network Monitoring, Threat Detection, Network Forensics |

| AWS Network Firewall | Logs | Traffic flow details, firewall rule actions (allow/deny) | Network
Security Monitoring, Policy Enforcement Verification |
| AWS WAF | Logs | Web request details, matched rules, source IPs, blocked threats (SQLi,
XSS) | Web Application Security Monitoring, Threat Analysis |
| Amazon Inspector | Findings | Software vulnerabilities, unintended network exposure |
Vulnerability Management, Risk Assessment |
| Amazon Macie | Findings | Location and type of sensitive data in S3, access anomalies | Data
Security, Compliance, Data Loss Prevention |

AWS Streaming Services:
| Kinesis Data Firehose
Primary Use Case: Reliable streaming delivery to S3, OpenSearch, Redshift, Splunk;simple ETL
Key Features: Auto-scaling, Buffering, Format Conversion, Lambda Transformation, Serverless
Sources: CloudWatch Logs, WAF, Network Firewall, KDS, Direct PUT; Destinations: S3, OpenSearch, Redshift, Splunk

| Kinesis Data Streams
Primary USe Case: Real-time streaming ingestion for multiple consumers or complex
stream processing
Key Features: High throughput, Durability, Shard-based scaling, 24hr-365day retention
Sources: SDK, Kinesis Agent, IoT; Destinations: Firehose, Lambda, Kinesis Data Analytics,
Custom Apps

| AWS Lambda
Primary Use Case: Custom data transformation logic within Firehose or triggered by other events
Key Features: Serverless compute, Event-driven, Pay-per-use |
Sources: Used with Firehose/KDS/S3/etc. for transformation/enrichment/filtering

🛡️ SentraBlueAI - AI-Powered Cyber Defense PlatformAdd commentMore actions

Status: MVP Phase 1 | Version: 1.0  

Author: Igbinedion Victor 

License: MIT

🔍 Project Overview

SentraBlueAI is an AI-enhanced Blue Team platform built to detect, analyze, and respond to cyber threats in real time. It leverages machine learning, stream processing, and endpoint telemetry to reduce alert fatigue and accelerate threat response across enterprise environments.

🎯 Objectives

- Reduce Mean Time to Detect (MTTD) and Mean Time to Respond (MTTR)


- Automatically surface suspicious behavior using unsupervised AI


- Provide human-readable alerts, threat scores, and behavior breakdowns


- Support both Windows and Linux endpoints with zero friction


🔧 MVP Scope

- Endpoint telemetry agent (`SentraAgent`)


- Ingestion API and message queue (`SentraGateway`)


- AI Engine for anomaly detection (`SentraBrain`)


- UI Dashboard for live alerts and threat scores (`SentraView`)


- PostgreSQL, MinIO/S3, Kafka-based backend
🧱 System Architecture

```
[SentraAgent] ---> [SentraGateway] ---> [Kafka Stream] ---> [SentraBrain]


                                             |                     |


                                        [DB + MinIO]        [Threat Scoring]


                                                                    |


                                                            [SentraView UI]

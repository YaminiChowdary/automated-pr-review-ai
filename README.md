<h1 align="center">🚀 Automated PR Review with AI</h1> <p align="center"> An AI-driven system that automates pull request reviews by analyzing code changes, retrieving context, and generating clear, actionable feedback. <br/> Fully serverless · Context-aware · Fast · Scalable </p>

🌟 Overview

This project improves the traditional PR review workflow by integrating AI-powered analysis into the development cycle. It eliminates slow manual reviews, missing context, and inconsistent feedback by generating high-quality, context-aware code review comments automatically.

🧠 Key Features

Intelligent analysis of code diffs

Context retrieval using vector embeddings

High-quality review comments using Amazon Bedrock Claude

Direct comment posting to Bitbucket PRs

Secure, event-driven, serverless backend

Fast, reliable, scalable processing


🏗 Architecture Summary

Bitbucket PR Event: Triggers review pipeline

API Gateway: Receives incoming payload

Lambda (Diff Parser): Extracts changes and metadata

Qdrant Vector DB: Retrieves related code context

Amazon Bedrock Claude: Generates code review insights

Lambda (Comment Publisher): Sends feedback to Bitbucket

SQS + Step Functions: Handle async execution + retries

Secrets Manager: Stores access tokens securely

A clean, fully event-driven pipeline optimized for reliability and low latency.


⚙️ Tech Stack

Cloud: AWS Lambda, API Gateway, SQS, Step Functions, CloudWatch

AI: Amazon Bedrock Claude

Vector DB: Qdrant

Backend: Python

Integrations: Bitbucket Webhooks

Security: AWS Secrets Manager

🧩 Engineering Highlights

Enhanced LLM clarity through structured prompts

Vector search enables deeper semantic understanding

Queue-based async design avoids webhook timeouts

Split Lambdas ensure low cold-start latency

Secure token rotation using Secrets Manager

📊 Impact

Review time reduced from hours → seconds

Improved clarity and consistency of feedback

Minimizes reviewer fatigue and human error

Scales effortlessly with team size

Delivers context-aware insights, not shallow comments

🔮 Future Improvements

Fine-tuned LLM models for deeper code reasoning

Metrics dashboard for team-level analytics

End-to-end encrypted prompt processing

Self-healing review pipeline

Multi-repository and multi-language support

🙏 Acknowledgments

Thanks to all collaborators and mentors who contributed to this project, including
Carol Manross, Shyam Yanamaddi, and the judging panel.

📄 Project Presentation

The complete slide deck is available in this repository:

📁 Code Review.pdf

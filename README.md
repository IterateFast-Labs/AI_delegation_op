# AI Multi-Agent Decision Framework

## Overview

The AI Multi-Agent Decision Framework is an advanced governance proposal analysis system that leverages multiple AI agents working in orchestration to provide comprehensive, reliable, and statistically robust evaluations of complex proposals. This framework combines expert domain knowledge simulation, collaborative discussion, and rigorous statistical analysis to produce actionable decision recommendations.

## Core Concept

### What is Multi-Agent Decision Making?

Traditional single-agent AI systems suffer from:
- **Single point of failure** - One model's biases affect the entire decision
- **Limited perspective** - Missing diverse domain expertise
- **Lack of deliberation** - No collaborative reasoning process
- **Statistical unreliability** - Single evaluation lacks confidence measures

Our framework addresses these limitations through:
- **Multi-agent orchestration** - Specialized agents for different domains
- **Collaborative discussion** - Agents interact and influence each other
- **Statistical rigor** - Multiple independent evaluations with G-Eval methodology
- **Transparent decision process** - Clear audit trail and reasoning

## Key Benefits

### 🎯 **Enhanced Decision Quality**
- **Domain Expertise**: Specialized agents (Finance, Technology, Governance) bring focused knowledge
- **Cross-pollination**: Agents challenge and refine each other's perspectives
- **Comprehensive Analysis**: Multi-dimensional evaluation covers all critical aspects

### 📊 **Statistical Reliability** 
- **G-Eval Methodology**: 10 independent evaluations provide robust scoring
- **Confidence Intervals**: Mathematical confidence levels based on standard deviation
- **Reproducible Results**: Temperature=0 ensures consistent, deterministic outputs
- **Outlier Detection**: Statistical analysis identifies and handles anomalous scores

### 🔄 **Transparent Process**
- **Audit Trail**: Every agent interaction and decision is logged
- **Performance Metrics**: Real-time tracking of duration, token usage, and efficiency
- **Explainable AI**: Clear rationales and reasoning chains for all decisions
- **Human Oversight**: Framework supplements rather than replaces human judgment

### ⚡ **Scalable Architecture**
- **Modular Design**: Easy to add new agents or modify existing ones
- **Parallel Processing**: Independent evaluations can run concurrently
- **Framework Agnostic**: Works with any LLM provider or model
- **Performance Optimization**: Built-in metrics for continuous improvement

## Detailed Framework Flow

### Phase 1: Initial Analysis & Classification

```
┌─────────────────┐    ┌──────────────────────┐
│   Proposal      │───▶│ Classification Agent │
│   Input         │    │                      │
└─────────────────┘    └──────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────┐
│ Optimism Governance Framework Classification    │
│ • Maintenance Upgrade                           │
│ • Protocol/Governor Upgrades                    │ 
│ • Token Allocations                             │
│ • Treasury Appropriations                       │
│ • Inflation Changes                             │
│ • Ratification                                  │
│ [... and 9 more categories]                     │
└─────────────────────────────────────────────────┘
```

**Process:**
1. **Proposal Input**: User submits proposal information and URL
2. **Content Extraction**: Jina Reader API fetches comprehensive proposal content
3. **Classification**: AI agent categorizes proposal using Optimism's governance framework
4. **Information Extraction**: Structured analysis of core elements, quantitative data, and community sentiment

### Phase 2: Expert Multi-Agent Discussion

```
┌─────────────────┐    ┌──────────────────────┐    ┌─────────────────────┐
│ Dr. Anya Sharma │    │   Ben Carter         │    │   Chloe Davis       │
│ (Finance)       │    │   (Technology)       │    │   (Governance)      │
│                 │    │                      │    │                     │
│ • Tokenomics    │    │ • Smart Contracts    │    │ • Process Compliance│
│ • Treasury      │    │ • Security           │    │ • Stakeholder Impact│
│ • ROI Analysis  │    │ • Scalability        │    │ • Regulatory Risk   │
└─────────────────┘    └──────────────────────┘    └─────────────────────┘
         │                        │                           │
         └────────────────────────┼───────────────────────────┘
                                  ▼
                    ┌─────────────────────────┐
                    │  Collaborative          │
                    │  Discussion             │
                    │  (2 Turns Each)         │
                    └─────────────────────────┘
```

**Discussion Process:**
1. **Turn-Based Discussion**: Each expert provides analysis in structured turns
2. **Context Accumulation**: Agents build upon previous discussions
3. **Perspective Evolution**: Dynamic prompt updates based on agent interactions
4. **Consensus Building**: Agents acknowledge when concerns are addressed
5. **Professional Discourse**: Experts maintain domain-specific standards

**Expert Responsibilities:**

| Expert | Domain | Key Focus Areas |
|--------|--------|-----------------|
| **Dr. Anya Sharma (Finance)** | DeFi Finance & Tokenomics | Financial sustainability, token economics, treasury implications, ROI analysis, funding risks |
| **Ben Carter (Technology)** | Blockchain CTO | Technical feasibility, security considerations, scalability impacts, implementation complexity |
| **Chloe Davis (Governance)** | Web3 Governance | Process adherence, voting mechanisms, stakeholder representation, regulatory compliance |

### Phase 3: G-Eval Feasibility Scoring

The framework implements **G-Eval** (Generative Evaluation) methodology for robust statistical analysis:

```
                    Expert Discussion Transcript
                              │
                              ▼
                    ┌─────────────────────┐
                    │  G-Eval Process     │
                    │  (10 Independent    │
                    │   Evaluations)      │
                    └─────────────────────┘
                              │
            ┌─────────────────┼─────────────────┐
            ▼                 ▼                 ▼
    ┌─────────────┐  ┌─────────────┐   ┌─────────────┐
    │ Evaluation  │  │ Evaluation  │...│ Evaluation  │
    │     #1      │  │     #5      │   │    #10      │
    │ Score: 75   │  │ Score: 82   │   │ Score: 73   │
    └─────────────┘  └─────────────┘   └─────────────┘
            │                 │                 │
            └─────────────────┼─────────────────┘
                              ▼
                    ┌─────────────────────┐
                    │ Statistical         │
                    │ Aggregation         │
                    │ • Mean: 76.2        │
                    │ • Median: 75.0      │
                    │ • StdDev: 4.3       │
                    │ • Confidence: High  │
                    └─────────────────────┘
```

#### G-Eval Methodology

**G-Eval** (Generative Evaluation using Large Language Models) is a framework-agnostic evaluation method that uses LLMs as evaluators. Our implementation:

1. **Multiple Independent Calls**: 10 separate API calls to the same LLM
2. **Consistent Prompting**: Each call uses identical context with slight variation
3. **Temperature=0**: Deterministic outputs reduce random variance
4. **Statistical Aggregation**: Mathematical computation of central tendency and dispersion

**Scoring Criteria (Applied in Each Evaluation):**
- **Evidence Quality (25%)**: How well-supported are arguments with data and precedent?
- **Expert Consistency (20%)**: Do experts maintain logical consistency?
- **Risk Assessment (20%)**: How thoroughly are risks identified and evaluated?
- **Implementation Viability (20%)**: How realistic are proposed solutions?
- **Stakeholder Impact (15%)**: How well does analysis consider affected parties?

**Statistical Analysis:**
```python
# Pseudocode for statistical processing
scores = [eval_1, eval_2, ..., eval_10]
mean = sum(scores) / len(scores)
median = sorted(scores)[len(scores)//2]
std_dev = sqrt(sum((x - mean)² for x in scores) / len(scores))

confidence_level = {
    "High": std_dev <= 5,
    "Medium": 5 < std_dev <= 15, 
    "Low": std_dev > 15
}
```

### Phase 4: Final Decision Recommendation

Based on the G-Eval median score, the framework provides clear recommendations:

| Score Range | Recommendation | Color Code | Rationale |
|-------------|----------------|------------|-----------|
| **81-100** | ✅ **Proceed** | Green | Strong feasibility with minimal risk |
| **50-80** | ⚠️ **Proceed with Caution** | Yellow | Moderate feasibility, risk mitigation needed |
| **30-49** | 🟠 **Not Recommended** | Orange | Low feasibility, significant concerns |
| **0-29** | ❌ **Do Not Proceed** | Red | Poor feasibility, fundamental flaws |

### Phase 5: Performance Metrics & Tracking

```
┌─────────────────────────────────────────────────┐
│              Performance Tracker                │
├─────────────────────────────────────────────────┤
│ Duration Metrics:                               │
│ • Total Execution Time: 45.3s                   │
│ • Per-Agent Breakdown:                          │
│   - Classification: 2.1s                        │
│   - Summary: 3.4s                               │
│   - Expert Discussion: 18.7s                    │
│   - G-Eval Scoring: 21.1s                       │
│                                                 │
│ Token Usage:                                    │
│ • Total Input Tokens: 12,847                    │
│ • Total Output Tokens: 3,924                    │
│ • Estimated Cost: $0.23                         │
│                                                 │
│ Efficiency Analysis:                            │
│ • Tokens per Minute: 22,159                     │
│ • Processing Rate: 366 tokens/second            │
│ • Bottlenecks: G-Eval scoring (46% of time)     │
└─────────────────────────────────────────────────┘
```

## Technical Architecture

### Agent Configuration System

```json
{
  "agent_id": {
    "name": "Agent Name",
    "model": "gemini-2.5-flash",
    "systemInstruction": "Role-specific instructions",
    "prompt": "Task-specific prompt with {placeholders}",
    "responseMimeType": "application/json",
    "responseSchema": { /* JSON schema */ },
    "maxOutputTokens": 400,
    "thinkingConfig": { "thinkingBudget": 200 }
  }
}
```

### Multi-Agent Orchestration Flow

1. **Sequential Processing**: Agents process in logical dependency order
2. **State Management**: React state tracks each agent's progress and outputs
3. **Error Handling**: Comprehensive error recovery and fallback mechanisms
4. **Progress Tracking**: Real-time updates on processing status
5. **Metrics Collection**: Performance data captured throughout execution

### Quality Assurance Features

- **Input Validation**: Proposal format and content verification
- **Output Validation**: JSON schema enforcement and parsing verification
- **Rate Limiting**: Controlled API call pacing to avoid throttling
- **Timeout Management**: Configurable timeouts for long-running operations
- **Logging**: Comprehensive debug and audit logging

## Performance Metrics Explained

# Multi-Agent Orchestration Flow

A stage-based pipeline that turns a governance proposal into a transparent, statistically robust recommendation using coordinated AI agents and G-Eval scoring


## Table of Contents

* [Overview](#overview)
* [Architecture at a Glance](#architecture-at-a-glance)
* [Execution Model](#execution-model)
* [State Management](#state-management)
* [Progress & Metrics](#progress--metrics)
* [Quality Assurance](#quality-assurance)
* [Rate Limiting, Timeouts & Caching](#rate-limiting-timeouts--caching)
* [G-Eval Scoring Metrics](#g-eval-scoring-metrics)
* [Use Cases](#use-cases)
* [Roadmap](#roadmap)


## Overview

This module coordinates multiple specialist agents to analyze a proposal, debate trade-offs, and produce a recommendation backed by reproducible statistics. It emphasizes determinism, structured outputs, and lightweight runtime instrumentation for credibility and scale


## Architecture at a Glance

```
Input → Classification → Expert Discussion → G-Eval (N runs) → Aggregation → Recommendation
                           │                     │
                           └── Retrieval (rules, precedents, evidence) ──┘
```

* **Stage-based pipeline** with parallel execution for independent steps
* **Deterministic runs** via temperature 0, fixed prompts, versioned artifacts
* **Idempotent tasks** identified by `run_id`, `agent_id`, `prompt_hash`, `seed`


## Execution Model

* **Stages**

  * **Classification**: map proposal to governance category and extract key variables
  * **Expert Discussion**: finance, technology, governance agents exchange structured turns
  * **G-Eval**: multiple independent evaluations on the same context
  * **Aggregation**: compute central tendency, dispersion, and confidence interval
  * **Recommendation**: map final score to action with risk-mitigation checklist
* **Independence & Parallelism**: independent calls can execute concurrently
* **Reproducibility**: consistent prompts and seeds enable byte-for-byte replays


## State Management

* **Server-side persistence** for each stage (status, latency, tokens in/out, cost, model, context fingerprint)
* **Input/Output snapshots** per stage to enable replays and side-by-side comparisons
* **Minimal UI state**: the UI consumes events; orchestration state remains on the server


## Progress & Metrics

* **Real-time events** surfaced to the UI (scheduled, started, succeeded, failed, retried)
* **Weighted progress** reflects parallel work and relative effort per stage
* **Core metrics**

  * **Timings**: per-stage and end-to-end wall-clock time
  * **Throughput**: tasks/second and tokens/second
  * **Token & cost accounting**: input/output tokens, estimated spend
  * **Cache effectiveness**: hit rate and avoided cost


## Quality Assurance

* **Input validation**

  * Proposal URL reachability and successful content extraction
  * Required fields populated after normalization to internal schema
* **Output validation**

  * Strict JSON schema for all agent responses
  * Score bounds and weight checks
  * Auto-correction prompts for incomplete structures, then re-validate


## Rate Limiting, Timeouts & Caching

* **Provider-level concurrency caps** with adaptive throttling
* **Per-stage soft/hard timeouts** with graceful fallbacks
* **Caching & de-duplication**

  * Response cache keyed by `prompt_hash + context_fingerprint`
  * Duplicate calls within a run are suppressed


## G-Eval Scoring Metrics

* **Central tendency**: report **median** (robust to outliers) alongside **mean** (skew awareness)
* **Dispersion**: **standard deviation** plus **IQR** for robust spread
* **Confidence intervals**: bootstrap CI at the aggregate score level
* **Outliers**: identify via nonparametric fences or standardized scores and note impact
* **Convergence**: track stability of the median as evaluations accumulate

**Evaluation quality signals**

* Parsing success rate for structured outputs
* Criteria coverage: Evidence Quality, Expert Consistency, Risk Assessment, Implementation Viability, Stakeholder Impact
* Evidence fidelity: count and relevance of retrieved citations
* Cross-evaluation consistency: detect contradictions and request clarification when needed


## Use Cases

* **Governance proposals**: automatic classification, precedent retrieval, expert debate, G-Eval aggregation, recommendation with mitigations
* **Enterprise decision support**: large-scale parallel scoring with model routing and transparent metrics for stakeholders


## Roadmap

* Dynamic agent selection based on proposal embeddings and historical performance
* Real-time human-in-the-loop comments that feed the next expert turns
* Multimodal analysis (diagrams, screenshots, code diffs) where relevant
* Model diversity and provider mixing for robustness under varying workloads

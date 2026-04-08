# Bot-Detection

## Overview
A hybrid bot detection system for social media platforms, currently being trained on live data from the Reddit and Bluesky APIs. The tool combines rule-based behavioral signals, NLP, and LLM-based analysis to identify inauthentic accounts and coordinated bot activity.

## Motivation
Bot farms and coordinated inauthentic behavior represent a growing threat to online platforms. Existing detection methods often rely on single-signal approaches that are easily evaded. This project explores a multi-layered detection pipeline that combines structured behavioral features with language-level signals to improve robustness.

## Approach
Behavioral analysis: Predefined criteria capturing posting frequency, timing patterns, account age, engagement ratios, and other activity-based signals
NLP: Text-level features extracted from post content to identify templated, repetitive, or inauthentic language patterns
LLM integration: Large language model components for deeper semantic analysis of content and context
Model experimentation: Currently evaluating clustering and regression models; additional classifiers will be benchmarked to identify optimal accuracy

## Data Sources
Reddit API (live data collection)
Bluesky API (live data collection)

## Current Status
Data collection pipeline operational
Feature engineering in progress
Model training and evaluation ongoing

## Preliminary Results
Current implementation achieves ~80% detection accuracy on test data. The remaining 20% gap is attributable to sophisticated bot farm techniques designed to mimic organic human behavior — a known open problem in adversarial machine learning.

## Tech Stack
Python
NLP / LLM frameworks
Reddit API, Bluesky API

## Roadmap
Complete model benchmarking across classification approaches
Improve robustness against adversarial bot farm evasion techniques
Explore graph-based methods for detecting coordinated account networks

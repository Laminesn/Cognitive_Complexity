# Cognitive Complexity Analysis

## Project Overview
This repository contains a comprehensive analysis of cognitive complexity in a modern web application. Cognitive complexity is a code metric designed to measure how difficult code is for humans to understand, focusing on the mental effort required to comprehend control flow.

## What is Cognitive Complexity?
Cognitive Complexity is a code metric developed by SonarSource in 2017 that measures the difficulty of understanding code. Unlike traditional metrics like Cyclomatic Complexity that focus on the number of paths through code, Cognitive Complexity prioritizes human comprehension by:

- Incrementing for control flow structures (`if`, `for`, `while`, etc.)
- Adding higher penalties for nested structures based on nesting depth
- Accounting for boolean operators that break linear reading flow
- Not penalizing "simplifying" structures like breaks and early returns

This makes it particularly useful for:
- Identifying maintenance hotspots in codebases
- Prioritizing refactoring efforts
- Improving developer onboarding experience
- Reducing defect rates (high complexity code tends to have more bugs)

## Key Findings
- **Extreme Concentration**: The dashboard page (205) accounts for 32% of the project's total complexity
- **File Type Patterns**: Page components show the highest complexity, followed by React components and API routes
- **Pareto Distribution**: 8 files (25% of the codebase) account for ~80% of the total complexity
- **Severity Breakdown**: 15.6% of files have critical complexity (>25), requiring immediate attention

## Tools Used
- **SonarQube**: For static code analysis and complexity measurement
- **Python**: For data processing and visualization
- **Pandas/Matplotlib**: For generating complexity analysis charts
- **Git**: For version control

## Repository Contents
- `/data`: CSV file with raw complexity metrics
- `/images`: Data visualizations and charts
- `report.md`: Detailed analysis of the cognitive complexity findings

## Visualization Examples
- Top files by complexity
- Distribution by severity categories
- Pareto analysis of cumulative impact
- File type complexity distribution 

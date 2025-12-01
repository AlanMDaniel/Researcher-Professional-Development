---
layout: default
title: Protocol A \- Computational Workflow
description: Technical guide for protecting code authorship using GitHub Forks, Zenodo DOIs, and git hashing.
keywords: git fork, zenodo doi, protect my code, github for academics, code authorship
---

# **Protocol A: Computational Workflow**

**Implementation Guide for Code and Data Heavy Research**

This protocol provides the technical steps to implement Digital Sovereignty using version control systems. It is designed for researchers using Python, R, MATLAB, or other scripting languages.

## **1\. The Fork Protocol (Ownership)**

When working on a project hosted in a laboratory organization account (e.g., github.com/LabName/Project), you do not own the repository. To ensure you retain a copy of your contribution:

Create a Fork:  
Do not just clone the lab repo. Click the "Fork" button in the top right corner of the GitHub interface to create a copy under your personal username (github.com/YourName/Project).  
Configure Remotes:  
Set up your local environment to push to both the lab (for collaboration) and your personal fork (for backup).  
git remote add upstream \[https://github.com/LabName/Project.git\](https://github.com/LabName/Project.git)  
git remote add origin \[https://github.com/YourName/Project.git\](https://github.com/YourName/Project.git)

Daily Workflow:  
Push your work to your personal fork (origin) daily. Submit Pull Requests to the lab repo (upstream) when ready for review. This ensures your commit history is preserved even if the lab repo is deleted or your access is revoked.

## **2\. The Zenodo Handshake (Timestamping)**

Git history is mutable; a DOI is permanent. To create an unalterable, citable record of your code:

1. **Link Accounts:** Log in to [Zenodo.org](https://zenodo.org) using your GitHub credentials.  
2. **Enable Repository:** In Zenodo settings, toggle the switch for your specific repository.  
3. **Create Release:** In GitHub, go to "Releases" \-\> "Draft a new release" \-\> "Publish release."  
4. **Result:** Zenodo automatically snapshots the code state and assigns a **DOI (Digital Object Identifier)**.

Use this DOI when citing your software in manuscripts or CVs. It serves as independent third-party verification of your authorship at a specific point in time.

## **3\. Cryptographic Verification (The Backup)**

If you cannot use Zenodo (e.g., private data), use Git’s internal hashing as proof of possession.

The Hash:  
Every commit generates a SHA-1 hash (e.g., 8f9d12a...). This string is mathematically derived from the exact content of your files.  
The Paper Trail:  
Periodically email the latest commit hash to your supervisor (and BCC your personal archive).

* *Example:* "Hi Professor, the new model is live. The current commit hash is 8f9d12a."

This email proves you possessed that specific codebase at that specific time, as it is mathematically impossible to generate that hash later without the original files.
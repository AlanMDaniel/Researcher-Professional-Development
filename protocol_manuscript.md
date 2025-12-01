---
layout: default 
title: Protocol B \- Manuscript & Archive Workflow 
description: How to protect non-code research using OSF, local archives, and file hashing. For humanities and qualitative researchers. 
keywords: OSF tutorial, protect my thesis, google drive backup, academic archiving, humanities data management
---
# **Protocol B: Manuscript & Archive Workflow**

**Implementation Guide for Humanities and Qualitative Social Sciences**

This protocol provides the technical steps to implement Digital Sovereignty for researchers working primarily with documents, archives, translations, or qualitative data. It is designed for workflows centered on Microsoft Word, Scrivener, Dropbox, or Google Drive.

## **1\. The "Cold Storage" Protocol (Redundancy)**

Cloud synchronization services (Google Drive, Dropbox, Box) are not backups; they are mirrors. If a file is deleted in the cloud (accidentally or intentionally), it is deleted from your computer.

Break the Sync:  
Once a month, you must create a "Cold Copy" of your research materials.

1. Create a folder on your local hard drive (outside of your Dropbox/Drive folder) named Research\_Archive\_\[Month\_Year\].  
2. Copy and paste your active project files into this folder.  
3. Do not edit these files. They are a frozen snapshot.

This protects you against accidental deletion, account lockouts, or administrative wipes of shared folders.

## **2\. The Open Science Framework (Timestamping)**

The Open Science Framework (OSF) allows non-coders to create immutable, timestamped records of their work, similar to a notary public.

**Set Up:**

1. Create a free account at [OSF.io](https://osf.io).  
2. Create a "Project" for your dissertation or research topic.  
3. Link your active storage (Google Drive, Dropbox, Box) in the project settings. This allows you to view your files within OSF without moving them.

The Registration (The Freeze):  
When you finish a chapter, a translation, or a dataset:

1. Go to the "Registrations" tab in your OSF project.  
2. Click "New Registration."  
3. Select "Freeze" or "Archive."

OSF will take a snapshot of all files in the project at that exact second and archive them on their servers. This creates a permanent, read-only record with a date stamp and a persistent link. Even if you or your collaborators delete the original files from Google Drive, the OSF Registration remains as proof of the work's existence and your contribution.

## **3\. The "Poor Man's Blockchain" (Verification)**

If you are working with sensitive data (e.g., oral history audio, ethnographic notes) that cannot be uploaded to *any* server due to privacy concerns:

1. **Zip It:** Compress your work into a single file (e.g., Fieldwork\_Logs\_Nov2025.zip).  
2. **Hash It:** You need a digital fingerprint of this file.  
   * *Windows:* Open PowerShell and type Get-FileHash \[drag file here\].  
   * *Mac:* Open Terminal and type shasum \-a 256 \[drag file here\].  
3. **Email It:** Copy the resulting string of characters (the hash) and email it to yourself and your supervisor.  
   * *Subject:* "Hash Verification for Fieldwork Archive."

This proves that a specific set of files existed in your possession on that date, without requiring you to upload the sensitive content itself.
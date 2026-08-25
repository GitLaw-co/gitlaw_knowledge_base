---
title: Organisation roles and permissions, explained
slug: organisation-roles-and-permissions-explained
category: frequently-asked-questions-faqs
excerpt: GitLaw has two separate kinds of role - one for managing people, one for who can open a specific file. Being an admin doesn't let you read everyone's documents.
---

## The short answer

GitLaw has **two separate kinds of role**:

- **Organisation roles** decide who can manage people and settings.
- **Document roles** decide who can open or edit a specific file.

They're independent. **Being an Org Admin does not let you read everyone's documents.**

## Organisation roles: managing people and settings

| Role          | Can do                                                          | Sees files?                                      |
| ------------- | --------------------------------------------------------------- | ------------------------------------------------ |
| **Org Owner** | Full control - people, roles, billing, settings                 | Only files they own or that are shared with them |
| **Org Admin** | Invite and remove members, change roles (but not manage Owners) | Same as a Member - no special access             |
| **Member**    | No admin powers; can leave anytime                              | Org-shared files, plus files shared with them    |

There must always be at least one Org Owner. An Org Admin can manage people but can't touch Owners - and gets **no** special access to anyone's private documents.

## Document roles: who can open a specific file

| Role       | Can do                                 |
| ---------- | -------------------------------------- |
| **Owner**  | Full control of the file; can share it |
| **Editor** | Edit the file; can share it            |
| **Viewer** | View the file only                     |

Every file is either **shared with the organisation** or **private** - you choose. Being an **Org Owner** does not grant access to other members' private documents. Only a file's **Owner** or **Editor** can share it.

## Why the split matters

Someone can help run your organisation without being able to read its contracts. You can delegate the admin work without giving away the confidential detail.

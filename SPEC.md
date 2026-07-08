# Project Name

OpenForm Builder

---

# Goal

Develop a web application similar to Ragic.

The system is a Low-Code Database Platform.

Users can build their own database tables by dragging fields onto an Excel-like canvas.

The UI should resemble:

- Ragic
- Airtable
- Google Sheets
- Notion Database

This project must be scalable, clean architecture, component-based, and production ready.

---

# Tech Stack

Frontend

- Next.js 15
- React 19
- TypeScript
- TailwindCSS
- shadcn/ui
- React Hook Form
- TanStack Table
- TanStack Query
- Zustand
- dnd-kit
- react-resizable
- react-window
- Framer Motion

Backend

- NestJS
- Prisma
- PostgreSQL
- Redis
- JWT Authentication
- RBAC Permission

Storage

- MinIO (S3 Compatible)

Deployment

- Docker
- Docker Compose

---

# UI Layout

```text
----------------------------------------------------------
Top Toolbar
----------------------------------------------------------

Logo

Current Form Name

Save

Preview

Undo

Redo

Publish

Design Mode

Data Mode

Search

Profile

----------------------------------------------------------
Left Sidebar
----------------------------------------------------------

Field Toolbox

System Fields

Components

Templates

----------------------------------------------------------
Center
----------------------------------------------------------

Spreadsheet Designer

Excel Grid

----------------------------------------------------------
Right Sidebar
----------------------------------------------------------

Field Properties

Layout Properties

Validation

Permission

----------------------------------------------------------
```

Dark Mode supported.

Responsive.

---

# Excel Designer

Create an Excel-like designer.

Support:

Rows

Columns

Resize Row

Resize Column

Merge Cells

Split Cells

Freeze Row

Freeze Column

Drag Cells

Copy Cells

Paste Cells

Delete Cells

Insert Row

Insert Column

Undo

Redo

Zoom

Auto Save

Infinite Scroll

Keyboard shortcuts:

Ctrl+C

Ctrl+V

Ctrl+X

Delete

Tab

Enter

Arrow Keys

Ctrl+Z

Ctrl+Y

Double Click Edit

---

# Field Toolbox

Users drag fields from the toolbox.

Available fields:

Single Line Text

Multi Line Text

Rich Text

Markdown

Number

Currency

Percent

Date

Datetime

Time

Checkbox

Radio

Dropdown

Multi Select

User

Department

Phone

Email

URL

Image Upload

File Upload

Signature

Location

Address

Auto Number

UUID

Barcode

QR Code

Formula

Lookup

Rollup

Relation

Button

Rating

Color

Progress

Password

JSON

Hidden Field

Separator

Section Title

---

# Field Properties

Every field has:

Field Name

Field ID

Description

Placeholder

Required

Read Only

Unique

Default Value

Validation

Max Length

Min Length

Regex

Width

Height

Background Color

Font Color

Visible

Permission

Display Condition

Calculation Formula

Lookup Source

Relation Table

Sorting

Filtering

Index

---

# Layout

Each cell stores:

Row

Column

RowSpan

ColSpan

Width

Height

Field ID

Alignment

Padding

Border

Background

Visibility

---

# Design Mode

Users can:

Drag fields

Delete fields

Move fields

Resize

Merge

Split

Duplicate

Copy

Paste

Import Layout

Export Layout

Preview

---

# Data Mode

Users fill records.

Supports:

Create Record

Edit Record

Delete Record

Copy Record

Import Excel

Export Excel

Export CSV

Print

Search

Filter

Sort

Grouping

Pagination

---

# Database Structure

Users

Roles

Permissions

Forms

Layouts

Fields

Records

RecordValues

Attachments

Comments

History

AuditLogs

Notifications

Favorites

Folders

Templates

---

# Prisma Schema

Design normalized tables.

Support:

One-to-Many

Many-to-Many

Cascade Delete

Soft Delete

Versioning

Audit Trail

---

# API

REST API

Authentication

POST /login

POST /logout

POST /refresh

Forms

GET /forms

POST /forms

PUT /forms/:id

DELETE /forms/:id

Fields

GET /fields

POST /fields

PUT /fields/:id

DELETE /fields/:id

Layouts

GET /layouts

PUT /layouts

Records

GET /records

POST /records

PUT /records/:id

DELETE /records/:id

Upload

POST /upload

Search

GET /search

---

# Permission

Role Based Access Control

Roles

Admin

Developer

Manager

Editor

Viewer

Guest

Permission

Read

Write

Delete

Export

Import

Approve

Publish

---

# File Upload

Support

Image

PDF

Word

Excel

ZIP

Video

Store in MinIO

Preview image

Download file

---

# Formula Engine

Support formulas similar to Excel.

Functions:

SUM()

COUNT()

AVERAGE()

IF()

AND()

OR()

LEFT()

RIGHT()

MID()

TODAY()

NOW()

DATE()

YEAR()

MONTH()

DAY()

ROUND()

ABS()

MAX()

MIN()

LOOKUP()

---

# Search Engine

Global Search

Filter Builder

Advanced Search

Saved Search

Quick Search

---

# Dashboard

Statistics

Recent Forms

Favorite Forms

Recent Records

Notifications

Charts

Activity

---

# UI Components

Button

Input

Textarea

Select

Checkbox

Switch

Radio

DatePicker

Modal

Drawer

Popover

Tooltip

Dropdown Menu

Tabs

Accordion

Card

Toast

Table

Tree

Breadcrumb

Context Menu

Loading

Skeleton

Avatar

Badge

Pagination

---

# Themes

Light

Dark

Custom Theme

Accent Color

---

# Audit Log

Record every action.

Create

Update

Delete

Login

Permission Change

Export

Import

---

# Notifications

System Notification

Mention

Assignment

Approval

Email Notification

---

# History

Every record supports version history.

Restore previous version.

---

# Auto Save

Every 5 seconds.

Only save changed fields.

---

# Performance

Virtual Scroll

Lazy Loading

Code Splitting

Memoization

Optimistic Update

Caching

---

# Docker

Provide

Dockerfile

docker-compose.yml

.env.example

---

# Testing

Unit Test

Integration Test

E2E Test

Playwright

Vitest

---

# Code Quality

Use ESLint

Prettier

Strict TypeScript

Reusable Components

Atomic Design

Repository Pattern

Service Layer

No duplicated code.

---

# Git Strategy

Every milestone must create one Git commit.

Commit format:

feat:

fix:

refactor:

style:

docs:

test:

---

# Development Milestones

Milestone 1

Create project

Setup Next.js

Setup NestJS

Setup Prisma

Setup PostgreSQL

Docker

Authentication

Commit

---

Milestone 2

Layout

Sidebar

Toolbar

Responsive

Dark Mode

Commit

---

Milestone 3

Spreadsheet Engine

Grid

Resize

Merge

Keyboard

Commit

---

Milestone 4

Drag and Drop Builder

Field Toolbox

Designer

Commit

---

Milestone 5

Database Schema

CRUD

Commit

---

Milestone 6

Record Entry

Validation

Commit

---

Milestone 7

Formula Engine

Lookup

Relation

Commit

---

Milestone 8

Import Export

Excel

CSV

PDF

Commit

---

Milestone 9

Permission

Audit

History

Commit

---

Milestone 10

Dashboard

Charts

Notification

Performance Optimization

Final Testing

Commit

---

# Important Rules

Never generate placeholder code.

Never leave TODO.

Never skip implementation.

Every feature must be production ready.

Every component must be reusable.

Always explain what will be implemented before generating code.

Never generate more than one milestone at a time.

Wait for confirmation before continuing to the next milestone.

---

# Codex Instructions

請擔任我的 Senior Full Stack Engineer。

請完全依照 SPEC.md 開發。

不要一次產生全部程式碼。

每次只完成一個 Milestone。

完成後：

1. 說明本次實作內容。
2. 建立完整檔案結構。
3. 提供所有程式碼（不可省略）。
4. 說明如何執行。
5. 說明測試方式。
6. 提供 Git Commit Message。
7. 等待我輸入「Continue」後再進入下一個 Milestone。

所有程式碼必須可直接執行，不允許使用 TODO、Placeholder、Mock 或偽代碼。

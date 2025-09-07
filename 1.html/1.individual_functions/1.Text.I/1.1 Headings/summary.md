**STAGEPROJECT: HTML headings**

---

[[Project title]]  
**HTML headings - Practice Pack**

---

[[1.1 Practice evey Day]]

## 📝 Description

This pack focuses exclusively on the correct and semantically appropriate use of HTML heading tags `<h1>` to `<h6>` within valid document structures.

## 🔧 Functional Requirements Implemented

-  Correct usage of each heading level (`<h1>` to `<h6>`)
    
-  Semantic nesting of heading levels
    
-  Validation of heading structure in full HTML documents
    
-  Use of headings to define content sections
    
-  Accessibility compliance (hierarchical structure)
    

## 🌟 Stretch Goals (Optional)

-  Dynamic heading structure for content-driven templates
    
-  ARIA landmarks with headings
    

## ⏱ Time Log

Estimated: 2 hours  
Actual: TBD

## 📚 Concepts Practiced

- Structural use of `<h1>`–`<h6>`
    
- Heading hierarchy
    
- Valid nesting and semantic flow
    
- W3C validation
    
- Accessibility via heading outline
    

## 📌 Notes

Emphasis is placed on heading levels and their semantic importance. Minimal markup used solely to ensure validation and outline clarity.

---

STAGEPROJECT: HTML headings

## **Stage**: HTML headings

## 🎓 Learning Objectives

- Use all six heading tags (`<h1>` through `<h6>`) appropriately
    
- Ensure heading structure is hierarchical and semantically valid
    
- Validate heading usage with W3C
    
- Apply heading tags inside valid HTML wrappers
    
- Detect and correct incorrect heading orders
    
- Recognize heading roles in accessibility and navigation
    

---

## 🧪 1. Microproject Set (choose count and justify)

**Number of microprojects chosen: 3 — Heading tags are limited in complexity, so three microprojects are sufficient to explore their structure, hierarchy, and role in document sections.**

---

### 1. Full Heading Spectrum — Use all `<h1>` to `<h6>` once
- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: A document containing all heading tags `<h1>` through `<h6>` in order
- **Constraints**: All heading tags must be present, used once, and in order from `<h1>` to `<h6>`
- **Acceptance tests**:
    - The document contains exactly one of each `<h1>` to `<h6>` tag
    - W3C validator should return no errors
- **Example(s)**:
    - `index.html`: A page titled "Heading Levels" with headings from `<h1>` to `<h6>` used in descending order
- **Notes**: Minimal wrapper (`<html><body>`) required for validation compliance

---

### 2. Nested Headings in Sectioned Content
- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: A document with `<h1>` as main title, and sections using `<h2>`/`<h3>` as nested headings
- **Constraints**: Must use at least three heading levels, with proper semantic nesting
- **Acceptance tests**:
    - All headings are used hierarchically (no `<h3>` before `<h2>`)
    - W3C validator returns no errors
    - `document.querySelector("h1") !== null`
- **Example(s)**:
    - `index.html`: A page with a main topic and two subtopics using `<h2>`, one sub-subtopic using `<h3>`
- **Notes**: `<section>` tags allowed to group logical units with headings

---

### 3. Outline Validation — Heading hierarchy in real content

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: A page with a heading structure that forms a valid, logical outline of content (e.g., a report or article)
    
- **Constraints**: Use at least four headings in total, but avoid skipping levels
    
- **Acceptance tests**:
    
    - No heading level is skipped (e.g., no `<h4>` following `<h2>`)
        
    - Outline structure reflects logical nesting when viewed in assistive tools
        
- **Example(s)**:
    
    - `index.html`: An article layout with `<h1>`, two `<h2>`s, each with `<h3>` children
        
- **Notes**: `<article>` used only to reflect realistic structure without adding new elements
    

---

## 🧠 2. Applied Problem Set (choose counts and justify)

**Total problems chosen: 12 — justification: HTML headings are foundational and simple; therefore, 8 Basic and 4 Intermediate problems are sufficient. No Advanced required.**

---

### [Basic] — Problem 1: Use One `<h1>`

- **Statement**: Create a document with one and only one `<h1>` element
    
- **Input**: none
    
- **Expected output**: HTML document with a single `<h1>`
    
- **Constraints**: Must not include other heading tags
    
- **Example**:
    
    - Input: none
        
    - Output: HTML with only one `<h1>` tag
        
- **Acceptance tests**:
    
    - `document.querySelectorAll("h1").length === 1`
        
    - W3C validation returns 0 errors
        

---

### [Basic] — Problem 2: Add Three Levels of Headings

- **Statement**: Add a `<h1>`, followed by a `<h2>` and `<h3>`
    
- **Input**: A skeleton HTML file
    
- **Expected output**: Three levels of headings in hierarchical order
    
- **Constraints**: No skipped levels
    
- **Example**:
    
    - Input: `<body></body>`
        
    - Output: `<h1>`, `<h2>`, `<h3>`
        
- **Acceptance tests**:
    
    - Heading order is valid
        
    - `document.querySelector("h2").previousElementSibling.tagName === "H1"`
        

---

### [Basic] — Problem 3: Identify Wrong Order

- **Statement**: A file has `<h1>`, `<h3>`, `<h2>` — fix the order
    
- **Input**: HTML with incorrect heading nesting
    
- **Expected output**: `<h1>` → `<h2>` → `<h3>`
    
- **Constraints**: No level skipping
    
- **Example**:
    
    - Input: `<h1>Title</h1><h3>Detail</h3><h2>Subsection</h2>`
        
    - Output: Proper nested order
        
- **Acceptance tests**:
    
    - DOM hierarchy is linear
        
    - `querySelector("h2").compareDocumentPosition(querySelector("h3")) === Node.DOCUMENT_POSITION_FOLLOWING`
        

---

### [Basic] — Problem 4: Use All Even Headings

- **Statement**: Use only `<h2>`, `<h4>`, and `<h6>`
    
- **Input**: none
    
- **Expected output**: Page with only even-level headings
    
- **Constraints**: Do not include `<h1>`, `<h3>`, `<h5>`
    
- **Example**:
    
    - Output: Headings are even-numbered levels
        
- **Acceptance tests**:
    
    - `querySelector("h1") === null`
        
    - All present headings match `/h[246]/`
        

---

### [Basic] — Problem 5: Replace Paragraphs with Headings

- **Statement**: Convert paragraph content to appropriate heading levels
    
- **Input**: `<p>Main Title</p><p>Sub Title</p>`
    
- **Expected output**: Replace with `<h1>`, `<h2>`
    
- **Constraints**: Only replace content, do not add new content
    
- **Example**: See input
    
- **Acceptance tests**:
    
    - No `<p>` tags remain
        
    - Headings reflect correct nesting
        

---

### [Basic] — Problem 6: Create FAQ Structure

- **Statement**: Use `<h2>` for each FAQ question
    
- **Input**: A list of FAQ entries (text only)
    
- **Expected output**: Each question wrapped in `<h2>`
    
- **Constraints**: One heading per question
    
- **Example**:
    
    - Input: “What is HTML?”, “What is CSS?”
        
    - Output: `<h2>` elements for both
        
- **Acceptance tests**:
    
    - `querySelectorAll("h2").length === 2`
        
    - All questions are inside `<h2>`
        

---

### [Basic] — Problem 7: Count and Validate Heading Tags

- **Statement**: Ensure that the document has six headings total
    
- **Input**: HTML with unknown structure
    
- **Expected output**: Exactly six headings
    
- **Constraints**: Can be any levels
    
- **Example**: Input has mix of heading tags
    
- **Acceptance tests**:
    
    - `document.querySelectorAll("h1, h2, h3, h4, h5, h6").length === 6`
        

---

### [Basic] — Problem 8: Accessibility Outline with Headings

- **Statement**: Create a structure that screen readers can use to navigate
    
- **Input**: none
    
- **Expected output**: Heading hierarchy that reflects content outline
    
- **Constraints**: No level skipping
    
- **Example**: n/a
    
- **Acceptance tests**:
    
    - Headings reflect nesting
        
    - Outline view reflects page structure
        

---

### [Intermediate] — Problem 9: Fix a Skipped Heading Level

- **Statement**: Correct an HTML where `<h1>` is followed by `<h4>`
    
- **Input**: HTML snippet
    
- **Expected output**: Proper intermediate heading levels added
    
- **Constraints**: Do not remove any content
    
- **Example**: see input
    
- **Acceptance tests**:
    
    - `<h2>` and `<h3>` inserted appropriately
        
    - No skipped levels remain
        

---

### [Intermediate] — Problem 10: Reorder Headings in a Document

- **Statement**: Given headings out of order, restructure them semantically
    
- **Input**: HTML file with random heading levels
    
- **Expected output**: Clean, hierarchical heading flow
    
- **Constraints**: Use only original text content
    
- **Example**: Input contains `<h1>`, `<h5>`, `<h3>`
    
- **Acceptance tests**:
    
    - Headings ordered by level
        
    - Validation passes
        

---

### [Intermediate] — Problem 11: Add Headings to Article Sections

- **Statement**: Given sections of an article, apply appropriate headings
    
- **Input**: Article without headings
    
- **Expected output**: Each section begins with a heading
    
- **Constraints**: Use `<h1>` once, then proper nesting
    
- **Acceptance tests**:
    
    - Sections begin with heading
        
    - `<h1>` used only once
        

---

### [Intermediate] — Problem 12: Convert Div Labels to Headings

- **Statement**: Replace `<div class="section-title">` with semantic headings
    
- **Input**: HTML using `<div>`s for titles
    
- **Expected output**: Replace all with correct `<h2>` or `<h3>`
    
- **Constraints**: Match nesting level by position
    
- **Acceptance tests**:
    
    - All `div.section-title` replaced with headings
        
    - DOM depth matches heading level
        

---

## ⚙️ 3. Debugging & Refactor Challenge

**Chosen count: 2 — one with incorrect order and one with repeated headings. These represent common, realistic structural mistakes in heading usage.**

---

### 🔧 Challenge 1: Broken Heading Order

#### **Broken code**

`<!DOCTYPE html> <html lang="en">   <head>     <title>About Page</title>   </head>   <body>     <h1>About Our Company</h1>     <h3>History</h3>     <h2>Mission & Vision</h2>     <h4>Core Values</h4>   </body> </html>`

---

### 🔧 Challenge 2: Repeated `<h1>` and Inconsistent Nesting

#### **Broken code**

`<!DOCTYPE html> <html lang="en">   <head>     <title>Services</title>   </head>   <body>     <h1>Our Services</h1>     <h1>Consulting</h1>     <h3>Technical</h3>     <h5>DevOps</h5>     <h4>Cloud</h4>   </body> </html>`

---

### 🧠 Instructions

For each code sample:

1. **List all bugs or semantic violations you detect**
    
2. **Write a corrected version of the code**
    
3. **Propose 2–3 short refactor suggestions** to improve semantic structure or accessibility (without introducing non-heading concepts)
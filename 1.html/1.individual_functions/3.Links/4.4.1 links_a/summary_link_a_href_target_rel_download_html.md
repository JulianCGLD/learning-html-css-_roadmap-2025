**STAGEPROJECT: 4.4.1 link_a_href_target_rel_download_html**

[[Project title]]  
4.4.1 link_a_href_target_rel_download_html - Practice Pack

[[1.1 Practice evey Day]]

## 📝 Description

This practice pack focuses on mastering the `<a>` element in HTML and the correct use of its `href`, `target`, `rel`, and `download` attributes.

## 🔧 Functional Requirements Implemented

-  Use of `href` to link internal and external resources
    
-  Use of `target="_blank"` to open links in new tabs
    
-  Use of `rel` to define relationship between documents
    
-  Use of `download` attribute to initiate file download
    
-  Combinations of `target` and `rel` for safe navigation
    
-  Accessibility considerations using descriptive link text
    

## 🌟 Stretch Goals (Optional)

-  Use of custom filename in `download`
    
-  Multiple anchor elements in a single document with different attribute combinations
    

## ⏱ Time Log

Estimated time: 60–75 minutes  
Actual time: TBD

## 📚 Concepts Practiced

- Anchor element `<a>`
    
- `href` linking behavior
    
- Target and rel interaction
    
- Download mechanism
    
- HTML5 validation
    
- Secure hyperlinking
    
- Attribute ordering and syntax correctness
    

## 📌 Notes

- No CSS or JS included
    
- Examples and tasks focused strictly on structural validity and behavior
    
- Tested via W3C validator and manual DOM query examples
    

---

STAGEPROJECT: 4.4.1 link_a_href_target_rel_download_html

## **Stage**: 4.4.1 link_a_href_target_rel_download_html

## 🎓 Learning Objectives

- Correctly implement `<a>` with required `href` attribute
    
- Use `target="_blank"` and `rel="noopener"` to secure new tab links
    
- Apply `download` to anchor elements and validate filename behavior
    
- Combine attributes correctly while maintaining HTML5 compliance
    
- Detect and fix structural and attribute misuse in anchor elements
    

---

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 4 — This number covers the major combinations of attribute functionality without unnecessary duplication.

---

### 1. Name — link_to_internal_page_with_href_only

- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: A clickable link to "page.html" inside the same directory
- **Constraints**: Must only use `<a>` with `href`
- **Acceptance tests**:
    - DOM must contain `<a>` with `href="page.html"`
    - W3C validator must show no errors
- **Example(s)**:  
    File: index.html  
    (include `<a href="page.html">Go to Page</a>`)
- **Notes**: Wrapped in `<body>` for valid structure
- DO NOT USE: `target`, `rel`, `download`, scripts, or styles

---

### 2. Name — external_link_that_opens_in_new_tab_safely.html

- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: A link to "[https://example.com](https://example.com/)" opens in new tab
- **Constraints**: Must include `target="_blank"` and `rel="noopener"`
- **Acceptance tests**:
    - DOM must contain `target="_blank"`
    - DOM must contain `rel="noopener"`
- **Example(s)**:  
    File: index.html  
    (include `<a href="https://example.com" target="_blank" rel="noopener">Visit Example</a>`)
- **Notes**: `<rel>` is required for security
- DO NOT USE: `download`, unnecessary nesting, or inline styles


---

### 3. Name — File download with custom filename

- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: A link downloads "report.pdf" and saves as "Annual_Report_2025.pdf"
- **Constraints**: Must include `download="Annual_Report_2025.pdf"`
- **Acceptance tests**:
    - DOM must contain `download="Annual_Report_2025.pdf"`
    - File URL must be reachable in `href`
- **Example(s)**:  
    File: index.html  
    (include `<a href="report.pdf" download="Annual_Report_2025.pdf">Download Report</a>`)
- **Notes**: `download` requires same-origin for browser compatibility
- DO NOT USE: `target`, `rel`, or JavaScript-based download handling
    

---

### 4. Name — combination_external_download_link opens_in_new_tab.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: Opens a new tab and downloads `guide.pdf`
    
- **Constraints**: Must combine `href`, `target`, `rel`, `download`
    
- **Acceptance tests**:
    
    - DOM must contain all four attributes (`href`, `target`, `rel`, `download`)
        
    - Link must pass HTML5 validation
        
- **Example(s)**:  
    File: index.html  
    (include `<a href="guide.pdf" target="_blank" rel="noopener" download>Get Guide</a>`)
    
- **Notes**: All attributes required to fulfill compound behavior
    
- DO NOT USE: styling, embedded scripting, non-link elements
    

---

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 12 — [justification: Full attribute set benefits from progressive, combinatory tasks that increase in complexity]

- Basic: 6
    
- Intermediate: 4
    
- Advanced: 2
    

---


### [Basic] — 1.problem_1_blank_rel_safe.html

- **Statement**: Secure a new-tab external link
    
- **Input**: none
    
- **Expected output**: `<a href="..." target="_blank" rel="noopener">`
    
- **Constraints**: Required `target` and `rel`
    
- **Example**: Link to `https://news.com`
    
- **Acceptance tests**:
    
    - DOM shows both attributes
        
    - Rel must include `noopener`
        
- DO NOT USE: `download`
    

---

### [Basic] — 2.problem_2_download_file.html

- **Statement**: Create a download link for `document.pdf`
    
- **Input**: none
    
- **Expected output**: Anchor that downloads
    
- **Constraints**: Must use `download` and valid `href`
    
- **Example**:  
    `<a href="document.pdf" download>`
    
- **Acceptance tests**:
    
    - Link triggers download on click
        
    - No validation errors
        
- DO NOT USE: `target`, `rel`
    

---

### [Basic] — 3.problem_3_multiple_links.html

- **Statement**: Add 3 different `<a>` links with different behaviors
- **Input**: none
- **Expected output**: 1 internal, 1 external new-tab, 1 download
- **Constraints**: Each anchor must vary
- **Example**:  
    Include at least one `download`, one `target`, and one plain
- **Acceptance tests**:
    - Three `<a>` elements present
    - Attributes applied correctly
- DO NOT USE: scripts, CSS
    

---

### [Intermediate] — 4.problem_4_external_download_blank.html

- **Statement**: Download an external file in new tab
    
- **Input**: none
    
- **Expected output**: `<a href="..." download target="_blank" rel="noopener">`
    
- **Constraints**: All 4 attributes required
    
- **Example**: PDF download
    
- **Acceptance tests**:
    
    - DOM contains full attribute set
        
    - W3C validation passes
        
- DO NOT USE: media tags, script
    

---


### [Advanced] — 5.problem_5_invalid_download_external.html

- **Statement**: Attempt download from disallowed external domain
- **Input**: none
- **Expected output**: Download fails due to COR
- **Constraints**: Must document the error
- **Example**: Remote URL
- **Acceptance tests**:
    - Console error or blocked action
    - Download doesn't trigger
- DO NOT USE: workaround techniques

---

### [Advanced] — 6.problem_6_missing_rel_blank.html

- **Statement**: Use `target="_blank"` without `rel`; explain risk
- **Input**: None
- **Expected output**: Highlight window.opener risk
- **Constraints**: Omission must be deliberate
- **Example**:  
    `<a href="..." target="_blank">`
- **Acceptance tests**:
    - Missing `rel`

    - Code must not validate as fully secure
- DO NOT USE: fake `rel`, explanations
    

---

## ⚙️ 3. Debugging & Refactor Challenge

Number of snippets: 2 — These reflect the most common real-world errors for anchor attribute misuse

---

### Debug Snippet 1

**Broken code**

```html
<a href="doc.pdf" target="_blank" download="report.pdf" rel>Download</a>
```

**Bug list**  
You must detect: missing value in `rel`, incorrect `download` usage, other possible issues

**Required fix**  
(To be discovered by user)

**Refactor notes**

- Use `rel="noopener"` when opening new tabs
    
- Ensure `download` only applied to same-origin resources
    

---

### Debug Snippet 2

**Broken code**

```html
<a download href="https://example.com" rel="nofollow">External</a>
```

**Bug list**  
To be found: invalid use of `download` for external file, missing `target` for new tab, inappropriate `rel`

**Required fix**  
(To be discovered by user)

**Refactor notes**

- Use `rel="noopener"` with `target="_blank"`
    
- Avoid `download` for cross-origin if not allowed
    

---

## ✅ Final Validation Checklist

- All anchor elements validate in W3C validator
    
- `href` used correctly and consistently
    
- `target="_blank"` includes `rel="noopener"` for safety
    
- `download` only used on same-origin or CORS-allowed URLs
    
- Meaningful link text improves accessibility
    
- No JS or CSS required to pass tests
    

---

## 📌 Grading rubric

- **Correctness** (0–40): Anchor tags behave as required
    
- **Semantics** (0–30): Meaningful link text, proper relationships
    
- **Accessibility** (0–20): Text clarity, no "click here", security rel used
    
- **Tests** (0–10): Validated DOM and HTML5 structure
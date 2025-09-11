**STAGEPROJECT: unordered_list_html**

[[Project title]]  
**STAGEPROJECT - Practice Pack**

[[1.1 Practice evey Day]]

## 📝 Description

Practice pack for mastering the `<ul>` (unordered list) HTML element, including proper nesting, structure, and validation.

## 🔧 Functional Requirements Implemented

-  Correct use of `<ul>` and `<li>` elements
    
-  Validation of unordered list structures
    
-  Nesting of `<ul>` elements
    
-  DOM structural assertions
    
-  Accessibility where applicable
    

## 🌟 Stretch Goals (Optional)

-  Dynamic generation via JavaScript
    
-  ARIA list roles
    

## ⏱ Time Log

Estimated: 60 minutes  
Actual: TBD

## 📚 Concepts Practiced

- Element hierarchy: `<ul>` containing `<li>`
    
- Nesting rules
    
- HTML5 validation
    
- Accessibility semantics
    

## 📌 Notes

Focused on valid, minimal implementations for unordered lists. No CSS, no styling beyond required validation structure. Based solely on HTML5 spec and W3C validator.

---

**STAGEPROJECT: unordered_list_html**

## **Stage**: unordered_list_html

## 🎓 Learning Objectives

1. Use `<ul>` with valid `<li>` children
    
2. Validate unordered list structure using W3C HTML5 rules
    
3. Construct properly nested `<ul>` elements
    
4. Avoid invalid children inside unordered lists
    
5. Implement minimal accessible list structures where applicable
    

---

## 🧪 1. Microproject Set (choose count and justify)

**Number of microprojects chosen: 3 — Scope of `<ul>` is narrow; 3 projects are enough to cover structure, nesting, and validation edge cases.**

---

### 1. Name — basic_unordered_list.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: A valid unordered list of 3 fruit names.
    
- **Constraints**: Must use only `<ul>` and `<li>`; no other elements.
    
- **Acceptance tests**:
    
    1. DOM querySelectorAll('ul > li') should return 3 elements
        
    2. HTML must validate without errors via W3C validator
        
- **Example(s)**:  
    Input: Create a bullet list of Apple, Banana, Cherry using `<ul>`
    
- **Notes**: `<html>`, `<head>`, and `<body>` tags included for validation purposes.
    

---

### 2. Name — nested_unordered_lists.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: A valid nested list with at least one `<ul>` inside another `<li>`.
    
- **Constraints**: Must nest `<ul>` inside `<li>` only; not directly in `<ul>`.
    
- **Acceptance tests**:
    
    1. DOM querySelectorAll('ul ul').length >= 1
        
    2. No HTML errors on W3C validator
        
- **Example(s)**:  
    Input: Nest a list of "Languages" with sublist "Python", "JavaScript"
    
- **Notes**: `<html>` structure included to ensure nesting is parsed correctly.
    

---

### 3. Name — unordered_list_accessibility.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: An unordered list with an ARIA label describing its purpose.
    
- **Constraints**: Must include `aria-label` or `aria-labelledby` for accessibility
    
- **Acceptance tests**:
    
    1. `ul.getAttribute('aria-label')` must return a non-empty string
        
    2. Structure must validate in W3C validator
        
- **Example(s)**:  
    Input: List of navigation sections labeled "Main Navigation"
    
- **Notes**: Added ARIA to improve accessibility and meet WAI-ARIA guidelines.
    

---

## 🧠 2. Applied Problem Set (choose counts and justify)

**Total problems chosen: 12 — [justification: Basic use of `<ul>` is simple, but nesting and validation cases require further testing]**  
Breakdown: Basic (6), Intermediate (4), Advanced (2)

---

### [Basic] — 1.problem_1_create_basic_list.html

- **Statement**: Create an unordered list with 3 book titles.
    
- **Input**: none
    
- **Expected output**: Valid `<ul>` structure with 3 `<li>` elements.
    
- **Constraints**: Do not use `<ol>`, `<div>`, or `<p>`.
    
- **Example**: Input: book names — use only `<ul>` and `<li>`.
    
- **Acceptance tests**:
    
    - querySelectorAll('ul > li').length === 3
        
    - Validates on W3C
        

---

### [Basic] — 2.problem_2_use_ul_only_once.html

- **Statement**: Create a single unordered list; do not create nested lists.
    
- **Input**: none
    
- **Expected output**: One `<ul>` element with at least 2 `<li>`.
    
- **Constraints**: No nested lists; one `<ul>` only.
    
- **Example**: Input: List of car brands
    
- **Acceptance tests**:
    
    - querySelectorAll('ul').length === 1
        
    - No validation errors
        

---

### [Basic] — 3.problem_3_empty_list_items.html

- **Statement**: Create a list of 2 items, each with non-empty content.
    
- **Input**: none
    
- **Expected output**: `<li>` must not be empty.
    
- **Constraints**: No blank or whitespace-only list items.
    
- **Example**: Input: name two planets
    
- **Acceptance tests**:
    
    - All `li.textContent.trim()` length > 0
        
    - Valid HTML
        

---

### [Basic] — 4.problem_4_semantic_purpose.html

- **Statement**: Use an unordered list to group related items semantically.
    
- **Input**: none
    
- **Expected output**: List of animals in one semantic group.
    
- **Constraints**: No unrelated items in list.
    
- **Example**: Input: animal names only
    
- **Acceptance tests**:
    
    - querySelectorAll('ul > li').length >= 2
        
    - Each `<li>` contains animal-related text
        

---

### [Basic] — 5.problem_5_validate_ul_structure.html

- **Statement**: Create a valid unordered list.
    
- **Input**: none
    
- **Expected output**: Properly nested and valid `<ul>`
    
- **Constraints**: Do not use invalid child tags inside `<ul>`
    
- **Example**: Input: 3 types of metal
    
- **Acceptance tests**:
    
    - Only `<li>` elements inside `<ul>`
        
    - Passes HTML validation
        

---

### [Basic] — 6.problem_6_ul_with_ids.html

- **Statement**: Create a `<ul>` with an `id` and 3 items.
    
- **Input**: none
    
- **Expected output**: Unordered list with `id="features"`
    
- **Constraints**: No classes, only `id` allowed
    
- **Example**: Input: List of features
    
- **Acceptance tests**:
    
    - `ul#features` exists
        
    - Contains 3 `<li>`
        

---

### [Intermediate] — 8.problem_8_two_nested_lists.html

- **Statement**: Use two nested unordered lists in separate `<li>` elements.
    
- **Input**: none
    
- **Expected output**: 2 distinct nested lists
    
- **Constraints**: Max depth: 2
    
- **Example**: Input: "Food" and "Drinks" each with 2 items
    
- **Acceptance tests**:
    
    - querySelectorAll('ul ul').length === 2
        
    - Valid HTML
        

---

### [Intermediate] — 9.problem_9_aria_label_for_list.html

- **Statement**: Add ARIA label to describe list purpose.
    
- **Input**: none
    
- **Expected output**: `aria-label` must describe content purpose
    
- **Constraints**: ARIA label required
    
- **Example**: Input: list of commands
    
- **Acceptance tests**:
    
    - `ul[aria-label]` exists
        
    - `aria-label.length > 0`
        

---


### [Advanced] — 12.problem_12_accessible_navigation_list.html

- **Statement**: Build a navigation list with ARIA support
    
- **Input**: none
    
- **Expected output**: `<ul>` with `role="navigation"` or `aria-label`
    
- **Constraints**: Must pass accessibility tests
    
- **Example**: list of page sections
    
- **Acceptance tests**:
    
    - `ul[aria-label]` or `ul[role="navigation"]` present
        
    - Contains only `<li>` children
        

---

## ⚙️ 3. Debugging & Refactor Challenge

**Count chosen: 2 — to address both structural and accessibility issues**

---

### Debug 1 — malformed_ul_list.html

**Broken code**:

```html
<ul>
  <div>Item 1</div>
  <li>Item 2</li>
  <li></li>
</ul>
```

---

### Debug 2 — invalid_nested_list.html

**Broken code**:

```html
<ul>
  <li>Level 1
    <ul>
      <ul>
        <li>Level 2</li>
      </ul>
    </ul>
  </li>
</ul>
```

---

## ✅ Final Validation Checklist

- All exercises validate without W3C errors
    
- No `<ul>` contains invalid children
    
- All nested lists follow correct hierarchy
    
- Accessibility attributes used when relevant
    
- No `<ul>` used where `<ol>` or `<dl>` is semantically required
    

---

## 📌 Grading rubric

|Criterion|Points|Description|
|---|---|---|
|Correctness|0–40|Uses `<ul>` and `<li>` correctly|
|Semantics|0–30|Proper nesting, valid children only|
|Accessibility|0–20|ARIA labels where appropriate|
|Tests|0–10|DOM assertions and validation checks exist|

---
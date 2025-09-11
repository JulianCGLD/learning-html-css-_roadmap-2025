**STAGEPROJECT: ordered lists HTML**

[[Project title]]  
`ordered lists HTML - Practice Pack`

[[1.1 Practice evey Day]]

## 📝 Description

Master the use of `<ol>` in HTML through microprojects, applied exercises, and debugging to ensure full semantic and structural correctness.

## 🔧 Functional Requirements Implemented

-  Create basic ordered lists using `<ol>` and `<li>`
    
-  Use `type`, `start`, and `reversed` attributes
    
-  Nest `<ol>` inside list items
    
-  Ensure semantic correctness and accessibility
    
-  Validate structure using W3C standards
    

## 🌟 Stretch Goals (Optional)

-  Combine `<ol>` with other list types in complex structures
    
-  Dynamic list manipulation (JavaScript not allowed per constraints)
    

## ⏱ Time Log

Estimated: 90 minutes  
Actual: TBD

## 📚 Concepts Practiced

- Ordered list creation
    
- Semantic ordering
    
- Attribute usage: `type`, `start`, `reversed`
    
- List nesting
    
- HTML5 validation
    
- Accessibility checks (screen reader implications of list order)
    

## 📌 Notes

All exercises are runnable and valid HTML. Minimal wrappers (`<html>`, `<head>`, `<body>`) were included for standards compliance.

---

STAGEPROJECT: ordered lists HTML

## **Stage**: ordered lists HTML

## 🎓 Learning Objectives

- Correctly implement ordered lists using `<ol>` and `<li>`
    
- Apply and validate `type`, `start`, and `reversed` attributes
    
- Maintain semantic correctness with nested list structures
    
- Ensure all lists pass W3C validation
    
- Demonstrate understanding of accessibility implications of list ordering
    

---

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 4 — This number is sufficient to isolate and master each facet of `<ol>` functionality without redundancy.

---

### 1. Name — basic_ordered_list.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: An ordered list with three steps, numbered automatically
    
- **Constraints**: Must use only `<ol>` and `<li>`; no attributes
    
- **Acceptance tests**:
    
    1. Document contains a single `<ol>` element with 3 `<li>` children
        
    2. W3C validator returns no errors
        
- **Example(s)**:
    
    - Input: A 3-step process
        
- **Notes**: HTML wrapper required for valid output — used only `<html>`, `<head>`, `<body>` tags
    
- **Do NOT use**: CSS, JavaScript, other HTML list types
    

---

### 2. Name — ordered_list_with_type_attribute.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: An ordered list using uppercase letters (A, B, C)
    
- **Constraints**: Must use `<ol type="A">`
    
- **Acceptance tests**:
    
    1. The `<ol>` element has attribute `type="A"`
        
    2. List items render with uppercase letters
        
- **Example(s)**:
    
    - Input: A list of book titles
        
- **Notes**: Wrapper tags required
    
- **Do NOT use**: CSS to simulate list styles
    

---

### 3. Name — ordered_list_with_start_attribute.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: An ordered list starting from 5
    
- **Constraints**: Must use `<ol start="5">`
    
- **Acceptance tests**:
    
    1. The `<ol>` element has attribute `start="5"`
        
    2. First item visually shows number 5
        
- **Example(s)**:
    
    - Input: Top 3 items starting from rank 5
        
- **Notes**: Wrapper tags used
    
- **Do NOT use**: JavaScript to manipulate numbering
    

---

### 4. Name — reversed_ordered_list.html

- **Files**: index.html
    
- **Input**: none
    
- **Expected output / rendered result**: List rendered in descending order
    
- **Constraints**: Must use `reversed` attribute only
    
- **Acceptance tests**:
    
    1. The `<ol>` element has boolean `reversed` attribute
        
    2. List items render in descending order
        
- **Example(s)**:
    
    - Input: Countdown list
        
- **Notes**: Required HTML wrapper only
    
- **Do NOT use**: CSS counters, JS
    

---

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 13 — [Scope is moderate; selected 8 Basic, 4 Intermediate, 1 Advanced for progressive mastery.]

---

### [Basic] — 1.problem_1_ordinal_suffix_in_text.html

- **Statement**: Create a numbered list where each item uses `<ol>` and `<li>` to show ordinal steps
- **Input**:none
- **Expected output**: Ordered list showing ordinal order (1st, 2nd, etc.)
- **Constraints**: Use only `<ol>` and `<li>`
- **Example**:  
    Input: Steps to assemble a desk
    - `<ol><li>Step one</li>...`
- **Acceptance tests**:
    1. Document must contain a valid `<ol>` element
    2. Must validate as HTML5
- **Do NOT use**: CSS numbering, JS

---

### [Basic] — 2.problem_2_type_attribute_variation.html

- **Statement**: Create a list that uses lowercase Roman numerals
    
- **Input**: none
    
- **Expected output**: i, ii, iii...
    
- **Constraints**: Must use `type="i"`
    
- **Example**: A list of ancient empires
    
- **Acceptance tests**:
    
    1. `<ol>` must have `type="i"`
        
    2. All list items render with Roman numerals
        
- **Do NOT use**: `list-style-type`
    

---

### [Basic] — 3.problem_3_start_attribute_effect.html

- **Statement**: Create a list that starts counting from 10
    
- **Input**: none
    
- **Expected output**: 10, 11, 12
    
- **Constraints**: Use `start` only
    
- **Example**: Ranking list
    
- **Acceptance tests**:
    
    1. `start="10"` present
        
    2. First item shows 10
        
- **Do NOT use**: Manual numbering in text
    

---

### [Basic] — 4.problem_4_no_list_repetition.html

- **Statement**: Create a short list of 3 `<li>` elements under `<ol>`
    
- **Input**: none
    
- **Expected output**: Simple ordered list
    
- **Constraints**: No attributes
    
- **Example**: 3 steps to login
    
- **Acceptance tests**:
    
    1. Exactly 3 `<li>` inside `<ol>`
        
    2. Passes HTML validation
        
- **Do NOT use**: `<ul>`, CSS
    

---

### [Basic] — 5.problem_5_multiple_lists.html

- **Statement**: Add two ordered lists in the same document
    
- **Input**: none
    
- **Expected output**: Two separately numbered lists
    
- **Constraints**: No shared attributes
    
- **Example**: Morning tasks / Evening tasks
    
- **Acceptance tests**:
    
    1. Two `<ol>` present
        
    2. Each has at least 2 `<li>`
        
- **Do NOT use**: Nesting
    

---

### [Basic] — 6.problem_6_empty_list_items.html

- **Statement**: Include a warning list and one `<li>` should be empty
    
- **Input**: none
    
- **Expected output**: List renders; one item blank
    
- **Constraints**: Use valid empty `<li></li>`
    
- **Example**: Safety checklist
    
- **Acceptance tests**:
    
    1. One `<li>` has no content
        
    2. Validates with no errors
        
- **Do NOT use**: JS to hide elements
    

---

### [Basic] — 7.problem_7_nested_ol.html

- **Statement**: Nest a second ordered list inside an item of the first
    
- **Input**: none
    
- **Expected output**: One item has sub-items
    
- **Constraints**: Only `<ol>` and `<li>`
    
- **Example**: Recipe steps with substeps
    
- **Acceptance tests**:
    
    1. One `<li>` contains another `<ol>`
        
    2. All elements validate
        
- **Do NOT use**: CSS for indentation
    

---

### [Basic] — 8.problem_8_invalid_tags_in_list.html

- **Statement**: Identify if an invalid element is used inside `<ol>`
    
- **Input**: code snippet
    
- **Expected output**: W3C validation fails
    
- **Constraints**: `<ol>` should contain only `<li>`
    
- **Example**: `<ol><div>Wrong</div></ol>`
    
- **Acceptance tests**:
    
    1. Must correct invalid structure
        
    2. Final version uses only `<li>`
        
- **Do NOT use**: `<div>`, `<p>` inside lists
    

---


### [Intermediate] — 10.problem_10_reverse_and_start.html

- **Statement**: Create a list that starts from 5 and goes in reverse
    
- **Input**: none
    
- **Expected output**: 5 to 1
    
- **Constraints**: Must use `reversed` and `start`
    
- **Example**: Countdown list
    
- **Acceptance tests**:
    
    1. `<ol start="5" reversed>`
        
    2. First item is 5
        
- **Do NOT use**: CSS counters
    

---

### [Intermediate] — 11.problem_11_mixed_nesting.html

- **Statement**: Create nested ordered lists with different types (e.g., "1", "A")
    
- **Input**: none
    
- **Expected output**: Visual variation
    
- **Constraints**: Use `type` to differentiate
    
- **Example**: Topics and subtopics
    
- **Acceptance tests**:
    
    1. Outer uses one `type`, inner uses another
        
    2. Validates fully
        
- **Do NOT use**: `<ul>`
    

---

## ⚙️ 3. Debugging & Refactor Challenge

Number of fragments: 2 — Covers common misuse and semantic issues

---

### broken_fragment_1.html

```html
<ol>
  <li>Step 1
  <li>Step 2
  <div>Invalid element</div>
</ol>
```

### broken_fragment_2.html

```html
<ol type="Z">
  <li>One</li>
  <li>Two</li>
</ol>
```

---

## ✅ Final Validation Checklist

-  All exercises validate without W3C errors
    
-  All `<ol>` elements use only allowed attributes
    
-  All list items are wrapped in `<li>` tags
    
-  Semantic nesting used correctly
    
-  Accessibility preserved: proper order, screen-reader readable
    

---

## 📌 Grading rubric

- **Correctness**: 0–40 — Are the lists syntactically and semantically correct?
    
- **Semantics**: 0–30 — Are ordered lists used where sequence matters?
    
- **Accessibility**: 0–20 — Do exercises respect screen-reader compatibility?
    
- **Tests**: 0–10 — Are test assertions clear and meaningful?



---- 



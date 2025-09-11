**STAGEPROJECT:** definitions_lists_html

---

[[Project title]]  
**definitions_lists_html - Practice Pack**

---

[[1.1 Practice evey Day]]

## 📝 Description

Practice pack focused on mastering HTML definition lists: `<dl>`, `<dt>`, and `<dd>` elements with valid structure and semantic correctness.

## 🔧 Functional Requirements Implemented

-  Use of `<dl>` to enclose term-definition pairs
    
-  Proper pairing of `<dt>` and `<dd>` elements
    
-  Multiple terms to one definition
    
-  Multiple definitions per term
    
-  DOM structure validation
    
-  W3C HTML5 compliance
    

## 🌟 Stretch Goals (Optional)

-  Nested definition structures (not standard but possible in context)
    
-  ARIA labeling or semantic enhancement
    

## ⏱ Time Log

Estimated: 40–60 minutes  
Actual: TBD

## 📚 Concepts Practiced

- `<dl>` container semantics
    
- Term/definition pairing
    
- Validation rules and nesting restrictions
    
- Semantic HTML usage
    
- Machine-checkable HTML structures
    

## 📌 Notes

Solved different structural configurations of definition lists. Novelty focused on term repetition, multiple descriptions, and incorrect nesting detection. No external sources used.

---

STAGEPROJECT: definitions_lists_html

## **Stage**: definitions_lists_html

## 🎓 Learning Objectives

- Identify and implement valid `<dl>` structures with `<dt>` and `<dd>`
    
- Avoid invalid nesting or misuse of list tags
    
- Apply multiple `<dt>` or `<dd>` patterns appropriately
    
- Validate all structures through W3C compliance
    
- Ensure semantic use without visual formatting reliance
    
- Understand how assistive tech interprets definition structures
    

---

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 3 — The definition list structure is relatively narrow, and three targeted microprojects are sufficient to cover all practical permutations.

---

1. Name — single_term_definition_pair.html
    - **Files**: simple_def_list.html
    - **Input**: none
    - **Expected output / rendered result**: One term and its definition are rendered; valid semantic structure.
    - **Constraints**: Must include only one `<dt>` followed by one `<dd>
    - **Acceptance tests**:
        - DOM must contain exactly one `<dl>` with one `<dt>` and one `<dd>`
        - W3C validator should return no errors
    - **Example(s)**: Use `<dl>`, followed by one `<dt>` and one `<dd>` inside
    - **Notes**: `<html>`, `<head>`, and `<body>` used as minimal valid structure  
    - **Do NOT use**: `<ul>`, `<ol>`, `<li>`, CSS classes
        

---

2. Name — multiple_terms_sharing_one_definition.html
    
    - **Files**: multi_term_single_def.html
        
    - **Input**: none
        
    - **Expected output / rendered result**: Two or more `<dt>` elements followed by one `<dd>` element
        
    - **Constraints**: Must use one `<dd>` after at least two `<dt>`
        
    - **Acceptance tests**:
        
        - Must have at least two `<dt>` tags followed by one `<dd>`
            
        - DOM structure must be valid per HTML5
            
    - **Example(s)**: Provide multiple terms sharing one explanation
        
    - **Notes**: Wrapper tags are required for valid HTML structure
        
    - **Do NOT use**: `<ul>`, `<li>`, unnecessary inline styling
        

---

3. Name — multiple_definitions_for_one_term.html
    
    - **Files**: single_term_multi_defs.html
    - **Input**: none
    - **Expected output / rendered result**: One `<dt>` followed by two or more `<dd>`s
    - **Constraints**: Use one `<dt>` and at least two `<dd>` elements
    - **Acceptance tests**:
        - W3C validator must return no errors
        - `<dt>` must precede at least two `<dd>` elements
    - **Example(s)**: Demonstrate several descriptions for one term
    - **Notes**: HTML structure wrapped to comply with W3C
    - **Do NOT use**: Tables, `<ul>`, visual grouping tags
        

---

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 12 — [justification: The element has limited complexity; 8 basic and 4 intermediate problems are enough. Advanced use cases are rare.]

Breakdown:

- Basic: 8 (Fundamentals: structure, order, valid nesting)
    
- Intermediate: 4 (Multiple terms, multiple defs, semantic misuse detection)
    
- Advanced: 0 (not applicable — no advanced constructs for this element)
    

---

### [Basic] — 1.problem_1_term_definition_pair.html

- **Statement**: Create a valid definition list with one `<dt>` and one `<dd>`
    
- **Input**: none
    
- **Expected output**: A simple definition structure
    
- **Constraints**: Must use one `<dl>`, one `<dt>`, one `<dd>`
    
- **Example**:  
    Input: None  
    Output: `<dl><dt>...</dt><dd>...</dd></dl>`
    
- **Acceptance tests**:
    
    - Document must contain exactly 1 `<dl>`
        
    - Structure must validate without W3C errors
        
- **Do NOT use**: `<ul>`, `<li>`, placeholder tags
    

---

### [Basic] — 2.problem_2_multiple_terms.html

- **Statement**: Include two `<dt>` elements followed by one shared `<dd>
- **Input**: none
- **Expected output**: Two terms sharing one description   
- **Constraints**: Must follow proper order: `<dt>`, `<dt>`, `<dd>`
- **Example**: Provide two different terms  
- **Acceptance tests**:
    - Two `<dt>` elements must be present
    - Only one `<dd>` element must follow
- **Do NOT use**: Any repeated `<dl>` wrappers

---


### [Basic] — 3.problem_3_nesting_inside_dl.html

- **Statement**: Use valid direct children for `<dl>`
    
- **Input**: none
    
- **Expected output**: No nested `<ul>`, `<li>`, etc. inside `<dl>`
    
- **Constraints**: Only `<dt>` and `<dd>` allowed inside `<dl>`
    
- **Example**: Invalid: `<dl><ul><li>...</li></ul></dl>`
    
- **Acceptance tests**:
    
    - No non-definition tags inside `<dl>`
        
    - Valid according to W3C rules
        
- **Do NOT use**: Nested lists, inline elements inside `<dl>`
    

---



### [Basic] — 4.problem_4_proper_nesting_order.html

- **Statement**: Maintain correct `<dt>` followed by `<dd>` order
    
- **Input**: none
    
- **Expected output**: Proper term-definition flow
    
- **Constraints**: No `<dd>` before `<dt>`
    
- **Example**: `<dl><dd>...</dd><dt>...</dt></dl>` is invalid
    
- **Acceptance tests**:
    
    - Each `<dd>` must follow a `<dt>` or group of `<dt>`s
        
    - Validator must return no error
        
- **Do NOT use**: Reordered tags
    

---

### [Intermediate] — 5.problem_5_mixed_grouping.html

- **Statement**: Create a list with two terms and two definitions in proper order
    
- **Input**: none
    
- **Expected output**: `<dt>`, `<dt>`, `<dd>`, `<dd>`
    
- **Constraints**: No nesting; order must be respected
    
- **Example**: Show distinction of multiple terms and defs
    
- **Acceptance tests**:
    
    - Exactly two `<dt>`, two `<dd>`
        
    - DOM order must be valid
        
- **Do NOT use**: Visual cues to simulate semantics
    


## ⚙️ 3. Debugging & Refactor Challenge

Chosen: 2 snippets — two errors are sufficient to cover common mistakes

---

### Debug Fragment 1

**Broken code**:

```html
<dl>
  <dt>JavaScript</dd>
  <dd>A programming language.</dt>
</dl>
```

**Provide bug list and corrections after review**

---

### Debug Fragment 2

**Broken code**:

```html
<dl>
  <ul>
    <li>HTML - Markup</li>
    <li>CSS - Styling</li>
  </ul>
</dl>
```

**Provide bug list and corrections after review**

---

## ✅ Final Validation Checklist

- All exercises validate without W3C HTML5 errors
    
- Only `<dt>` and `<dd>` used within `<dl>`
    
- No improper nesting or unordered list tags
    
- Accessibility: structure parseable by screen readers
    
- Each `<dl>` includes at least one `<dt>` and `<dd>`
    

---

## 📌 Grading rubric

- **Correctness (0–40 pts)**: Valid structure, tag use, nesting rules
    
- **Semantics (0–30 pts)**: Proper use for term-definition pairing
    
- **Accessibility (0–20 pts)**: Screen reader parseability, structure
    
- **Tests (0–10 pts)**: DOM and W3C validator tests included for all
    

---
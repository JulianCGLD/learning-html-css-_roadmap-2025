[[STAGEPROJECT]] 4.2.7 quotation_html

[[Project title]]  
STAGEPROJECT - Practice Pack

[[1.1 Practice evey Day]]

## 📝 Description

Practice creating, structuring, and attributing quotations in HTML using `<q>` and `<blockquote>`.

## 🔧 Functional Requirements Implemented

-  Use `<q>` for inline quotations
    
-  Use `<blockquote>` for block-level quotations
    
-  Include `cite` attribute for source attribution
    
-  Validate HTML5 compliance for all quotation elements
    
-  Ensure semantic correctness and accessibility for quoted content
    

## 🌟 Stretch Goals (Optional)

-  Style quotations using inline attributes for demonstration
    
-  Include nested quotations combining `<q>` inside `<blockquote>`
    

## ⏱ Time Log

Estimated: 90 minutes — Actual: TBD

## 📚 Concepts Practiced

- Inline vs block-level quotation elements
    
- `cite` attribute usage
    
- Semantic HTML validation
    
- Accessibility implications of quotations
    
- DOM validation for HTML5
    

## 📌 Notes

All exercises focus exclusively on `<q>` and `<blockquote>`. Minimal `<html>` and `<body>` wrappers were included for runnable HTML structure. Resources: MDN Web Docs on `<q>` and `<blockquote>` ([https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q), [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote)).

STAGEPROJECT: 4.2.7 quotation_html

## **Stage**: 4.2.7 quotation_html

## 🎓 Learning Objectives

- Correctly implement inline and block-level quotations in HTML
    
- Apply the `cite` attribute appropriately for attribution
    
- Validate HTML5 structure for quotation elements
    
- Ensure accessibility compliance in quoted content
    
- Distinguish semantic roles between `<q>` and `<blockquote>`
    

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 4 — Chosen to cover fundamental usage of both quotation elements and `cite` attribute variations with runnable, independent exercises.

1. Inline_Quotation_Simple.html — Add a single inline quotation using `<q>`
    - **Files**: index.html
    - **Input**: a short sentence to quote
    - **Expected output / rendered result**: sentence wrapped in `<q>` with browser-rendered quotation marks
    - **Constraints**: Only `<q>` inside `<p>` allowed, must validate as HTML5
    - **Acceptance tests**:
        1. `<q>` element exists inside `<p>`
        2. W3C HTML validator reports no errors
    - **Example(s)**: Input text: "HTML is semantic." — Expected HTML: `<p>He said, <q>HTML is semantic.</q></p>`
    - **Notes**: `<p>` wrapper included to satisfy valid block content rules

2. Inline_Quotation_With_Cite.html — Add an inline quotation with a `cite` attribute
    - **Files**: index.html
    - **Input**: sentence and source URL
    - **Expected output / rendered result**: `<q>` wraps text with `cite` referencing URL
    - **Constraints**: Only `<q>` and `cite` allowed, inline within `<p>`
    - **Acceptance tests**:
        1. `<q>` element contains non-empty text and `cite` attribute 
        2. W3C validator shows no errors 
    - **Example(s)**: Input: "Practice makes perfect." URL: [https://example.com](https://example.com/) — HTML: `<p>She noted, <q cite="https://example.com">Practice makes perfect.</q></p>
    - **Notes**: Demonstrates use of `cite` attribute for attribution

3. Block_Quotation_Simple.html — Add a single block-level quotation
    - **Files**: index.html
    - **Input**: multi-sentence paragraph to quote
    - **Expected output / rendered result**: `<blockquote>` wrapping paragraph(s)
    - **Constraints**: Only `<blockquote>` allowed, may contain `<p>` inside, must validate as HTML5
    - **Acceptance tests**:
        1. `<blockquote>` exists and contains text
        2. W3C validator passes
    - **Example(s)**: Input: "Long quotation content here." — HTML: `<blockquote><p>Long quotation content here.</p></blockquote>`
    - **Notes**: `<p>` necessary inside `<blockquote>` for proper block content
 
4. Block_Quotation_With_Cite.html — Add block-level quotation with `cite` attribute
    - **Files**: index.html
    - **Input**: paragraph text and source URL
    - **Expected output / rendered result**: `<blockquote>` with `cite` referencing source
    - **Constraints**: Only `<blockquote>` with `cite`, may contain `<p>`
    - **Acceptance tests**:
        1. `<blockquote>` has `cite` attribute and non-empty content
        2. HTML5 validation passes
    - **Example(s)**: Input: Text: "HTML5 is flexible." URL: [https://example.com](https://example.com/) — HTML: `<blockquote cite="https://example.com"><p>HTML5 is flexible.</p></blockquote>`
    - **Notes**: `<p>` wrapper included for valid block content
        

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 8 — Cover both inline and block quotations with variations on `cite` and accessibility; Basic: 5, Intermediate: 3, Advanced: 0 because advanced edge cases are unnecessary to master the tag.

### [Basic] — 1.problem_1_inline_quotation.html

- **Statement**: Wrap a provided short sentence in an inline quotation.
    
- **Input**: "Learning HTML is fun."
    
- **Expected output**: `<p><q>Learning HTML is fun.</q></p>`
    
- **Constraints**: Only `<q>` inside `<p>`; no `<blockquote>`
    
- **Example**: Input: same — Expected: `<p><q>Learning HTML is fun.</q></p>`
    
- **Acceptance tests**:
    
    1. `<q>` exists with content
        
    2. HTML5 validation passes
        

### [Basic] — 2.problem_2_inline_with_cite.html

- **Statement**: Create an inline quotation with a URL in the `cite` attribute
- **Input**: "Semantic HTML improves accessibility." URL: [https://example.com](https://example.com/)
- **Expected output**: `<p><q cite="https://example.com">Semantic HTML improves accessibility.</q></p>`
- **Constraints**: Only `<q>` allowed; include `cite`
- **Example**: Input as above — Expected output: HTML snippet
- **Acceptance tests**:
    1. `cite` attribute exists and is valid
    2. HTML5 validation passes

### [Basic] — 3.problem_3_block_quotation.html

- **Statement**: Wrap multi-line paragraph in `<blockquote>`
    
- **Input**: "Block quotations can span multiple sentences."
    
- **Expected output**: `<blockquote><p>Block quotations can span multiple sentences.</p></blockquote>`
    
- **Constraints**: Only `<blockquote>` and `<p>` allowed
    
- **Example**: Input as above — Expected output snippet
    
- **Acceptance tests**:
    
    1. `<blockquote>` exists with paragraph inside
        
    2. HTML5 validator passes
        

### [Basic] — 4.problem_4_block_with_cite.html

- **Statement**: Block quotation with `cite` attribute
    
- **Input**: Text and URL: "HTML5 enhances web structure." URL: [https://example.com](https://example.com/)
    
- **Expected output**: `<blockquote cite="https://example.com"><p>HTML5 enhances web structure.</p></blockquote>`
    
- **Constraints**: Only `<blockquote>` and `<p>`; `cite` required
    
- **Example**: Input as above — Expected output snippet
    
- **Acceptance tests**:
    
    1. `<blockquote>` contains `cite`
        
    2. HTML5 validation passes
        

### [Intermediate] — 5.problem_5_nested_inline_quotation.html

- **Statement**: Place one inline quotation inside another for nested quotes
    
- **Input**: Outer: "He said", Inner: "HTML is amazing."
    
- **Expected output**: `<p>He said, <q><q>HTML is amazing.</q></q></p>`
    
- **Constraints**: Only `<q>`; nesting required
    
- **Example**: Input as above — Expected output snippet
    
- **Acceptance tests**:
    
    1. Two nested `<q>` elements present
        
    2. HTML5 validation passes
        

### [Intermediate] — 6.problem_6_block_and_inline_combined.html

- **Statement**: Place inline quotation inside a block quotation
    
- **Input**: Block: "Expert said", Inline: "Semantic HTML matters."
    
- **Expected output**: `<blockquote><p>Expert said, <q>Semantic HTML matters.</q></p></blockquote>`
    
- **Constraints**: Only `<blockquote>`, `<p>`, `<q>`
    
- **Example**: Input as above — Expected output snippet
    
- **Acceptance tests**:
    
    1. `<blockquote>` contains `<p>` and `<q>`
        
    2. HTML5 validation passes
        

### [Intermediate] — 7.problem_7_inline_accessibility.html

- **Statement**: Inline quotation with emphasis on accessibility by providing a descriptive `cite`
    
- **Input**: "Accessibility is key." URL: [https://example.com](https://example.com/)
    
- **Expected output**: `<p><q cite="https://example.com">Accessibility is key.</q></p>`
    
- **Constraints**: Only `<q>` and `cite`; emphasize semantic attribute for assistive technologies
    
- **Example**: Input as above — Expected output snippet
    
- **Acceptance tests**:
    
    1. `cite` attribute exists
        
    2. Screen reader can interpret `<q>` semantically
        

## ⚙️ 3. Debugging & Refactor Challenge

Number of broken code snippets: 2 — Enough to demonstrate typical misuse of quotation elements.

1. Broken code:
    

```
<p>He said "HTML is fun."</p>
```

- Bug list:
    
    1. Missing `<q>` element for inline quotation
        
    2. Quotation marks manually inserted instead of semantic tag
        
- Required fix:
    


2. Broken code:
    

```
<blockquote>"HTML5 improves structure."</blockquote>
```

- Bug list:
    
    1. Manual quotation marks instead of semantic usage
        
    2. Missing `<p>` inside `<blockquote>` for valid block content
        
- Required fix:
    

```
<blockquote><p>HTML5 improves structure.</p></blockquote>
```

- Refactor notes:
    
    - Use `<p>` inside `<blockquote>` for valid HTML5
        
    - Consider adding `cite` attribute for attribution
        

## ✅ Final Validation Checklist

- All exercises validate without W3C errors
    
- `<q>` and `<blockquote>` used correctly according to content type
    
- `cite` attributes present where applicable
    
- Inline quotations do not contain block-level elements
    
- Accessibility: semantic use recognized by assistive technologies
    

## 📌 Grading rubric

- Correctness 0–40: Quotation elements used properly
    
- Semantics 0–30: Correct inline/block distinction, `cite` usage
    
- Accessibility 0–20: Assistive technology compatibility, semantic correctness
    
- Tests 0–10: DOM assertions and validation checks passed

**STAGEPROJECT:** superscript_and_subscript

[[Project title]]  
superscript_and_subscript - Practice Pack

[[1.1 Practice evey Day]]

## 📝 Description

Mastery of the `<sup>` and `<sub>` elements in HTML for scientific, mathematical, and ordinal formatting.

## 🔧 Functional Requirements Implemented

-  Use of `<sup>` for superscript notation
    
-  Use of `<sub>` for subscript notation
    
-  Correct HTML5 structure and validation
    
-  Inline usage within text content
    
-  Combined use of `<sup>` and `<sub>` in a single line
    

## 🌟 Stretch Goals (Optional)

-  Dynamic switching between superscript and subscript with JavaScript
    
-  Styling variations using inline CSS
    

## ⏱ Time Log

Estimated: 40 minutes  
Actual: TBD

## 📚 Concepts Practiced

- Superscript and subscript semantics
    
- Tag placement in inline contexts
    
- HTML5 validation compliance
    
- Nested text structure
    
- Proper rendering behavior in browsers
    

## 📌 Notes

Focused exclusively on `<sup>` and `<sub>` usage. No external resources were required beyond internal model knowledge and W3C/MDN reference.

---

STAGEPROJECT: superscript_and_subscript

## **Stage**: superscript_and_subscript

## 🎓 Learning Objectives

1. Use `<sup>` to correctly render text above the baseline.
    
2. Use `<sub>` to correctly render text below the baseline.
    
3. Validate correct tag placement inside inline HTML contexts.
    
4. Combine both tags within the same sentence properly.
    
5. Ensure all usages pass W3C HTML5 validation.
    
6. Practice accessibility-friendly inline usage.
    

---

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 3 — Each project focuses on a distinct and essential application pattern: scientific notation, ordinal indicators, and combined inline usage.

1. chemical_formula_display
- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: H2O displayed inline within a sentence
- **Constraints**: Must use `<sub>` within inline paragraph context
- **Acceptance tests**:
    - Query selector `document.querySelector("sub")` must return an element with text `2`
    - W3C validator should return no errors or warnings
- **Example(s)**: Include "H2O" in a sentence.
- **Notes**: `<p>` wrapper included for valid structure

2. exponent_notation
- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: 53 should appear in a sentence as an exponent
- **Constraints**: Use `<sup>` only within paragraph
- **Acceptance tests**:
    - Query selector `document.querySelector("sup")` must return element with text `3`
    - W3C validator returns no structural or semantic errors
- **Example(s)**: "53 equals 125"
- **Notes**: Paragraph used to allow inline flow

3.scientific_sentence_combining_superscript_and_subscript
- **Files**: index.html
- **Input**: none
- **Expected output / rendered result**: A sentence containing both `<sup>` and `<sub>` correctly
- **Constraints**: Must use both elements inline in one paragraph
- **Acceptance tests**:
    - `document.querySelectorAll("sub").length === 1`
    - `document.querySelectorAll("sup").length === 1`
    - W3C validator returns no errors
- **Example(s)**: "The isotope U235 differs from U238"
- **Notes**: Inline context requires paragraph wrapper

---

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 12 — [justification: Basic usage is limited but needs extensive small variation coverage; no advanced cases needed]  
Breakdown:

- Basic: 8
    
- Intermediate: 4
    
- Advanced: 0 (not applicable due to concept simplicity)
    

---

### [Basic] — 1.problem_1_ordinal_suffix_in_text.html

- **Statement**: Add a superscript for the ordinal suffix in "21st century"
    
- **Input**: Plain text sentence
    
- **Expected output**: 21st appears inline
    
- **Constraints**: Must use only `<sup>`
    
- **Example**: Input: "We live in the 21st century"  
    Output: "We live in the 21st century"
    
- **Acceptance tests**:
    
    - `<sup>` exists and contains `st`
        
    - W3C validator returns no errors
        

### [Basic] — 2.problem_2_chemical_compound_notation.html

- **Statement**: Use subscript to render CO2 correctly
    
- **Input**: none
    
- **Expected output**: CO2
    
- **Constraints**: Use only `<sub>`
    
- **Example**: "CO2 is a greenhouse gas"
    
- **Acceptance tests**:
    
    - DOM contains `<sub>` with value `2`
        
    - No validation errors
        

### [Basic] — 3.problem_3_superscript_for_math_expression.html

- **Statement**: Use superscript to represent “x squared”
    
- **Input**: none
    
- **Expected output**: x2
    
- **Constraints**: No CSS or script
    
- **Example**: "x2 + 3x + 2 = 0"
    
- **Acceptance tests**:
    
    - DOM has `<sup>`
        
    - TextContent of `<sup>` is `2`
        

### [Basic] — 4.problem_4_multiple_subscripts.html

- **Statement**: Display H2SO4 correctly
    
- **Input**: none
    
- **Expected output**: Full formula with 2 subscript values
    
- **Constraints**: Use only `<sub>`
    
- **Example**: "H2SO4"
    
- **Acceptance tests**:
    
    - Two `<sub>` elements exist
        
    - Validation passes
        

### [Basic] — 5.problem_5_multiple_superscripts.html

- **Statement**: Render two exponents: a2 + b2
    
- **Input**: none
    
- **Expected output**: Both variables have superscripts
    
- **Constraints**: No duplication of values
    
- **Example**: "a2 + b2"
    
- **Acceptance tests**:
    
    - Two `<sup>` elements exist
        
    - No nesting issues
        

### [Basic] — 6.problem_6_isotope_mass_number.html

- **Statement**: Render the isotope as U235
    
- **Input**: none
    
- **Expected output**: Superscript mass number
    
- **Constraints**: Superscript only
    
- **Example**: "U235"
    
- **Acceptance tests**:
    
    - `<sup>` with `235`
        
    - Validation passes
        

### [Basic] — 7.problem_7_basic_time_notation.html

- **Statement**: Represent 12th hour with superscript
    
- **Input**: none
    
- **Expected output**: 12th hour
    
- **Constraints**: Only `<sup>`
    
- **Example**: "12th hour"
    
- **Acceptance tests**:
    
    - `<sup>` contains `th`
        
    - No structural issues
        

### [Basic] — 8.problem_8_subscript_element_in_equation.html

- **Statement**: Render x1 + x2
    
- **Input**: none
    
- **Expected output**: Indexed variables
    
- **Constraints**: Only `<sub>`
    
- **Example**: "x1 + x2"
    
- **Acceptance tests**:
    
    - Two `<sub>` elements
        
    - Each contains a digit
        

### [Intermediate] — 9.problem_9_combine_isotope_and_molecule.html

- **Statement**: Render U235O2
    
- **Input**: none
    
- **Expected output**: Combined super and sub inline
    
- **Constraints**: Use both tags in one word
    
- **Example**: "U235O2"
    
- **Acceptance tests**:
    
    - One `<sup>`, one `<sub>`
        
    - Proper nesting
        

### [Intermediate] — 10.problem_10_scientific_expression.html

- **Statement**: Render Na2SO4 + CaCl2
    
- **Input**: none
    
- **Expected output**: Subscripts on all numbers
    
- **Constraints**: Only `<sub>`
    
- **Example**: "Na2SO4 + CaCl2"
    
- **Acceptance tests**:
    
    - Three `<sub>` elements
        
    - All values correct
        

### [Intermediate] — 11.problem_11_superscript_for_scientific_unit.html

- **Statement**: Represent m/s2
    
- **Input**: none
    
- **Expected output**: Superscript 2 on s
    
- **Constraints**: Inline formatting
    
- **Example**: "m/s2"
    
- **Acceptance tests**:
    
    - `<sup>` with `2`
        
    - Appears within a sentence
        

### [Intermediate] — 12.problem_12_combined_math_term.html

- **Statement**: Write A12
    
- **Input**: none
    
- **Expected output**: Subscript and superscript on same base
    
- **Constraints**: Must wrap each tag separately
    
- **Example**: "A12"
    
- **Acceptance tests**:
    
    - One `<sup>`, one `<sub>`
        
    - DOM structure correct
        

---

## ⚙️ 3. Debugging & Refactor Challenge

Number of snippets: 2 — The concept has few edge cases, so two concise, flawed examples are sufficient

### Broken code 1

```html
<p>Water is represented as H<sub2>O</sub></p>
```

### Broken code 2

```html
<p>Einstein's equation: E = mc<sup>2</p>
```

---

## ✅ Final Validation Checklist

- All exercises validate without W3C errors
    
- All uses of `<sup>` and `<sub>` are semantically appropriate
    
- All exercises follow inline usage conventions
    
- No unnecessary HTML elements used
    
- Accessibility preserved in inline contexts
    

---

## 📌 Grading rubric

|Criterion|Points|Description|
|---|---|---|
|Correctness|0–40|Syntax and DOM structure correctness|
|Semantic clarity|0–30|Use of tags in appropriate contexts|
|Validation compliance|0–20|All files pass HTML5 validation|
|Testing inclusion|0–10|DOM tests and accessibility included properly|
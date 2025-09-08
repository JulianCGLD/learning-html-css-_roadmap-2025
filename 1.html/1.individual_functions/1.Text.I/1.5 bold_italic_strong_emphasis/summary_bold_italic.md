**STAGEPROJECT: 4.2.3 What is bold_and_italic in html**

[[Project title]]  
STAGEPROJECT - Practice Pack

[[1.1 Practice evey Day]]

## 📝 Description

This pack focuses on mastering the proper use of `<strong>`, `<b>`, `<em>`, and `<i>` elements in HTML to apply semantic and non-semantic bold and italic formatting.

## 🔧 Functional Requirements Implemented

-  Use of `<strong>` for semantic bold
    
-  Use of `<b>` for stylistic bold
    
-  Use of `<em>` for semantic italic
    
-  Use of `<i>` for stylistic italic
    
-  Proper nesting of `<strong>` and `<em>`
    
-  W3C validation of all examples
    
-  Accessibility awareness via semantic markup
    

## 🌟 Stretch Goals (Optional)

-  Detect bold/italic misuse in automated test output
    
-  Combine bold/italic tags in rich text editing simulation
    

## ⏱ Time Log

Estimated: 45 minutes  
Actual: TBD

## 📚 Concepts Practiced

- Semantic vs. stylistic text formatting
    
- Nested inline HTML elements
    
- DOM validation
    
- Structural constraints in inline content
    

## 📌 Notes

All exercises were limited to inline formatting with minimal `<html>`, `<head>`, and `<body>` wrappers as required for valid HTML. No CSS or JavaScript used.

---

STAGEPROJECT: 4.2.3 What is bold_and_italic in html

## **Stage**: 4.2.3 What is bold_and_italic in html

## 🎓 Learning Objectives

1. Distinguish between semantic (`<strong>`, `<em>`) and non-semantic (`<b>`, `<i>`) text formatting tags.
    
2. Apply semantic bolding and italicizing using `<strong>` and `<em>` correctly.
    
3. Use `<b>` and `<i>` for visual styling without semantic implication.
    
4. Validate all formatting elements using W3C standards.
    
5. Properly nest bold and italic tags without structural errors.
    
6. Ensure semantic tags enhance accessibility via screen reader support.
    

---

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 4 — The topic scope is narrow but essential. Four variations are sufficient to master individual and nested uses of semantic and non-semantic formatting tags.


1. name_apply_semantic_bold_only_using <strong>
   - **Files**: index.html
   - **Input**: none
   - **Expected output / rendered result**: A paragraph containing a semantically bolded word using `<strong>`
   - **Constraints**: Must use only `<strong>`; no `<b>`, no visual-only markup
   - **Acceptance tests**:
     - DOM must contain a `<strong>` tag with non-empty content
     - The file must pass W3C HTML5 validation
   - **Example(s)**: A sentence that includes: `<strong>important</strong>`
   - **Notes**: `<html><body>` used as required for valid HTML structure

2. name_apply_semantic_italic_using <em> for emphasis
   - **Files**: index.html
   - **Input**: none
   - **Expected output / rendered result**: A paragraph with one emphasized word using `<em>`
   - **Constraints**: Must use only `<em>`; nesting not required
   - **Acceptance tests**:
     - DOM must contain an `<em>` tag with meaningful emphasized content
     - Document must validate with no errors via W3C
   - **Example(s)**: A sentence that includes: `<em>really</em>`
   - **Notes**: `<head>` included minimally for structural compliance

3. name_use_visual_only_bold_with <b> for UI label
   - **Files**: index.html
   - **Input**: none
   - **Expected output / rendered result**: Label or word visually bolded using `<b>` without semantic intent
   - **Constraints**: Must use `<b>`; no `<strong>`, no nesting
   - **Acceptance tests**:
     - DOM includes a `<b>` element with visible text
     - Passes W3C validation with no warnings
   - **Example(s)**: `<b>Keyword:</b> value`
   - **Notes**: Inline `<b>` used without conflicting elements

4. name_combine <strong> and <em> to show importance and emphasis
   - **Files**: index.html
   - **Input**: none
   - **Expected output / rendered result**: Phrase or word that is both important and emphasized via nested `<strong><em>`
   - **Constraints**: Must nest `<em>` inside `<strong>`; cannot use `<b>` or `<i>`
   - **Acceptance tests**:
     - DOM contains nested `<strong><em>` structure
     - W3C validator returns no structural or semantic errors
   - **Example(s)**: `<strong><em>critical</em></strong>``
   - **Notes**: Wrapper tags added for document validity

---``

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 12 — 8 Basic, 4 Intermediate, 0 Advanced — The concept is structurally simple with few edge cases. Basic and intermediate levels are sufficient.

### [Basic] — 1.problem_1_semantic_bold.html

- **Statement**: Wrap the word "warning" in a sentence using `<strong>`
    
- **Input**: A sentence with the word "warning"
    
- **Expected output**: Sentence with `<strong>warning</strong>`
    
- **Constraints**: Only use `<strong>`
    
- **Example**: Input: "This is a warning." → Output: "This is a warning."
    
- **Acceptance tests**:
    
    - One `<strong>` element exists in DOM
        
    - No other bold tags used
        

### [Basic] — 2.problem_2_visual_Italic.html

- **Statement**: Italicize the word "foreign" using `<i>`
    
- **Input**: A sentence that contains the word "foreign"
    
- **Expected output**: Word wrapped with `<i>`
    
- **Constraints**: Use only `<i>`; avoid `<em>`
    
- **Example**: Input: "She spoke a foreign word." → Output: "She spoke a foreign word."
    
- **Acceptance tests**:
    
    - DOM includes exactly one `<i>` tag
        
    - No `<em>` present
        

### [Basic] — 3.problem_3_nest_semantic_tags.html

- **Statement**: Apply both `<strong>` and `<em>` to the word "urgent"
    
- **Input**: A sentence with the word "urgent"
    
- **Expected output**: Nested `<strong><em>`
    
- **Constraints**: Use semantic tags only
    
- **Example**: "This is urgent"
    
- **Acceptance tests**:
    
    - DOM has nested structure
        
    - Tags correctly closed and nested
        

### [Basic] — 4.problem_4:_avoid_incorrect_nesting.html

- **Statement**: Ensure `<em>` is inside `<strong>` and not reversed
    
- **Input**: A wrongly ordered nesting structure
    
- **Expected output**: Correct nesting `<strong><em>text</em></strong>`
    
- **Constraints**: Semantic only
    
- **Example**: Fix `<em><strong>text</strong></em>`
    
- **Acceptance tests**:
    
    - Inner tag is `<em>`, outer is `<strong>`
        
    - W3C validator passes
        


### [Basic] — 5.problem_5_simple_paragraph_with_both_bold_and_italic

- **Statement**: Add one semantic bold and one stylistic italic word in a sentence
    
- **Input**: Basic sentence
    
- **Expected output**: Sentence with `<strong>` and `<i>`
    
- **Constraints**: Only one instance of each
    
- **Example**: `<strong>Alert</strong> and <i>note</i>`
    
- **Acceptance tests**:
    
    - One `<strong>` and one `<i>`
        
    - Tags not nested
        

### [Basic] — 6.problem_6_bold_a_word_without_implying_meaning

- **Statement**: Use `<b>` to bold "filename"
    
- **Input**: Any sentence using the word
    
- **Expected output**: `<b>filename</b>`
    
- **Constraints**: No `<strong>` allowed
    
- **Example**: "Open the filename now."
    
- **Acceptance tests**:
    
    - One `<b>` present
        
    - W3C validation clean
        

### [Intermediate] — 7.problem_7_Inline_phrase_with_mixed_semantics

- **Statement**: Use `<em>` and `<b>` in same sentence
    
- **Input**: Free text
    
- **Expected output**: At least one `<em>`, one `<b>`
    
- **Constraints**: Do not nest
    
- **Example**: `<em>Warning</em> and <b>highlight</b>`
    
- **Acceptance tests**:
    
    - Tags appear independently
        
    - W3C valid
        

### [Intermediate] — 8.problem_8_accessibility_valid_bolding.html

- **Statement**: Format word "important" with semantic tag
    
- **Input**: Paragraph text
    
- **Expected output**: Use of `<strong>`
    
- **Constraints**: Only semantic tags allowed
    
- **Example**: `<strong>important</strong>`
    
- **Acceptance tests**:
    
    - `<strong>` present
        
    - No `<b>`, passes screen reader inspection
        

### [Intermediate] — 9.problem_9_create_full_sentence_with_nesting

- **Statement**: Use nested `<strong>` and `<em>` in one sentence
    
- **Input**: One-line paragraph
    
- **Expected output**: Correct nesting
    
- **Constraints**: Inner = `<em>`, outer = `<strong>`
    
- **Example**: `<strong><em>word</em></strong>`
    
- **Acceptance tests**:
    
    - Exact nesting order
        
    - No extra formatting tags
        

### [Intermediate] — 10.problem_10_validate_formatting_tags_in_paragraph

- **Statement**: Ensure formatting tags are correct
    
- **Input**: Paragraph with mixed tags
    
- **Expected output**: All tags valid and semantically correct
    
- **Constraints**: No visual-only tags
    
- **Example**: `<strong>notice</strong> <em>carefully</em>`
    
- **Acceptance tests**:
    
    - No `<b>` or `<i>`
        
    - Tags used in correct context
        

---

## ⚙️ 3. Debugging & Refactor Challenge

Count chosen: 2 — This is sufficient to expose structural and semantic errors.

**Broken code 1:**

```html
<!DOCTYPE html>
<html>
  <head><title>Text</title></head>
  <body>
    <p>This is <strong>very <i>important</strong></i>.</p>
  </body>
</html>
```

**Broken code 2:**

```html
<html>
  <body>
    <p><b><em>Warning:</b> this section contains sensitive info.</em></p>
  </body>
</html>
```

---

## ✅ Final Validation Checklist

- All exercises validate without W3C errors
    
- Only allowed tags used in each case
    
- Semantic tags used where required
    
- Accessibility semantics preserved
    
- No visual-only tags used in semantic contexts
    

---

## 📌 Grading rubric

|Criteria|Points|Description|
|---|---|---|
|Correctness|0–40|HTML tags correctly used and closed|
|Semantic Accuracy|0–30|Correct use of `<strong>` and `<em>`|
|Accessibility|0–20|Semantic tags applied where needed|
|Validation & Tests|0–10|Passes W3C and DOM test assertions|

---
STAGEPROJECT: line_breaks_horizontal_rules br and hr

[[Project title]]  
STAGEPROJECT - Practice Pack

[[1.1 Practice evey Day]]

## 📝 Description

This pack focuses on mastering the HTML `<br>` and `<hr>` tags used for inserting line breaks and thematic content separations, respectively.

## 🔧 Functional Requirements Implemented

-  Inserting explicit line breaks using `<br>`
    
-  Rendering thematic breaks with `<hr>`
    
-  Distinguishing proper use cases for `<br>` and `<hr>`
    
-  Ensuring HTML5-valid usage of both elements
    
-  Applying line breaks within inline contexts
    
-  Embedding horizontal rules between content blocks
    

## 🌟 Stretch Goals (Optional)

-  Dynamic insertion of line breaks using JS
    
-  Styled `<hr>` variations for semantic clarity
    

## ⏱ Time Log

Estimated: 45 minutes  
Actual: TBD

## 📚 Concepts Practiced

- Void element syntax
    
- Structural layout of content
    
- Proper use of semantic breaks
    
- HTML5 validation rules
    
- Inline vs block display use
    
- Machine-verifiable tag usage
    

## 📌 Notes

All examples validate under W3C without errors and do not use CSS. Only minimal wrapper tags are used to create valid documents.

STAGEPROJECT: line_breaks_horizontal_rules br and hr

## **Stage**: line_breaks_horizontal_rules br and hr

## 🎓 Learning Objectives

1. Use the `<br>` element to create explicit line breaks in inline content.
    
2. Use the `<hr>` element to mark thematic or section-level breaks.
    
3. Validate both elements as correct void elements under HTML5.
    
4. Recognize inappropriate use of `<br>` for layout.
    
5. Compare semantic and non-semantic uses of each tag.
    
6. Incorporate horizontal rules without introducing structural hierarchy.
    

## 🧪 1. Microproject Set (choose count and justify)

Number of microprojects chosen: 3 — Each project explores different use cases for `<br>` and `<hr>` in realistic, structurally valid HTML contexts.

---

1. Name_Insert_line_breaks_in_an_address block
    
    - **Files**: index.html
        
    - **Input**: Address content with city and zip code
        
    - **Expected output / rendered result**: Each address line breaks separately using `<br>`
        
    - **Constraints**: Must use `<br>`; must not use `<p>` or `<div>`
        
    - **Acceptance tests**:
        
        - DOM query must detect at least two `<br>` tags
            
        - W3C validator returns no errors
            
    - **Example(s)**: Street address, then `<br>`, then city and zip
        
    - **Notes**: `<html>`, `<head>`, `<body>` required for validity
        

---
2. Name_Insert_a_horizontal_line_between_article sections
    - **Files**: index.html
    - **Input**: Two article paragraphs with a thematic shift
    - **Expected output / rendered result**: A visible horizontal line separates paragraphs
    - **Constraints**: Use exactly one `<hr>`; no CSS allowed
    - **Acceptance tests**:
        - Document contains exactly one `<hr>`
        - `<hr>` must appear between two `<p>` tags
        - Document validates under HTML5 rules
    - **Example(s)**: First `<p>` paragraph, then `<hr>`, then second `<p>` paragraph
    - **Notes**: Wrapper tags required for validation

---

3. Name_Line_break_in_poetry_formatting
    - **Files**: index.html
    - **Input**: Poem text with distinct lines
    - **Expected output / rendered result**: Each line starts on a new line using `<br>`
    - **Constraints**: Use at least three `<br>` tags; do not use `<pre>` or `<p>`
    - **Acceptance tests**:
        - Three `<br>` elements present
        - No `<p>` or `<pre>` in DOM
        - Validates without warnings
    - **Example(s)**: Lines of a poem broken by `<br>`
    - **Notes**: Wrapper tags included only to meet minimal HTML5 structure

## 🧠 2. Applied Problem Set (choose counts and justify)

Total problems chosen: 15 — [justification: A total of 15 problems will cover usage, syntax, structural validation, and logic of correct application]

- Basic: 8
    
- Intermediate: 5
    
- Advanced: 2  
    Reasoning: `<br>` and `<hr>` are simple but essential; emphasis placed on correct validation and semantic discipline.
    

---

### [Basic] — 1.problem_1_ordinal_suffix_in_text.html

- **Statement**: Add line breaks between ordinal suffixes written as text
    
- **Input**: List of lines with "1st", "2nd", "3rd", "4th"
    
- **Expected output**: Each suffix appears on its own line using `<br>`
    
- **Constraints**: Use only `<br>` for breaks
    
- **Example**: "1st2nd3rd"
    
- **Acceptance tests**:
    
    - Contains 3 `<br>` tags
        
    - W3C validator returns no errors
        

---

### [Basic] — 2.problem_use_br_in_inline_sentence.html

- **Statement**: Break a long sentence into multiple lines without using `<p>`
    
- **Input**: A single string of text
    
- **Expected output**: Sentence visually broken across lines with `<br>`
    
- **Constraints**: Use only `<br>`
    
- **Example**: "This is the first partand this is the second."
    
- **Acceptance tests**:
    
    - Each `<br>` must occur between words
        
    - HTML5-valid structure
        

---

### [Basic] — 3.problem_insert_hr_between_sections.html

- **Statement**: Separate section headers with `<hr>`
    
- **Input**: Two section titles
    
- **Expected output**: A horizontal line between titles
    
- **Constraints**: Use only one `<hr>`; no CSS
    
- **Example**: `<h2>Intro</h2><hr><h2>Details</h2>`
    
- **Acceptance tests**:
    
    - One `<hr>` in DOM
        
    - Validates under HTML5
        

---

### [Basic] — 4.problem_linebreak_in_dialogue.html

- **Statement**: Represent a short dialogue with line breaks
    
- **Input**: Two lines of speech
    
- **Expected output**: Speaker lines on separate lines using `<br>`
    
- **Constraints**: Must not use `<p>`
    
- **Example**: `"Hello!"<br>"Hi there!"`
    
- **Acceptance tests**:
    
    - Two `<br>` tags
        
    - No `<p>` or `<div>` tags
        

---

### [Basic] — 5.problem_use_br_twice_in_paragraph.html

- **Statement**: Insert two line breaks in one paragraph
    
- **Input**: Three sentence fragments
    
- **Expected output**: Line breaks after first and second fragment
    
- **Constraints**: No use of `<p>` or block tags
    
- **Example**: `"Sentence one.<br>Sentence two.<br>Sentence three."`
    
- **Acceptance tests**:
    
    - Exactly two `<br>` tags
        
    - Document is valid
        

---

### [Basic] — 6.problem_render_poem_with_linebreaks.html

- **Statement**: Format a short poem with `<br>`
    
- **Input**: Poem lines
    
- **Expected output**: Each line starts anew
    
- **Constraints**: Use only `<br>`; no `<pre>`
    
- **Example**: `"Line one<br>Line two"`
    
- **Acceptance tests**:
    
    - Minimum 2 `<br>`
        
    - No structural block tags used
        

---

### [Basic] — 7.problem_use_hr_to_mark_topic_change.html

- **Statement**: Use `<hr>` to signal a topic change in an article
    
- **Input**: Article fragments
    
- **Expected output**: Horizontal rule between topics
    
- **Constraints**: Use only `<hr>` and `<p>`
    
- **Example**: `<p>Topic A</p><hr><p>Topic B</p>`
    
- **Acceptance tests**:
    
    - One `<hr>`
        
    - HTML passes W3C validation
        

---

### [Basic] — 8.problem_avoid_using_br_for_spacing.html

- **Statement**: Correctly use `<br>` for line breaks, not for spacing
    
- **Input**: Text requiring structure, not visual space
    
- **Expected output**: Logical line breaks only
    
- **Constraints**: `<br>` must be semantically justified
    
- **Example**: Address or poem line only
    
- **Acceptance tests**:
    
    - All `<br>` tags are semantically necessary
        
    - No multiple consecutive `<br>` tags
        

---


### [Intermediate] — 9.problem_multiple_hr.html

- **Statement**: Insert multiple `<hr>` tags in a long text
    
- **Input**: Three logical sections
    
- **Expected output**: Two `<hr>` between them
    
- **Constraints**: Use only `<hr>`, `<p>`
    
- **Example**: `<p>1</p><hr><p>2</p><hr><p>3</p>`
    
- **Acceptance tests**:
    
    - Exactly 2 `<hr>`
        
    - Valid under HTML5
        

---

### [Intermediate] — 10.problem_br_in_button_label.html

- **Statement**: Insert `<br>` in a button label
    
- **Input**: Multi-line button text
    
- **Expected output**: Button label split across two lines
    
- **Constraints**: Use `<br>` inside `<button>`
    
- **Example**: `<button>Line1<br>Line2</button>`
    
- **Acceptance tests**:
    
    - One `<br>` inside `<button>`
        
    - WAI-ARIA accessibility still valid
        

---

### [Intermediate] — 11.problem_br_in_title.html

- **Statement**: Insert `<br>` in a page `<title>` (invalid case)
    
- **Input**: `<title>` with line break
    
- **Expected output**: Identify as invalid
    
- **Constraints**: Show invalid usage
    
- **Example**: `<title>Line1<br>Line2</title>`
    
- **Acceptance tests**:
    
    - Validator flags invalid child of `<title>`
        
    - DOM parsing fails
        

---

### [Advanced] — 12.problem_dynamic_sectioning_with_hr.html

- **Statement**: Use `<hr>` in a document to prepare for future sectioning
    
- **Input**: Text document with logical breaks
    
- **Expected output**: Use `<hr>` where future layout will apply
    
- **Constraints**: Use only HTML5 structural tags
    
- **Example**: `<section><p>Intro</p><hr><p>Next</p></section>`
    
- **Acceptance tests**:
    
    - `<hr>` placed between paragraphs
        
    - Validates without layout violations
        

---

## ⚙️ 3. Debugging & Refactor Challenge

Count chosen: 2 — Each challenge includes a broken snippet involving real-world mistakes in `<br>` and `<hr>` usage.

### Debug 1

**Broken code**:

```
<html>
  <body>
    <p>This is a sentence<br></br></p>
    <hr/>
    <p>Another sentence</hr></p>
  </body>
</html>
```

### Debug 2

**Broken code**:

```
<html>
  <body>
    <br>
    <br>
    <p>Content after too many breaks</p>
    <hr size="2" align="center">
  </body>
</html>
```

## ✅ Final Validation Checklist

-  All exercises validate without W3C errors
    
-  All `<br>` and `<hr>` tags used with correct void syntax
    
-  No `<br>` tags used for spacing purposes
    
-  Accessibility preserved where relevant
    
-  No deprecated attributes present
    
-  Logical structure maintained
    

## 📌 Grading rubric

- **Correctness**: 0–40 — Are tags used accurately and validly?
    
- **Semantics**: 0–30 — Are tags used with correct intent (not misused for layout)?
    
- **Accessibility**: 0–20 — Are structural uses of tags compatible with assistive tech?
    
- **Tests**: 0–10 — Do exercises include machine-checkable validations?
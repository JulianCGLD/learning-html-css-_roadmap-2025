**STAGEPROJECT:** 4.5.1 img_src_alt_width_height_loading

[[Project title]]  
STAGEPROJECT - Practice Pack

[[1.1 Practice evey Day]]

## 📝 Description

Practice using the `<img>` element with its required attributes: `src`, `alt`, `width`, `height`, and `loading`, ensuring correctness, accessibility, and conformance with HTML standards.

## 🔧 Functional Requirements Implemented

-  Use of `src` for specifying image source
    
-  Inclusion of accessible `alt` text
    
-  Dimension control using `width` and `height`
    
-  Lazy and eager loading using `loading` attribute
    
-  Syntax and structure validation
    
-  Attribute presence and order checks
    

## 🌟 Stretch Goals (Optional)

-  Dynamic values for `width` and `height` using percentage (not recommended but allowed)
    
-  Test browser behavior with broken image URLs
    

## ⏱ Time Log

Estimated: 40 minutes  
Actual: TBD

## 📚 Concepts Practiced

- `img` attributes usage
    
- Required vs optional attributes
    
- Validating attribute combinations
    
- Accessibility enforcement via `alt`
    
- Performance tuning via `loading`
    

## 📌 Notes

Exercises exclude use of CSS, JavaScript, or `<figure>`. Only minimum structural HTML is included for file validity.  
References:

- [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img)
    
- [https://html.spec.whatwg.org/multipage/embedded-content.html#the-img-element](https://html.spec.whatwg.org/multipage/embedded-content.html#the-img-element)
    

---

STAGEPROJECT: 4.5.1 img_src_alt_width_height_loading

## **Stage**: 4.5.1 img_src_alt_width_height_loading

## 🎓 Learning Objectives

1. Properly define an image using `src`, `alt`, `width`, `height`, and `loading`.
    
2. Validate the structure and correctness of the `<img>` tag with all five attributes.
    
3. Apply lazy vs eager loading strategies effectively.
    
4. Detect and correct common markup errors related to the `<img>` tag.
    
5. Ensure all images pass accessibility tests using meaningful `alt` text.
    
6. Master HTML5 validation of image elements.
    

---

## 🧪 1. Microproject Set (choose count and justify)

**Number of microprojects chosen: 4 — Each project introduces distinct attribute behavior and validation scenarios to cover full mastery.**

---

1. Name — 1.all_required_img attributes_correctly.html
    
    - **Files**: index.html
    - **Input**: none
    - **Expected output / rendered result**: An image correctly displayed with given dimensions and valid attributes
    - **Constraints**: Must use `src`, `alt`, `width`, `height`, and `loading`
    - **Acceptance tests**:
        - Image must load from the given `src`
        - HTML must pass W3C validation
        - `alt` attribute must not be empty
    - **Example(s)**:
        - Provide a sample image reference and descriptive text
    - **Notes**: `<html>`, `<head>`, and `<body>` tags used for validity — no additional tags permitted

---

2. Name — 2.compare_lazy_vs_eager_image_loading.html
    - **Files**: index.html
    - **Input**: none
    - **Expected output / rendered result**: Two images, one loading immediately, the other deferred
    - **Constraints**: Only one `<img>` with `loading="lazy"`, one with `loading="eager"`
    - **Acceptance tests**:
        - Both `loading` values must be present
        - Images must have different viewport load timings
        - HTML must validate without errors
    - **Example(s)**:
        - Two `<img>` tags stacked
    - **Notes**: Visual observation confirms behavior, structure validated by DOM


3. Name — 3.enforce_aspect_ratio_with_width_and_height.html
    - **Files**: index.html
    - **Input**: none
    - **Expected output / rendered result**: Image scaled without distortion
    - **Constraints**: `width` and `height` must preserve the original aspect ratio
    - **Acceptance tests**:
        - Specified `width` and `height` must match actual image proportions
        - HTML must pass validation
    - **Example(s)**:
        - Use 600x400 image with matching attributes
    - **Notes**: Aspect ratio must be matched manually; no CSS allowed

---

4. Name — 4.Image_with_broken_src_and_fallback_alt.html
    - **Files**: index.html
    - **Input**: none
    - **Expected output / rendered result**: No image appears; only `alt` text shown
    - **Constraints**: Use non-existent image URL and meaningful alt
    - **Acceptance tests**:
        - Browser displays `alt` text
        - HTML structure valid and complete
        - `src` URL fails to load intentionally
    - **Example(s)**
        - `<img src="missing.jpg" alt="Image not found" ...>`
    - **Notes**: Testing image failure; CSS not used

## 🧠 2. Applied Problem Set (choose counts and justify)

**Total problems chosen: 14 — [justification: Broad yet contained scope allows for deep testing of attribute usage and error handling]**  
**Breakdown**: Basic: 8 | Intermediate: 6 | Advanced: 0 (not required here)

---

### [Intermediate] — 1.problem_1_lazy_loading_multiple_images.html

- **Statement**: Apply lazy loading to all images in a document.
- **Input**: HTML with 3 `<img>` elements
- **Expected output**: Each has `loading="lazy"`
- **Constraints**: No CSS or JS allowed
- **Example**: Apply change manually
- **Acceptance tests**:
    - All 3 have correct loading attribute
    - Validator shows no errors


---

## ⚙️ 3. Debugging & Refactor Challenge

**Total fragments: 2 — Enough to cover common `<img>` misuse scenarios**

---

**Broken code 1**

```html
<img source="dog.jpg" width="300" height="200">
```

---

**Broken code 2**

```html
<img src="banner.png" alt loading="lazy">
```

---

## ✅ Final Validation Checklist

- All images use `src`, `alt`, `width`, `height`, and `loading` correctly
    
- No exercises produce W3C validation errors
    
- All `alt` attributes contain non-empty descriptive text
    
- Lazy vs eager loading applied and verified
    
- No extraneous tags used
    

---

## 📌 Grading rubric

|Criteria|Points|Description|
|---|---|---|
|Correctness|0–40|Attributes used and implemented as required|
|Semantics|0–30|Meaningful `alt`, valid loading strategies|
|Accessibility|0–20|`alt` present and specific for all cases|
|Tests|0–10|All test cases pass and are structurally valid|
# Exercise 1.9 — The Page That Passes

## Part A — Audit the Frozen Page

The original ai-page.html was checked for problems that an HTML validator might not identify. The following findings are based on the HTML code and the information provided in the original prompt.

**1. Unconfirmed currency and prices**

The page lists a custom suit at $250.00 and alterations from $20.00. The prompt did not specify prices or currency. For a shop in The Gambia, the owner must confirm the actual prices and whether they should be listed in Gambian dalasi (GMD).

**2. Unverified establishment date**

The page states that the shop was established in 1985. This information was not provided in the prompt and must be confirmed by the owner.

**3. Unsupported customer count**

The page claims that the shop has more than 2,000 satisfied customers. No evidence was supplied for this claim, so it should be removed unless the owner verifies it.

**4. Unsupported award claim**

The page describes the shop as an award-winning destination for tailoring. No award was identified or provided in the prompt. The claim needs evidence or should be removed.

**5. Poor image alternative text**

The image uses alt="image". This does not meaningfully describe the image to users who rely on alternative text. The text should describe the actual image, once its contents are known.

**6. Unverified contact details**

The page provides the phone number `(555) 123-4567` and the email address `info@tailoringshop.com`. Neither detail was supplied in the prompt. The owner must provide and verify the correct contact information.

**7. Unconfirmed opening hours**

The page states that the shop opens from Monday to Friday, 9:00 AM to 5:00 PM, and closes on weekends. The prompt did not provide a schedule. The actual working week and Friday prayer arrangements must be confirmed with the owner.

**8. Unverified deposit policy**

The page states that a 50% non-refundable deposit is required for all custom orders. This business policy was not provided in the prompt and must be confirmed before publication.

**9. Headings used for appearance rather than structure**

The heading sequence is H1, H2, H2, H2, H3, H2, H2 and H2. The tagline “Quality You Can Trust!” is marked as a heading even though it functions as introductory text. Headings should describe the page's content and follow a logical outline.

**10. Fake bullet list**

The services are written inside a paragraph using bullet characters and line breaks. This is not a semantic HTML list. The services should use `<ul>` and `<li>` elements.

**11. Important warning marked only with bold formatting**

The deposit warning uses <b> to make the text bold. Bold formatting alone does not communicate the importance of a warning semantically. The warning should use <strong>.

## Part B — Compare Today's AI Output

### 1. Which defects did today's model avoid?

The output saved as ai-page-today.html improves several aspects of the original page. It uses Gambian dalasi prices, identifies Serrekunda, The Gambia, includes a proper list for services, and presents opening hours and prices in tables. It also includes a placeholder for the phone number and uses a more descriptive heading structure.

However, it still contains details that need attention. The prices, opening hours, contact information and service claims need verification. The sample prices are not confirmed business prices, and the Friday schedule does not clearly account for a prayer break. The page also includes a WhatsApp contact link that must be checked to ensure it works and points to the correct number.

### 2. What did the improved prompt change?

The improved prompt explicitly required the correct currency and location, a working-week schedule with Friday prayer arrangements marked for confirmation, logical heading structure, semantically marked important warnings, and no invented business facts.

The resulting ai-page-better.html follows these instructions more carefully. It uses semantic HTML elements, labels prices in Gambian dalasi, marks unknown business details for the owner to confirm, and leaves the Friday opening hours and prayer break unresolved rather than inventing exact times.

One remaining issue is that the image does not display in the browser because `images/shop-placeholder.jpg may not exist at the specified location. The file path must be checked, and a real image should be added if one is available.

## Part C — Improved Prompt

The following constraints were added to the improved prompt.

**Currency and location:** Specify Gambian dalasi (GMD/D) and Serrekunda, The Gambia. This reduces the risk of using the wrong currency or location. **Kind 1: Specification defect.**

**Working week and Friday prayer:** Require a realistic working-week schedule and clearly mark Friday hours and the prayer break for the owner to confirm. This reduces the risk of presenting invented opening hours as facts. **Kind 1: Specification defect.**

**Logical headings:** Require headings to follow a meaningful outline instead of being selected only for their visual size. This reduces heading-structure problems. **Kind 1: Specification defect.**

**Semantic warnings:** Require important warnings to be marked with appropriate HTML semantics, such as <strong>. This improves the meaning conveyed by the HTML. **Kind 1: Specification defect.**

**No invented business facts:** Prohibit unsupported claims and require unknown details to be clearly marked for confirmation. This reduces the risk of publishing false information about the business. **Kind 1: Specification defect.**

**Meaningful image alternative text:** Require accurate alternative text or a clearly labelled placeholder when the actual image is unavailable. This improves accessibility. **Kind 1: Specification defect.**

### Which defects survived a well-written prompt?

The broken image can remain because the referenced image file may be missing, even when the HTML contains a placeholder and descriptive alternative text. Business details such as actual prices, opening hours, contact information and available services also remain unconfirmed until the owner supplies accurate information.

### Why could no wording have prevented them?

A prompt cannot provide genuine business facts that were never supplied, so the owner must confirm those details. A prompt also cannot guarantee that an image file exists at the specified path; the file and website implementation must be checked.

## Part D — Fix the Page

The corrected page is saved as fixed-page.html. The original ai-page.html` must remain unchanged so that it continues to serve as evidence of the original AI output.

The corrected page should use semantic HTML, logical headings, a proper services list, meaningful image alternative text, Gambian dalasi, and clearly marked placeholders for unknown business details. The owner must confirm all prices, services, opening hours, Friday prayer arrangements, contact details and business claims before the page is published.

After making the corrections, open fixed-page.html in the browser and check that it displays correctly. Validate the HTML and fix any remaining errors. Then complete the AI Log, commit the exercise with the message `Complete exercise 1.9, and push the changes to the repository.
# VetDD Feedback Repository

## What is VetDD?

VetDD is a veterinary disease reference application designed for students and professionals in the veterinary field. It provides structured, section-by-section information on over 150 animal diseases — covering causes, clinical signs, gross pathology, pathophysiology, diagnosis, and more.

This repository is where members of the public can contribute feedback to improve the accuracy and depth of disease information displayed in the app.

---

## How This Repo Works

Each disease in VetDD has its own Markdown file inside the `diseases/` folder above (in this repositry). The file is named per the disease name in all lowercase, with a hyphen instead of a space, for example:

- `diseases/botulism.md`
- `diseases/foot-and-mouth-disease.md`
- `diseases/bovine-tuberculosis.md`

Each file contains the same set of sections that appear in the app. The initial content is marked as:

```
Initial: Content shown in the app is from launch
```

For uders submitting feedback, feedback lines are added **below** the initial line (or below previous feedback lines) within the relevant section.

---

## Finding the Disease You Want to Review

All disease files are stored alphabetically in the `diseases/` folder. You can:

1. Browse the `diseases/` folder in GitHub directly
2. Use GitHub's search (press `/` on the repo page) to search for a disease name
3. Clone the repo locally and search with your editor or terminal

---

## How to Submit Feedback

Follow these steps to contribute feedback on any disease section:

### Step 1 — Fork the Repo

Click the **Fork** button at the top right of this page to create your own copy of the repository.

### Step 2 — Navigate to the Disease File

In your fork, open the `diseases/` folder and find the `.md` file for the disease you want to review.

For example, to give feedback on *Rabies*, open `diseases/rabies.md`.

### Step 3 — Add Your Feedback

Under the section you want to edit, add a **new line** below the existing content. Do **not** remove or modify any existing lines.

Format your feedback as follows:

**To suggest a change:**
```
15 April 2026: Change ___ → ___ (source)
```

**To add new information:**
```
15 April 2026: Add ___ (source)
```

**Example:**
```markdown
### Clinical Signs
Initial: Content shown in the app is initial content from launch
15 April 2026: Add dysphagia and ascending paralysis in cattle cases (Acha & Szyfres, Zoonoses, 3rd ed.)
16 April 2026: Change "salivation" → "hypersalivation with inability to swallow" (Source as a link)
```

### Step 4 — Submit a Pull Request

Once you have made your changes:

1. Commit your changes with a clear message indicating the diseaes where edits were suggested and the sections in that disease to which an edit was suggested.
    For example: `"Rabies – Clinical Signs"`. 
    If you have made suggestions to multiple diseases, in your message, use a new line per (disease & section) to ensure clarity. Example:
    `"Rabies - Clinical Signs"`
    `"Rabies - Pathophysiology"`
    Be sure to copy this message's text as we will need it again in step 6 below.
2. Push the commit to your fork
3. Navigate back to the **original** `anon2348/vetdd-feedback` repository
4. Click **New Pull Request** and select your fork as the source branch
5. Provide a brief description of your changes in the PR description (You can simply paste the same content from step 1 above)
6. Submit the Pull Request

A maintainer will review your feedback, verify sources, and merge acceptable changes.
To ensure you suggestion is rapidly and promptly accepted, it is advisable to ensure the sources are provided as links. 
In the end-deployment to the app, should a change be accepted, the source for that change will be cited as per an academic standard appropriate to the UI of the app and, the source added to the "Relevant Acadamic Journal/Article" section of the app.

---

## Rules for Contributors

| Rule | Detail |
|------|--------|
| **Never remove previous lines** | All previous feedback lines must be preserved, even if you disagree with the feedback. Only add new lines below existing ones. |
| **Always date your line** | Use the format `DD Month YYYY:` at the start of every feedback line (e.g. `15 April 2026:`). |
| **Always include a source** | Every feedback line must reference a credible source in parentheses at the end — e.g. a textbook, journal article, or official guideline. Links are preferred to expedite verifiability. |
| **Be specific in each feedback point** | Use `Change ___ → ___` for corrections and `Add ___` for new information. Avoid vague comments. |
| **Be specific in in the commit message and pull request message** | The commit message helps act as a traceability point for the suggestion being made whilst the pull request message helps the maintainer of the app promptly review your suggestions. |

---

## What Happens After Your Feedback is Accepted?

When a Pull Request is reviewed and merged by a maintainer:

1. The feedback line is committed to the disease file in this repository - publicly verifiable.
2. The accepted content is transposed into the VetDD app - privcately conducted, results are public.
3. The app reflects the updated information.

Your contribution directly improves what veterinary students and professionals see in the app and we thank you for your contribution.

---

# VetDD Feedback Repository

## What is VetDD?

VetDD is a veterinary disease reference application designed for students and professionals in the veterinary field. It provides structured, section-by-section information on over 150 animal diseases — covering causes, clinical signs, gross pathology, pathophysiology, diagnosis, and more.

This repository is where the veterinary community can contribute peer-reviewed feedback to improve the accuracy and depth of disease information displayed in the app.

---

## How This Repo Works

Each disease in VetDD has its own Markdown file inside the `diseases/` folder. The file is named after the disease (lowercase, hyphen-separated), for example:

- `diseases/botulism.md`
- `diseases/foot-and-mouth-disease.md`
- `diseases/bovine-tuberculosis.md`

Each file contains the same set of sections that appear in the app. The initial content is marked as:

```
Initial: Content shown in the app is initial content from launch
```

Feedback lines are added **below** the initial line (or below previous feedback lines) within the relevant section.

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
16 April 2026: Change "salivation" → "hypersalivation with inability to swallow" (OIE Technical Disease Card – Rabies)
```

### Step 4 — Submit a Pull Request

Once you have made your changes:

1. Commit your changes with a clear message, e.g. `"Feedback: Rabies – Clinical Signs update"`
2. Push the commit to your fork
3. Navigate back to the **original** `anon2348/vetdd-feedback` repository
4. Click **New Pull Request** and select your fork as the source branch
5. Provide a brief description of your changes in the PR description
6. Submit the Pull Request

A maintainer will review your feedback, verify sources, and merge accepted changes.

---

## Rules for Contributors

| Rule | Detail |
|------|--------|
| **Never remove previous lines** | All feedback lines must be preserved. Only add new lines below existing ones. |
| **Always date your line** | Use the format `DD Month YYYY:` at the start of every feedback line (e.g. `15 April 2026:`). |
| **Always include a source** | Every feedback line must reference a credible source in parentheses at the end — e.g. a textbook, journal article, or official guideline. |
| **One disease per PR** | Keep each Pull Request focused on a single disease file to make review easier. |
| **Be specific** | Use `Change ___ → ___` for corrections and `Add ___` for new information. Avoid vague comments. |

---

## What Happens After Your Feedback is Accepted?

When a Pull Request is reviewed and merged by a maintainer:

1. The feedback line is committed to the disease file in this repository
2. The accepted content is transposed into the VetDD app
3. The app reflects the updated, peer-reviewed information

Your contribution directly improves what veterinary students and professionals see in the app.

---

## Questions?

If you have questions about the feedback process, open an [Issue](../../issues) in this repository.

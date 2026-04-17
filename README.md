# VetDD Feedback Repository

   > Please note there is a "navigation" button on the top right of this page's header for you to navigate to the section you wish to read.

## What is VetDD?

VetDD is a veterinary disease reference application designed for students and professionals in the veterinary field. It provides categorised, section-by-section information on over 100 animal diseases — covering causes, clinical signs, gross pathology, pathophysiology, diagnosis, and more.

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

For users submitting feedback, feedback lines are to be added **below** the initial line or below previous feedback lines within the relevant section.

### Tip for researchers & academics:

If you wish to be credited for your contributions outside the scope of VetDD, be sure to link your Github profile with ORCID. 

To do this, navigate to your [profile settings](https://github.com/settings/profile) → Scroll down to "ORCID iD" → [Connect your ORDID iD](https://github.com/settings/orcid_connection/new). 

More details on ORCID are avaialble here: https://info.orcid.org/what-is-orcid/. 

_Please note: How ORCID handles & reflects the correlation is outside the scope of our operations._

---

## Finding the Disease You Want to Review

All disease files are stored alphabetically in the `diseases/` folder. You can:

1. Browse the `diseases/` folder in GitHub directly
2. Use GitHub's search (press `/` on the repo page) to search for a disease name
3. Clone the repo locally and search with your editor or terminal

---

## How to Submit Feedback for existing diseases

Follow these steps to contribute feedback on any existing diseases:

### Step 1 — Fork the Repo

Click the **Fork** button at the top right of this page to create a copy of the repository for yourself.

If you have already created a fork of the repository, before submitting additional feedback, be sure to press "Sync fork" in your forked copy before doing the next steps. This ensure you are editing the latest version of the repo.

### Step 2 — Navigate to the Disease File

In your fork, open the `diseases/` folder and find the `.md` file for the disease you wish to provide feedback for.

For example, to give feedback on *Rabies*, open `diseases/rabies.md`.

### Step 3 — Add Your Feedback

Under the section you want to edit, add a **new line** below the existing content. Do **not** remove or modify any existing lines.

Format your feedback as follows:

**To suggest a change:**
```
Change ___ → ___ (source)
```

**To add new information:**
```
Add ___ (source)
```

**Example:**
```markdown
### Clinical Signs
Initial: Content shown in the app is initial content from launch
15 April 2026: Add dysphagia and ascending paralysis in cattle cases (Acha & Szyfres, Zoonoses, 3rd ed.)
16 April 2026: Change "salivation" → "hypersalivation with inability to swallow" (Source as a link)
```

### Step 4 — Submit the changes

Once you have made your changes to a disease page, on the page:

1. Press the green "Commit changes" button at the top right of the page section and ensure it is selected to commit the change to your fork.
2. Commit your changes with a clear message indicating the diseaes where edits were suggested and the sections in that disease to which an edit was suggested.
    
    For example: `"Rabies – Clinical Signs"`
    
    If you have made suggestions to multiple sections in one disease, in your message, use a new line per (disease & section) to ensure clarity.
    
    Example: 
    
    `"Rabies - Clinical Signs"`
    
    `"Rabies - Pathophysiology"` 
    
    Be sure to copy this message's text as it will be needed again in step 6 below.

    This is a per disease process. Please do this per disease as you suggest edits to each disease and, be sure to save your commit message per diseae to a notepad/word document to use in step 6 later.
3. Once you have committed all your suggestions to your forked repository, navigate back to the **original** [`/vetdd-feedback`](https://github.com/anon2348/vetdd-feedback) repository
4. Click **New Pull Request** and select your fork as the source branch
5. Provide a brief description of your changes in the PR description (You can simply paste the same content from step 1 above)
6. Submit the Pull Request

A maintainer will review your feedback, verify sources, and merge changes.
To ensure your suggestion is promptly accepted, it is advisable to provide the sources are as a publicly accesible link.
In the end-deployment to the app, should a change be accepted, the source for that change will be cited as per an academic standard appropriate to the UI of the app and, the source will be added to the "Relevant Acadamic Journal/Article" section of the app.

---
## How to add new diseases

If there is a disease that is not included in the `/diseases/` folder, please follow these steps to add it.

### Step 1 - Fork the repo
   _same as above_

Click the **Fork** button at the top right of this page to create a copy of the repository for yourself.

If you have already created a fork of the repository, before submitting additional feedback, be sure to press "Sync fork" in your forked copy before doing the next steps. This ensure you are editing the latest version of the repo.

### Step 2 - Copy the template

Navigate to the page [`/template.md`](https://github.com/anon2348/vetdd-feedback/blob/main/template.md) and copy the format of the template

### Step 3 - Create a new page in the main folder

   - In the `/diseases`folder, create a new page
   - Label this page with the format `[disease].md`
   - Paste the template text you just copied into the page section
   - Edit each section in the page as specified
   
### Step 4 - Submit the changes
   _similar to above_

   1. Press the green "Commit changes" button on the top right of the new disease page entry created. There is no need to detail each section where information has been added, simply type `New Disaese added: [Disease name]` as the commit message.

      This is a per-page commit so, if you have multiple diseases to add, create all the new disease entries you wish to have uploaded by repeating **Step 2** and **Step 3** above for each disease.
      
   2. Push the commit to your fork
   3. Navigate back to the **original** [`/vetdd-feedback`](https://github.com/anon2348/vetdd-feedback) repository
   4. Click **New Pull Request** and select your fork as the source branch
   5. Detail what the new disaese added is in the Pull Request message. This can be the same as the `New Disaese added: [Disease name]` from above.
   6. Submit the Pull Request

A maintainer will review your addition, verify sources, and merge changes.
To ensure your suggestion is promptly accepted, it is advisable to provide the sources are as a publicly accesible link.
In the end-deployment to the app, should a change be accepted, the source for that change will be cited as per an academic standard appropriate to the UI of the app and, the source will be added to the "Relevant Acadamic Journal/Article" section of the app.

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

# VetDD Feedback Repository

   > Please note there is a "navigation" button on the top right of this page's header for you to navigate to the section you wish to read.

## What is VetDD?

VetDD is a veterinary disease reference application designed for students and professionals in the veterinary field. It provides categorised, section-by-section information on over 100 animal diseases — covering causes, clinical signs, gross pathology, pathophysiology, diagnosis, and more.

This repository is where members of the public can contribute feedback to improve the accuracy and depth of disease information displayed in the app.


## How This Repo Works

Each disease in VetDD has its own file inside the `diseases` folder above. The file is named per the disease name in all lowercase, with a hyphen instead of a space, for example:

- `diseases/botulism.md`
- `diseases/foot-and-mouth-disease.md`
- `diseases/bovine-tuberculosis.md`

Each file contains the same set of sections that appear in the app. The initial content is marked as:

```
Initial: Content shown in the app is from launch
```

For members wishing to feedback;
   1. Please check the feedback backlog that is still pending implementation before submitting anything. You can find this by navigating to the "Pull requests" tab above (or click [here](https://github.com/anon2348/vetdd-feedback/pulls)).

      - If there is a pull request made on the same disease you wished to provide feedback for, please wait until that feedback has been implemented, and only after, submit your feedback.
      - If there are pull requests in the backlog queue but, it is not on the disease(s) you wished to provide feedback on, you don't need to wait. You can go ahead and submit your feedback.
     
   2. Please read the two sections below namely [How to submit feedback for existing diseases](https://github.com/anon2348/vetdd-feedback/pulls) and [How to add new diseases](https://github.com/anon2348/vetdd-feedback/pulls) before attempting to submit feedback
   3. Familiarise yourself with the [Rules for contributors](https://github.com/anon2348/vetdd-feedback/pulls) section


### Tip for researchers & academics:

If you wish to be credited for your contributions outside the scope of VetDD, be sure to link your Github profile with ORCID. 

To do this, navigate to your [profile settings](https://github.com/settings/profile) → Scroll down to "ORCID iD" → [Connect your ORCID iD](https://github.com/settings/orcid_connection/new). 

More details on ORCID are avaialble here: https://info.orcid.org/what-is-orcid/. 

_Please note: How ORCID handles & reflects the correlation is outside the scope of our operations._


---


## How to submit feedback for existing diseases

Follow these steps to contribute feedback on any existing diseases:

### Step 1 — Navigate to the Disease File

In the `diseases` folder above, find the file for the disease you wish to provide feedback for.

For example, to give feedback on *Rabies*, open `diseases/rabies.md`.

### Step 2 — Add Your Feedback

First, press the pencil icon in the top right section of the header.

Under the section you want to edit, **add a new line** *below* the existing content. Do **not** remove or modify any existing lines. This is very important!

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
15 April 2026: Add ascending paralysis in cattle cases (Acha & Szyfres, Zoonoses, 3rd ed.)
16 April 2026: Change "salivation" → "hypersalivation with inability to swallow" (Source as a link)
```

Note: Citing a publicly accesibly link for the source in this feedback process is highly suggested and preferred. Citing as per academic standards will slow down the verification & implementation process. 

When physical books/private journals are used as a source, we would appreciate a redirect to the book's/private journal article's listing/summative page and a page number so we can attempt to source the book/journal article and verify the feedback.

### Step 3 — Submit the changes

Once you have made your changes to a disease page, on the page:

1. Press the `Propose changes` button.
2. In the message box, clearly indicate the sections under the diseas where edits were suggested.
    
    For example: `"Rabies – Clinical Signs"`
    
    If you have made suggestions to multiple sections in one disease, in your message, use a new line per (disease & section) to ensure clarity.
    
    Example: 
    
    `"Rabies - Clinical Signs"`
    
    `"Rabies - Pathophysiology"` 

3. Once you have listed all your edits, submit the form and press the `Create pull request` button that appears in the next popout. The message field should populate with the same information you just wrote out.

A maintainer will review your feedback, verify sources, and accept or reject the feedback.

To ensure your suggestion is promptly accepted, it is advisable to provide the sources as a publicly accesible link.

In the end-deployment to the app, should a change be accepted, the source for that change will be cited as per an academic standard appropriate to the UI of the app. The source will be added to the "Relevant Acadamic Journal/Article" section of the app.

You will receive a notification in Github about the status of your feedback.


---


## How to add new diseases

If there is a disease that is not included in the `diseases` folder, please follow these steps to add it.

### Step 1 - Copy the template

Navigate to the page [`template.md`](https://github.com/anon2348/vetdd-feedback/blob/main/template.md) and copy the format of the template (press the copy button in the header).

### Step 2 - Create a new page in the main folder

   - Navigate to the [`diseases` folder](https://github.com/anon2348/vetdd-feedback/tree/main/diseases) and click "Add file" → "Create New File"
   - Label this page (at the top) with the ending `[disease].md`
       - Ensure you only use lowercase and use a hypen "-" instead of spaces
       - Ensure you add `.md` to the end of your file name
   - Paste the template text you just copied into the page section
   - Edit each section in the page as specified
   
### Step 3 - Submit the changes

Once you have made your changes to the new disease page:

1. Press the `Commit changes` button
2. There is no need to detail each section where information has been added, simply type `New Disaese added: [disease name]` as the commit message. Submit this form.
3. Press the `Create pull request` button that appears in the next popout

A maintainer will review your feedback, verify sources, and accept or reject changes.

To ensure your suggestion is promptly accepted, it is advisable to provide the sources are as a publicly accesible link.

In the end-deployment to the app, should a change be accepted, the source for that change will be cited as per an academic standard appropriate to the UI of the app. The source will be added to the "Relevant Acadamic Journal/Article" section of the app.

You will receive a notification in Github about the status of your suggestion.


---


## Rules for Contributors

| Rule | Detail |
|------|--------|
| **Review ongoing feedback first** | Before creating a feedback submission, navigate to the "Pull requests" tab above to view ongoing feedback. Do not submit feedback for a disesae that may have a feedback backlog item pending review. |
| **Never remove previous lines** | All previous feedback lines must be preserved. Only add new lines below existing ones. |
| **Always date your line** | Use the format `DD Month YYYY:` at the start of every feedback line (e.g. `15 April 2026:`). |
| **Always include a source** | Every feedback line must reference a credible source in parentheses at the end — e.g. a textbook, journal article, or official guideline. Links are preferred to expedite verifiability. |
| **Be specific in each feedback point** | Use `Change ___ → ___` for corrections and `Add ___` for new information. Avoid vague comments/long sentences. |
| **Be specific in in the form message** | The commit message helps act as a traceability point for the suggestion being made whilst the pull request message helps the maintainer of the app promptly review your suggestions. Please do add both. |


Your contribution directly improves what veterinary students and professionals see in the app and we thank you for your contribution.


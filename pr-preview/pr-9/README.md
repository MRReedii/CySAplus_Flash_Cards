# 🛡 CySA+ Flashcards

A lightweight, browser-based flashcard deck for CompTIA CySA+ study — built by students, for students.

---

### How This Started

We're in the middle of a three-month cybersecurity program with about 30 people, working toward CySA+ and Splunk certifications while balancing real work.

Somewhere along the way, people started making digital flashcard sets — PDFs, question banks, the usual.

One of the students in our Standup group shared a solid PDF set. I turned those questions into this web page so we could study them more easily.

Now the two of us are collaborating to turn this into a small hub where members of the cohort can share and study from each other's question sets.

### What This Is Right Now

* Clean, interactive flashcard interface
* Flip cards
* Keyboard navigation
* Question shuffling
* CySA+ practice questions
* Topics covering:

  * Network Security
  * Vulnerability Management
  * Incident Response
  * Threat Intelligence
  * Security Operations
  * And more
* Hosted on GitHub Pages for easy access

### 📚 Open the Flashcards

Visit the live application:
**[CySA+ Study Hub](https://mrreedii.github.io/CySAplus_Flash_Cards/)**


### Where We're Headed

* Pull in more question sets from other students in the class
* Create a shared space for cohort study materials
* Password-protect some decks while leaving others public
* Keep the platform simple and useful

This is an independent side project between the two students who started it.

**No official affiliation — just students helping each other get through the material.**


### 🌐 Custom Data Sources

### Hidden Feature

You can load external, decentralized, or remote question sets directly into the application without modifying the codebase.

### How to Access

1. **Triple-click (3x)** the **User Profile Pill** in the top-left corner of the application.
2. A prompt will appear asking for either:

   * A **Public Data CID**, or
   * A **Direct JSON URL**
3. Enter a valid CID or URL.
4. The application will fetch the payload and dynamically load the question set into the available decks.
5. Submitting an empty input clears custom-loaded sets and resets the application to the default question banks.


### 🛠 Feature Flags & Developer Controls

Unfinished and experimental features are isolated behind feature flags to keep the production view clean while allowing active development.

### How to View the Developer Control Panel

1. Click the main **🛡 CYSA+ STUDY HUB** title/logo **5 times in rapid succession**.
2. A hidden developer header (`dev-header`) will toggle at the top of the application.
3. Individual features can then be enabled or disabled in real time.

### Active Feature Flags

| Flag                       | Description                                                      |
| -------------------------- | ---------------------------------------------------------------- |
| `SHOW_ALL_DEV_FEATURES`    | Overrides and enables all hidden UI components simultaneously.   |
| `ENABLE_AUTH`              | Toggles the login and user authentication portal view.           |
| `ENABLE_APPLE_AUTH`        | Shows the Apple OAuth login option.                              |
| `ENABLE_MS_AUTH`           | Shows the Microsoft OAuth login option.                          |
| `ENABLE_PROGRESS_TRACKING` | Displays progress tracking and community activity panels.        |
| `ENABLE_TOPIC_BROWSING`    | Displays domain/topic quick-select category cards.               |
| `ENABLE_STUDY_MATERIALS`   | Opens the tabbed study materials and reference guides workspace. |

### How to Add or Remove Feature Flags

#### 1. Define the Flag

Add or remove the key-value pair in the `FEATURE_FLAGS` object inside `index.html`:

```javascript
const FEATURE_FLAGS = {
  ENABLE_NEW_FEATURE: false
};
```

#### 2. Add the Developer Control

Add a corresponding `<select>` control inside the `#devHeader` element so the feature can be controlled from the developer bar.

#### 3. Bind Feature Visibility

Apply the `feature-in-dev` CSS class along with your specific feature tag (for example, `feature-new`) to any HTML element that should be conditionally hidden or revealed.
The feature visibility is then handled through `applyFeatureFlags()`.

---

**Open the flashcards:** just visit the [GitHub Pages link](https://mrreedii.github.io/CySAplus_Flash_Cards/) for this repo.

Study hard. Share what works. Lift each other up.  
We're all trying to pass the same exams.  
Let's make the path a little clearer for the people next to us.

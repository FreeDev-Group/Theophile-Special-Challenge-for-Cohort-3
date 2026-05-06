# TEST NOTES (Live Testing)

While I was testing the surveys on the site, most things matched up with the use case diagram, but in comparison to the use case diagram, it is mentioned that the process of answering questions will be automatically saved, but unfortunately, when I lost my connection, everything was erased. 
I noticed that this does not follow the logic of the use case diagram.

---

## What I am testing

### All surveys

To access the survey menu, I first log in to my account and am directed to the 'surveys' tab, where I found all the surveys available on the site.
![All surveys](./Images/All%20surveys.png)

### Responding to questions

I selected a survey at random and began entering my responses. So far, everything is functioning as expected; the multiple choice is correct according to the 'Provide Survey' use case, and this image bellow is the palpable proof that answers this question.
![Responding to questions](./Images/Responding%20to%20questions.png)

### Confirmation message of submission

After confirming my answers, I clicked the 'submit' button and my responses were successfully recorded.
![Confirmation message](./Images/Confirmation%20message%20of%20submission.png)

### Missing one response

Exactly as shown in the use case diagram, I intentionally left a field blank while filling out the responses, and it’s working exactly as expected. 
The response wasn't saved in 'completed surveys'; instead, it stayed there, waiting for the empty field to be filled.
![Missing response](./Images/Missing%20one%20response.png)

### Completed surveys

To bridge the gap between the use case theory and the live site, I checked the 'completed surveys' section to validate the data entry. 
I found that every submitted survey is accurately listed, which is consistent with the intended design.
![Completed survey](./Images/Completed%20survey.png )

### Survey reference

Although not specified in the use case diagram, providing the user with clear navigation context is vital. Keeping a fixed header and clearly indicating the active tab status is crucial for user orientation.
![Survey reference](./Images/Survey%20reference.png)

---

## What I did (steps)

1. I logged into my account and navigated to the 'Surveys' tab.
2. I selected a survey and began answering the questions.
3. While filling out the survey, I lost my internet connection.
4. I noticed that all of my responses were erased and not automatically saved.
5. I checked the 'completed surveys' section to validate the data entry.
6. Finally, I navigated to the 'Student' tab and noticed that clicking on 'Profile' triggers no action. 

---

## What I noticed (IMPORTANT)

- When my connection dropped, all the survey answers I had filled in were erased.
- The use case diagram explicitly states that the process of answering questions will be automatically saved, but this is not happening. Additionally, regarding the 'Student' tab and its two sub-sections: currently, clicking on 'Profile' triggers no action. I suggest that this section at least displays the logged-in user's information and allows for profile navigation. 
For instance, if two people are sharing the same machine, it is currently impossible to identify who is logged in.

---

## What should have happened

Based on the use case:

- The system should automatically save my responses as a draft while I am answering the questions.
- Upon losing connection, my progress should remain intact so I can resume when reconnected.

---

## Is this a problem?

If YES, I describe it clearly:

- **Short description:**
  Survey progress is completely lost if the internet connection drops, despite the use case specifying automatic saves.

- **Why this is a problem:**
  It contradicts the expected behavior in the use case diagram and results in a poor user experience, forcing users to restart the survey from scratch.

- **Type:** Bug / UX

- **Severity (my opinion):** High

---

## Special note (VERY IMPORTANT)

I explicitly note:

- The lack of an auto-save feature is a direct deviation from the expected behavior in the use case.
- On a positive note, providing a fixed header indicating the active tab status (Survey reference) is very helpful for navigation, though not explicitly mentioned in the use case diagram.

---

## Evidence

- I have attached screenshots of the normal flow above. The main evidence for the bug is that returning to the survey after losing connection shows it completely empty.

---

## My thoughts / questions

- Why isn't local storage or a similar mechanism being used to temporarily save the draft state of the survey?
- Can we implement a visual indicator (like "Saving..." or "Saved as draft") so the user knows when their progress is actually saved?

---

## Action taken

- I added the "bug" and "high priority" labels.


---

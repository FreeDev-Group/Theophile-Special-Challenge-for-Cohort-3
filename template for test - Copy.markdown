
## What I am testing

### Register as a student

This screenshot serves as proof of my student registration. I'll start the registration process, and I'll address the remaining details in the work that follows.
![](./Images/Register%20as%20a%20student.png)

### Mail confirmation

After completing my registration on the site as a student, I received this confirmation email in my inbox. According to the logic of the use-case diagram, everything is clear and precise up to this point.
![](./Images/Mail%20confirmation.png)

### Changine my password

By confirming my email address, I was able to access the student dashboard on the site, and so far, everything is functioning as expected according to the student use-case diagram.
![](./Images/Changine%20my%20password.png)

### Confirmation email of changing password

In the process of initiating a password change, the system obliges me to provide my email address as a means of verifying that the request genuinely originates from me.![](./Images/Confirmation%20email%20of%20changing%20password.png)

### WEAK Password

When attempting to change my password to one of my own preference, the system refused to save it, claiming it was too weak. On this point, I believe that the choice of password should remain a personal decision. In particular, students often prefer something simple rather than overly complex, and such flexibility could help reduce the frequent reliance on the 'forgot password' option. ![](./Images/WEAK%20Passwork.png)

### Strong Password

After adding characters and other symbols to the password, I was finally able to change it and move on to the next step. However, this requirement is personally difficult for me, and perhaps for some students as well, because forgetting even a single symbol would force us to repeatedly reset the password.
![](./Images/Strong%20password.png)

 ### DASHBOARD

After attempting to change the password, this step went smoothly, and in the end, I was able to access the student dashboard.
 ![](./Images/DASHBOARD.png)

### Creating an account with an existing email

create account with a valid email and password works fine. But creat account with an existing credantials did not work as expected, because it should not allow the creation of an account with the credentials of an already existing account.
![](./Images/Existing%20email.png)


## What I did (steps)

After receiving the repository from my mentor, I proceeded to the site where I created a student account using my personal details. I entered an email address, and subsequently, a confirmation password was sent to me. At first, I used the default password before changing it to another one. This was unexpected on my part, as I initially believed that each user had the freedom to create a password of their own choice. However, I discovered that this was not possible, so I followed the system’s recommendation and successfully created a new password. Afterwards, I accessed the homepage and scrolled through the displayed menus, which allowed me to take the screenshot that I mentioned earlier in my report regarding the tabs."

Here is the clear sequence:

1. Receiving the repository.

2. Creating the account.

3. Email confirmation and default password.

4. Password change process.

5. Accessing the homepage.

6. Navigating menus and capturing a screenshot.

## What I noticed (IMPORTANT)

### Testing the App

During my testing of the application, I discovered that when navigating through the site’s tabs, a student can easily become disoriented because **it is not immediately clear which menu they are in**. In my view, it would be prudent to fix the interface so that the active tab is clearly highlighted, thereby helping students to maintain orientation while navigating.
Moreover, incorporating a **return button directly into the application interface is essential**, as it provides a more reliable navigation option than depending exclusively on the browser’s back function.

I think it's also very important to keep the site’s header fixed at the top of the page.
![](./Images/Testing%20the%20App.png)

### Footer case

The footer is not properly positioned, which may make it somewhat difficult for a student to understand the layout. Therefore, it is crucial to place it correctly in order to maintain the site’s visual appeal and ensure better usability.

Moreover, as this message appears on the screen, it is **impossible to determine from which tab it originates**. Therefore, it is essential to highlight the **active tab** clearly so that students can easily identify their current location within the site.
![](./Images/Footer%20case.png)

### setting 

As with most websites and other online platforms, a user’s profile picture is very important, as it can serve as an access point to several functions such as profile settings, account preferences, logout, and other user-related options. However, in this case, such a feature does not exist. I believe this is a matter of choice, either to implement it or to leave it aside.
![](./Images/Setting%20button.png)
---

## What should have happened

1. **Visual Feedback:** The navigation menu should clearly highlight the **active tab** so the student always knows their location within the app.
2. **Navigation Ease:** A dedicated **"Return" or "Back" button** should be integrated into the UI to provide a seamless navigation experience without relying solely on the browser.
3. **Layout Integrity:** The **header should remain fixed** for constant access to menus, and the **footer should be pinned** to the bottom of the page to maintain a professional layout.
4. **Account Management:** Clicking the profile area should ideally open a **settings/profile menu** for better user control.

---

## Is this a problem?

Yes, it is a significant problem because it affects both functionality and user trust. Specifically, the system fails to prevent duplicate accounts, while the lack of navigation feedback and inconsistent layout makes the application difficult for students to use effectively. These issues combined create a confusing experience that deviates from professional standards.

- **Why this is a problem:**

The lack of navigational cues (active tabs, return buttons) significantly degrades the user experience, making the app feel unfinished and difficult for students to trust.
---

## Special note (VERY IMPORTANT)

1. Essential navigation elements like active tab indicators and internal return buttons are completely missing from the UI.
2. The absence of a profile settings menu limits user control and deviates from standard student application patterns.

---

## Evidence

- I add screenshots when needed
- I make sure the issue is visible in context

---

## My thoughts / questions

- **What confused me:** I was initially disoriented when navigating because the active tabs aren't highlighted.
- **What I don’t understand:** Why the password requirements are so strict for a student app?
- **Ideas for improvement:**
  1. Fix the header and footer positions to ensure a consistent and professional UI layout.
  2. Implement a dedicated "Return" button within the app so students don't have to rely on the browser's back button.
  3. Add a profile/settings menu triggered by the user's profile picture for better account accessibility.

---

## Action taken

- Documented all navigation and layout issues and captured visual evidence for the development team.
- Submitted these suggestions for UX improvements to enhance overall student orientation and usability.

---

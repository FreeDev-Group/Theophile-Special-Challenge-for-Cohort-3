Sub-Use Case: Managing question type.
=================================
**Actors** : Instructor

## Adding questions to the Survey

During testing of the question component, I successfully saved my questions without any issues, fully aligning with the instructor's requirements as outlined in the use case.

![](./Images/Adding%20questions%20to%20the%20Survey.png)

## Updating survey

As outlined in the use case, the question update functionality operates flawlessly within the system framework. This feature provides instructors with the necessary flexibility to seamlessly revise erroneous inputs or dynamically update question content to maintain the relevance and accuracy of their assessments. By ensuring real-time modifications can be executed without disrupting the overall structure of the survey, the platform effectively minimizes administrative overhead and optimizes content management workflows.

Furthermore, this robust capability directly aligns with key user expectations by offering an intuitive yet powerful mechanism for ongoing content refinement. Instructors can confidently adapt their surveys to evolving educational requirements, ensuring that data collection remains both precise and purposeful. Ultimately, the seamless execution of this functionality reinforces the system's reliability as a professional-grade tool tailored for efficient academic administration.

![](./Images/Updating%20survey.png)

## Associating survey

The survey association functionality executes flawlessly, precisely routing each question to its designated survey to ensure seamless data alignment. This robust linking mechanism is critical to maintaining system-wide architecture; by preventing the misallocation of questions, it protects data integrity and guarantees that the specialized survey structures created by other authors remain entirely undisturbed.

![](./Images/Associating%20to%20survey.png)

## Question type

The question type feature delivers total control over response formatting, allowing us to effortlessly define parameters for multiple choice, phone number, email inputs, and beyond. This functionality operates flawlessly under all conditions, executing with zero friction and proving that the system is fully optimized to handle diverse data validation requirements without a single misstep.

![](./Images/Question%20type.png)

## From student

After completing the question, there is no need to revisit it. However, a scenario may arise where the instructor updates a survey that a student has already submitted; unfortunately, this could penalize the student, as they will no longer have the option to return to it.

![](./Images/From%20student.png)

## Schedule a question

I scheduled a question, and it works well. However, the remaining issue is the one I raised in the previous section: it would be better to allow students to update the questions they have already submitted once the survey is updated. Right now, it's completely impossible to access it again. Once they answer a question, there is no way for them to go back to it.

![](./Images/Schedule%20a%20question.png)

## Other question tested

I have completed comprehensive testing on all question formats across the platform. Every functional element is operating precisely as intended, with no deviations or performance issues detected during the evaluation.

This successful outcome represents a significant milestone, particularly when measured against the initial benchmarks established by the design engineering team. The seamless functionality achieved not only validates the system architecture but also exceeds the baseline technical expectations set for this phase of development.

![](./Images/Questions%20tested.png)

## Conclusion

The question management workflow is stable and meets the instructor's needs. The system correctly handles adding questions, updating survey content, linking questions to the correct surveys, and enforcing the configured question types.

The primary recommendation is to improve the student experience when a survey is changed after submission. Implementing a way for students to revisit or reconcile affected responses would make the workflow fairer and prevent lost access after a survey update.

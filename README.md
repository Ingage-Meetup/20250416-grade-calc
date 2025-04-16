# Grade Calculator

## Constraints

1. Please use Test Driven Development practices to develop the code
1. Please try to know your next commit

   - Think about the next smallest increment to adding functionality and supporting tests to your application
   - Confirm that previous tests run and that there are no regressions on previous work
   - Commit your code to your local git repository every time you make any small forward progress
   - Give you commit a descriptive message

1. Keep your code in working order for all previous features / tests
1. Please try to keep you code clean

   - Try not to leave commented out code in case you need it.
   - If you run into a situation where you think you need that older code either find it in source control, or revert your code to the last commit (or stash the code) and rewrite your code for the "next commit".

## The Backstory

Your assignment, should you accept it is to create a system to support our schools, teachers, and children to evaluate the students process toward matriculation. Unfortunately due to recent budget cuts we had to terminate our contract with our school management system, and we have a dire need to be able to calculate students grades.

## Requirements

At a bare minimum we need a working system that can calculate students grades. We should be able to display both numeric grades (0 to 4.0) and alphabetic grades (A, B, C, D, F). Regardless of other features in the system we need at least this much to work, but would like additional features incorporated as you have time and budget.

For this initial request each students grade will be based on a number of equally weighted tests in the range of 0 to 100 points for each tests. Each teacher will determine frequency and number of equally weighted tests for each of their classes.

### Alphabetic Grades

    A - 90.0% to 100%
    B - 80.0% up to 90.0%
    C - 70.0% up to 80%
    D - 60.0% up to 70%
    F - 0.0% up to 60%

### Numeric GPA

| Percentage | GPA |
| ---------- | --- |
| 97-100%    | 4.0 |
| 93–96%     | 3.9 |
| 90–92%     | 3.7 |
| 87–89%     | 3.
| 83–86%     | 3.0 |
| 80–82%     | 2.7 |
| 77–79%     | 2.3 |
| 73–76%     | 2.0 |
| 70–72%     | 1.7 |
| 67–69%     | 1.3 |
| 63–66%     | 1.0 |
| 60–62%     | 0.7 |
| 0–59%      | 0.0 |

We would love to be able to show students and parents the students current grade part way through the semester based on already graded tests. We might also consider showing their final grade based on both graded an upgraded tests, but aren't sure if this would be useful or not.

In an effort to keep grades consistent between classes we would also like to be able to grade each individual test on a curve. The amount of the curve for all students will be based on the top performer of that test having their score adjusted from their graded scored up to 100 points. This difference will be added to all other students in the class. We should be able to show earned grade (alphabetic and numeric) as well as curved grade (alphabetic and numeric) for each test as well as their total current grade. Obviously, ungraded tests should not have the curve applied.

Ideally the grading system should be as flexible as possible. In the past classes have had different categories of work including quizzes, homework, labs, tests, and final exams. Each different type of work can represent a different percentage of the final grade. For example all quizzes are graded from 1-10 points, and cumulatively account for 15% of final grade.

This is a sample breakdown for a class

- Quizzes: 15%
- Homework: 20%
- Labs: 10%
- Tests: 25%
- Final Exam: 30%

Based on discussions with several teachers they indicated that they all use tests, almost all use homework, some use quizzes, science and engineering classes use labs, and roughly half have final exams.

Additional considerations that we would be willing to pay extra for are as follows

- Deductions of a letter grade for attendance problems such as missing X number of classes
- Some students struggle at classes initially, and would benefit from additional bonus / makeup work?
- Allow test re-takes for those students who want to retake a test
- Allow each student to drop the lowest grade in certain categories
- Increase / Decrease grade due to many times the parent have called to complain

We also welcome ideas from you for additional functionality, discussions with you to help clarify the requirements, as well as ideas for simplifying the system and also making the system more flexible.

# C3ProjectTemplate

See solutions in different languages in the "Templates" directory. Once you decide which language you'd like to use,
simply open that directory in your favorite IDE, and you should be able to run the included unit tests "out of the box".

## Duplicating this Repo

To create a duplicate repository from this one, follow these steps:

1. Create your new repository. For example, MyNewRepo.

2. Open Git Bash.

3. Create a bare clone of the repository.

   ```
   git clone --bare https://github.com/Ingage-Meetup/MyNewRepo.git
   ```

4. Mirror-push to the new repository.

   ```
   cd MyNewRepo.git
   git push --mirror https://github.com/Ingage-Meetup/MyNewRepo.git
   ```

5. Remove the temporary local repository you created earlier.

   ```
   cd ..
   rm -rf OLD-REPOSITORY.git
   ```

Your new repository now contains a mirror of this repo.

The recommended IDEs are as follows, but feel free to use whatever IDE you are comfortable with.

- [C#](Templates/C%23) - [Microsoft Visual Studio](https://visualstudio.microsoft.com/vs/community/)
- [Java](Templates/Java) - [IntelliJ Idea](https://www.jetbrains.com/idea/download) (Community Edition is fine)
- [JavaScript](Templates/JavaScript) - [Microsoft Visual Studio Code](https://code.visualstudio.com/)
- [Kotlin](Templates/Kotlin) - [IntelliJ Idea](https://www.jetbrains.com/idea/download) (Community Edition is fine)
- [Python](Templates/Python) - [Pycharm](https://www.jetbrains.com/pycharm/download/?section=windows) (Community Edition is fine)
- [TypeScript](Templates/TypeScript) - [Microsoft Visual Studio Code](https://code.visualstudio.com/)

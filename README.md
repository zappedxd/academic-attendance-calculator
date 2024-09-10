Here's the updated README file for your Attendance Calculator, reflecting the changes to track the number of lectures attended and excluding singular holidays:

```markdown
# Attendance Calculator

This web-based Attendance Calculator helps you track and calculate your attendance percentage for different subjects over a specified period.
It accounts for both holidays and vacation periods, excluding these dates from the attendance calculations.

## Features

- Date Range Input: Specify the start and end dates for the period you want to calculate attendance for.
- Singular Holidays: Input multiple singular holidays to exclude them from calculations.
- Vacation Periods: Input vacation periods with a start and end date.
- Dynamic Attendance Fields: Enter the number of lectures attended for each subject.
- Attendance Calculation: Automatically calculates the attendance percentage for each subject and overall attendance percentage.
- Timetable Integration: Uses a predefined timetable to determine lecture days for each subject.

## Usage

1. **Download or Clone the Repository**
   ```bash
   git clone https://github.com/zappedxd/academic-attendance-calculator.git
   ```
   or download the ZIP file from [GitHub Releases](https://github.com/zappedxd/academic-attendance-calculator/releases).

2. **Open the HTML File**
   - Navigate to the folder where the HTML file is located.
   - Open `attendance.html` in a web browser.

3. **Input Data**
   - **Start Date**: Enter the start date of the period.
   - **End Date**: Enter the end date of the period.
   - **Holidays**: Enter multiple singular holidays in the format `yyyy-mm-dd` separated by commas.
   - **Vacations**: Enter multiple vacation periods in the format `yyyy-mm-dd,yyyy-mm-dd` separated by semicolons.
   - **Lectures Attended**: Enter the number of lectures attended for each subject.

4. **Calculate Attendance**
   - Click the **Calculate Attendance** button to get the attendance percentages.

## Customizing Your Timetable

To customize the timetable in the Attendance Calculator, you'll need to modify the `timetable` object in the JavaScript code of `attendance.html`. This object defines which subjects are scheduled on which weekdays. Each subject is associated with an array of numbers representing weekdays (0 for Monday through 4 for Friday) when the lectures are held.

Example: Suppose your timetable is as follows:
- Subject A: Mondays and Thursdays
- Subject B: Tuesdays and Fridays

You would update the `timetable` object in the JavaScript code like this:

```javascript
const timetable = {
    'Subject A': [0, 3], // Monday and Thursday
    'Subject B': [1, 4]  // Tuesday and Friday
};
```

In this example, `[0, 3]` represents Monday and Thursday, and `[1, 4]` represents Tuesday and Friday. Adjust these arrays to match your own weekly timetable, ensuring that each subject's lecture days are accurately reflected. Save the changes to the HTML file, and your attendance calculations will automatically use the updated timetable.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to fork the repository, make changes, and create a pull request. Any contributions are welcome!

Happy calculating!
```

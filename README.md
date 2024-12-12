# **Technical Challenge: Habit Tracker Application**

## **Project Description**
Create a habit tracker application where users can:
1. Add a habit they want to track.
2. Log their progress whenever they complete a habit.
3. View a summary of their progress for each habit.
4. Fetch motivational quotes from an API to encourage users.
5. Optimize performance in list rendering and complex functions using advanced hooks.

---

## **Functional Requirements**
1. **Add Habits**: 
   - A form with an `input` field for the habit name.
   - On form submission, the habit is added to a list.

2. **Log Progress**:
   - Each habit will have a button to log completion for the current day.
   - Show the streak of consecutive days the habit has been maintained.

3. **Progress Summary**:
   - Display a list of all habits with their progress (name, streak).
   - Include a search/filter input to find specific habits.

4. **Fetch Motivational Quotes**:
   - Fetch a motivational quote from an API such as [ZenQuotes API](https://zenquotes.io/) or [Quotes REST API](https://api.quotable.io/random) when the user logs progress.
   - Display the quote prominently to encourage the user.

5. **Temporary Persistence**:
   - Habits and their progress should persist across page reloads (use `localStorage`).

---

## **Technical Requirements**
1. **Use of Basic and Advanced Hooks**:
   - **`useState`**: To manage states like habits, progress, the search filter, and the fetched quote.
   - **`useEffect`**: To sync habit data with `localStorage` and fetch motivational quotes.
   - **`useRef`**: For managing form references (e.g., clearing the input field).
   - **`useCallback`**: To memoize functions passed as props (e.g., handle progress logging).
   - **`useMemo`**: To optimize habit list filtering.

2. **Styling**: Use plain CSS or a library like Tailwind CSS for styling.

---

## **Component Breakdown**
1. **App**: Main component managing global state.
2. **HabitList**: Displays the list of habits with details and actions.
3. **HabitForm**: A form for adding a new habit.
4. **HabitItem**: Component for individual habits with their progress.
5. **MotivationalQuote**: Component to display a fetched motivational quote.

---

## **Bonus Points**
- **Validations**: Prevent duplicate habits or empty fields.
- **Responsive Design**: Ensure it looks good on mobile devices.
- **Charts**: Use a library like `chart.js` to visually display progress (optional).

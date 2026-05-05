# Report with Findings and Design Improvement Suggestions

Based on the quantitative logs and qualitative feedback gathered during the usability testing of the Zenith Wellness Prototype, we have identified the following key findings and actionable design improvements:

## Finding 1: Generic System Feedback
*   **Observation:** Users were slightly confused by the generic "Action recorded!" toast notification when using the Quick Actions on the Home screen. They wanted confirmation of *what* specific action was logged.
*   **Improvement Suggestion:** Implement Dynamic Contextual Toasts. Update the JavaScript logic so that clicking the water icon triggers a specific confirmation like, *"Logged 1 Glass of Water!"* This provides immediate, reassuring, and specific feedback to the user.

## Finding 2: Expectation of Native Gestures
*   **Observation:** 40% of the users (2 out of 5) attempted to use native mobile swipe gestures (swiping left or right) to navigate between the Home, Activity, and Profile tabs before realizing they had to click the bottom bar.
*   **Improvement Suggestion:** Add Swipe Event Listeners. Enhance the prototype's JavaScript to detect horizontal touch-swipes, allowing users to transition between screens naturally. This matches their existing mental models of how native mobile applications operate.

## Finding 3: Profile Navigation Friction
*   **Observation:** During Scenario 3, some users tried to access their profile by clicking the small avatar image on the top-right of the Home screen, rather than using the designated 'Profile' icon in the bottom navigation bar.
*   **Improvement Suggestion:** Link Top Avatar to Profile Screen. Make the profile picture in the header a clickable element that routes the user directly to the Profile tab. This creates a secondary, intuitive navigation path and reduces user friction.

## Finding 4: Static Data Visualization
*   **Observation:** On the "Activity" screen, users attempted to tap the bar chart to see exact data points for specific days, but the chart is currently static CSS.
*   **Improvement Suggestion:** Make the chart interactive. Tapping a bar should highlight it and display a small tooltip showing the exact duration or calorie count for that specific day.

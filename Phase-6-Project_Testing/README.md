1. Testing Objectives
 Functional Testing: Verify that the user input text is successfully accepted and processed by the Gemini model to generate comic scripts without crashing.
 API Integration Testing: Ensure secure communication with the Google Gemini API and proper handling of API responses.
 UI Responsiveness Testing: Check that the generated scripts display cleanly and legibly across various screen sizes.
2. Test Cases & Scenarios
 Test Case 1: Valid Prompt Input
 Input: "A cyberpunk detective solving a mystery in a neon city."
 Expected Result: The system successfully returns a structured comic script with character descriptions and panel breakdowns.
 Status: Passed.
 Test Case 2: Empty/Blank Input Handling
 Input: Clicking generate without entering text.
 Expected Result: The application prompts the user to enter a valid description.
 Status: Passed.
 Test Case 3: API Error Handling
 Scenario: Simulating network loss or invalid API key.
 Expected Result: Graceful error message displayed to the user instead of a system crash.
 Status: Passed.
3. Bug Fixes & Optimizations
 Optimized prompt formatting to ensure Gemini consistently outputs data in clear, separated sections (Panels and Dialogues).
 Added environment variable checks to prevent application startup if the API key is missing.

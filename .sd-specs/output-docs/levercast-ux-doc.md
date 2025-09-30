# Levercast User Interface Description Document

This document outlines the user interface design for Levercast, based on the "Power-User Dashboard" concept.

## Layout Structure

The interface is built on a single-screen, three-column layout designed for maximum efficiency on desktop devices.

-   **Left Column (Input):** A dedicated space for the user to input their raw content ideas via text or voice.
-   **Center Column (Editors):** Contains the AI-generated, editable posts. There will be two distinct editor components, one for LinkedIn and one for Twitter, clearly separated and labeled.
-   **Right Column (Previews):** Displays live, non-interactive previews of how the posts will appear on each platform. These previews update in real-time as the user edits the content in the center column.
-   **Header:** A persistent header at the top of the page will contain the Levercast logo and a user profile icon for accessing account settings and logging out.

## Core Components

-   **Input Capture:** A primary text area for typing ideas. It will be accompanied by a "Record Voice" button for voice-to-text input and an "Attach Image" button. A prominent "Generate Posts" button will initiate the AI process.
-   **Content Editors:** Two separate, clearly labeled text areas for the LinkedIn and Twitter content. Each editor will provide standard text formatting controls.
-   **Live Previews:** Two components that visually mimic the UI of a LinkedIn post and a Twitter post, respectively. They will render the content from the editors, providing an accurate preview.
-   **Action Bar:** A primary "Publish All" button will be located in the center column. Individual "Publish" buttons for each platform may also be included.
-   **Authentication:** A secure OAuth flow will be used for connecting LinkedIn and Twitter accounts, managed under the User Profile section.

## Interaction Patterns

1.  The user enters an idea into the input text area or uses the voice-to-text feature.
2.  The user clicks the "Generate Posts" button.
3.  The center column populates with the AI-generated content for LinkedIn and Twitter, and the right column populates with the corresponding visual previews.
4.  The user can click into either the LinkedIn or Twitter editor in the center column to make changes.
5.  As the user types, the corresponding preview in the right column updates instantly to reflect the changes.
6.  Once satisfied, the user clicks "Publish All" to post the content directly to their connected accounts.

## Visual Design Elements & Color Scheme

-   **Theme:** The design will be clean, modern, and professional, with a minimalist aesthetic to keep the focus on the user's content.
-   **Color Scheme:** A neutral palette will be used for the overall interface (e.g., light grays, white, and dark text for high readability). A single, strong accent color (like a vibrant blue) will be used for primary calls-to-action like "Generate Posts" and "Publish" to guide the user.
-   **Iconography:** Simple, universally recognized line icons will be used for actions like "Record Voice," "Attach Image," and "User Profile."

## Mobile, Web App, Desktop Considerations

-   **Desktop (Primary):** The three-column layout is the default and intended experience for desktop users.
-   **Web App:** The application is a responsive web app that functions across all modern browsers.
-   **Mobile & Tablet:** On smaller screens, the three-column layout is not viable. The design will adapt by stacking the columns vertically. The experience will likely resemble a guided workflow out of necessity:
    1.  The input area is presented first.
    2.  After generation, the user scrolls down to a tabbed or stacked view where they can toggle between editing/previewing the LinkedIn and Twitter posts.

## Typography

-   **Font Family:** A clean, highly readable sans-serif font like **Inter** or **Roboto** will be used throughout the application.
-   **Headings:** Section titles and labels will use a semi-bold weight to establish a clear visual hierarchy.
-   **Body Text:** The main text within the editors and previews will be set at a comfortable size for reading and writing (e.g., 16px) in a regular weight.

## Accessibility

-   **Color Contrast:** All text and UI elements will adhere to WCAG AA contrast ratio guidelines to ensure readability for users with low vision.
-   **Keyboard Navigation:** The entire application will be navigable and operable using only a keyboard. Tabbing order will be logical, flowing from left to right and top to bottom.
-   **Screen Reader Support:** Semantic HTML5 tags (`<header>`, `<main>`, `<aside>`, `<button>`) will be used to structure the content correctly for screen readers. All interactive elements will have appropriate ARIA labels.
-   **Focus States:** Clear and visible focus indicators will be present on all interactive elements.

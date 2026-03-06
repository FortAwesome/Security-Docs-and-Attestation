# Voluntary Product Accessibility Template (VPAT®) 2.5

**Product Name:** Font Awesome  
**Product Version:** 3.1.60  
**Report Date:** February 2026  
**Report Version:** 1.0  
**Prepared By:** Jory Raphael, Head of Product  
**Contact:** hello@fontawesome.com  
**Description:** Font Awesome is an icon library and toolkit used by millions of designers and developers to add scalable vector icons to websites and applications. This report covers the fontawesome.com web application, including icon search, Kit management, and account features.

---

## Applicable Standards / Guidelines

This report covers the degree of conformance for the following accessibility standards/guidelines:

| Standard / Guideline | Included in Report |
|---|---|
| [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/) | Yes |
| [Revised Section 508 standards](https://www.access-board.gov/ict/) published January 18, 2017 and corrected January 22, 2018 | Yes |

---

## Terms

The following terms are used throughout this report:

| Term | Meaning |
|---|---|
| **Supports** | The functionality of the product has at least one method that meets the criterion without known defects or meets with equivalent facilitation. |
| **Partially Supports** | Some functionality of the product does not meet the criterion. |
| **Does Not Support** | The majority of product functionality does not meet the criterion. |
| **Not Applicable** | The criterion is not relevant to the product. |
| **Not Evaluated** | The product has not been evaluated against the criterion. This can be used only in WCAG Level AAA criteria. |

---

## WCAG 2.1 Report

### Table 1: Success Criteria, Level A

| Criteria | Conformance Level | Remarks and Explanations |
|---|---|---|
| [1.1.1 Non-text Content](https://www.w3.org/TR/WCAG21/#non-text-content) (Level A) | Supports | All images include descriptive alt text or are marked decorative with empty alt attributes. Partner and sponsor logo links include visually hidden text labels. |
| [1.2.1 Audio-only and Video-only (Prerecorded)](https://www.w3.org/TR/WCAG21/#audio-only-and-video-only-prerecorded) (Level A) | Not Applicable | fontawesome.com does not publish audio-only or video-only content. All video content includes both audio and visual tracks and is covered under 1.2.2 and 1.2.3. |
| [1.2.2 Captions (Prerecorded)](https://www.w3.org/TR/WCAG21/#captions-prerecorded) (Level A) | Supports | Captions are enabled on prerecorded video content hosted via Vimeo. |
| [1.2.3 Audio Description or Media Alternative (Prerecorded)](https://www.w3.org/TR/WCAG21/#audio-description-or-media-alternative-prerecorded) (Level A) | Supports | An audio description track or text-based media alternative is provided for prerecorded video content. |
| [1.3.1 Info and Relationships](https://www.w3.org/TR/WCAG21/#info-and-relationships) (Level A) | Supports | Semantic HTML is used throughout. Heading hierarchy, form labels, and ARIA relationships have been reviewed and corrected. Duplicate IDs and multiple label issues identified during audit have been resolved. |
| [1.3.2 Meaningful Sequence](https://www.w3.org/TR/WCAG21/#meaningful-sequence) (Level A) | Supports | Content order in the DOM is logical and meaningful without CSS applied. |
| [1.3.3 Sensory Characteristics](https://www.w3.org/TR/WCAG21/#sensory-characteristics) (Level A) | Supports | Instructions and UI guidance do not rely solely on shape, size, visual location, or orientation. |
| [1.4.1 Use of Color](https://www.w3.org/TR/WCAG21/#use-of-color) (Level A) | Supports | Color is never used as the sole means of conveying information, indicating an action, prompting a response, or distinguishing a visual element. |
| [1.4.2 Audio Control](https://www.w3.org/TR/WCAG21/#audio-control) (Level A) | Not Applicable | No audio plays automatically on fontawesome.com. A sound effect is present as an easter egg triggered only by deliberate user interaction (clicking a specific icon); it does not auto-play and is therefore not subject to this criterion. |
| [2.1.1 Keyboard](https://www.w3.org/TR/WCAG21/#keyboard) (Level A) | Partially Supports | Most functionality is operable via keyboard. Some interactions in the Style Toolkit section have inconsistent keyboard behavior. Additionally, tab behavior is inconsistent between Chrome and Safari; currently under investigation. Remediation is planned. |
| [2.1.2 No Keyboard Trap](https://www.w3.org/TR/WCAG21/#no-keyboard-trap) (Level A) | Supports | No keyboard traps were identified during testing. Users can navigate away from all interactive elements including modals, dropdowns, and color pickers using standard keyboard commands. |
| [2.1.4 Character Key Shortcuts](https://www.w3.org/TR/WCAG21/#character-key-shortcuts) (Level A) | Supports | A single-character keyboard shortcut (/) is implemented in the documentation section to launch the search interface. The shortcut only activates when focus is on the page and does not fire when focus is within a form field or text input, meeting the requirement that shortcuts do not interfere with standard text entry. |
| [2.2.1 Timing Adjustable](https://www.w3.org/TR/WCAG21/#timing-adjustable) (Level A) | Supports | An auto-cycling animation in the homepage hero area cycles through icon styles. Users can click the logo to advance to the next style and pause the animation. A second click advances to the next style and restarts the auto-cycle, giving users full control over the timing behavior. |
| [2.2.2 Pause, Stop, Hide](https://www.w3.org/TR/WCAG21/#pause-stop-hide) (Level A) | Supports | The auto-cycling hero animation can be paused by clicking the logo icon. Clicking again restarts the animation. Users have a clear, discoverable mechanism to stop the auto-playing content. |
| [2.3.1 Three Flashes or Below Threshold](https://www.w3.org/TR/WCAG21/#three-flashes-or-below-threshold) (Level A) | Supports | No flashing or strobing content was identified during testing. |
| [2.4.1 Bypass Blocks](https://www.w3.org/TR/WCAG21/#bypass-blocks) (Level A) | Partially Supports | A skip navigation link is not currently present. Users must tab through the full navigation on every page load. A visually hidden "Skip to main content" link is planned for a future release. |
| [2.4.2 Page Titled](https://www.w3.org/TR/WCAG21/#page-titled) (Level A) | Supports | Each page has a unique, descriptive title that identifies the current page and site. Titles are set dynamically per route. |
| [2.4.3 Focus Order](https://www.w3.org/TR/WCAG21/#focus-order) (Level A) | Supports | Focus moves in a logical, meaningful sequence throughout the site consistent with the visual layout and content order. |
| [2.4.4 Link Purpose (In Context)](https://www.w3.org/TR/WCAG21/#link-purpose-in-context) (Level A) | Supports | All links have discernible names that describe their purpose. Previously identified nameless links have been resolved by adding aria-label attributes and visually hidden text. |
| [2.5.1 Pointer Gestures](https://www.w3.org/TR/WCAG21/#pointer-gestures) (Level A) | Not Applicable | No functionality requires multi-point or path-based pointer gestures. |
| [2.5.2 Pointer Cancellation](https://www.w3.org/TR/WCAG21/#pointer-cancellation) (Level A) | Supports | Actions are triggered on mouse-up rather than mouse-down, allowing users to cancel accidental activations by moving the pointer away before releasing. |
| [2.5.3 Label in Name](https://www.w3.org/TR/WCAG21/#label-in-name) (Level A) | Supports | Accessible names for interactive elements contain the visible label text, ensuring consistency for speech input users. |
| [2.5.4 Motion Actuation](https://www.w3.org/TR/WCAG21/#motion-actuation) (Level A) | Not Applicable | No functionality is triggered by device motion or user movement. |
| [3.1.1 Language of Page](https://www.w3.org/TR/WCAG21/#language-of-page) (Level A) | Supports | The `<html>` element includes a valid `lang="en"` attribute on all pages. |
| [3.2.1 On Focus](https://www.w3.org/TR/WCAG21/#on-focus) (Level A) | Supports | No context changes occur as a result of an element receiving focus. |
| [3.2.2 On Input](https://www.w3.org/TR/WCAG21/#on-input) (Level A) | Supports | Changing the value of form controls does not automatically trigger unexpected context changes such as page navigation or form submission. |
| [3.3.1 Error Identification](https://www.w3.org/TR/WCAG21/#error-identification) (Level A) | Supports | Form validation errors are clearly identified and describe which field failed and why. |
| [3.3.2 Labels or Instructions](https://www.w3.org/TR/WCAG21/#labels-or-instructions) (Level A) | Supports | All form fields have programmatic labels via visible label elements or aria-label attributes. Placeholder text is used in addition to, not instead of, proper labels. |
| [4.1.1 Parsing](https://www.w3.org/TR/WCAG21/#parsing) (Level A) | Supports | HTML is well-formed with no duplicate IDs. Issues identified during audit including duplicate id="rotate-custom" attributes have been resolved. |
| [4.1.2 Name, Role, Value](https://www.w3.org/TR/WCAG21/#name-role-value) (Level A) | Supports | Interactive elements have appropriate names, roles, and states. Issues identified during audit including an unnamed button, an untitled iframe, and a prohibited ARIA attribute have been resolved. |

---

### Table 2: Success Criteria, Level AA

| Criteria | Conformance Level | Remarks and Explanations |
|---|---|---|
| [1.2.4 Captions (Live)](https://www.w3.org/TR/WCAG21/#captions-live) (Level AA) | Not Applicable | No live audio or video streams are currently published on fontawesome.com. When live streaming has been conducted on the site, captions have been included. This criterion will be revisited if live streaming becomes a regular feature. |
| [1.2.5 Audio Description (Prerecorded)](https://www.w3.org/TR/WCAG21/#audio-description-prerecorded) (Level AA) | Partially Supports | Prerecorded video content on the homepage does not currently include a dedicated audio description track. Users who cannot see the video may miss visually-presented information. An audio description track or enhanced text alternative is planned for a future release. |
| [1.3.4 Orientation](https://www.w3.org/TR/WCAG21/#orientation) (Level AA) | Supports | The site does not lock to a single orientation. Content reflows correctly in both portrait and landscape orientations on mobile devices. |
| [1.3.5 Identify Input Purpose](https://www.w3.org/TR/WCAG21/#identify-input-purpose) (Level AA) | Supports | Form inputs include appropriate autocomplete attributes. Sign-in and sign-up fields include autocomplete="email" and autocomplete="current-password" as appropriate. |
| [1.4.3 Contrast (Minimum)](https://www.w3.org/TR/WCAG21/#contrast-minimum) (Level AA) | Supports | All text content meets the required 4.5:1 contrast ratio for normal text and 3:1 for large text. Color themes used in the homepage hero animation have been verified to meet minimum contrast requirements against the white background. |
| [1.4.4 Resize Text](https://www.w3.org/TR/WCAG21/#resize-text) (Level AA) | Supports | Text resizes cleanly up to 200% zoom without loss of content or functionality. No overlapping, clipping, or disappearing content was observed. |
| [1.4.5 Images of Text](https://www.w3.org/TR/WCAG21/#images-of-text) (Level AA) | Supports | In a small number of cases, text is rendered within an SVG image. These instances represent the visual identity of specific icon packs where the specific visual presentation is essential to the content being communicated, meeting the exception for essential images of text. All such images include appropriate alt text and titles. |
| [1.4.10 Reflow](https://www.w3.org/TR/WCAG21/#reflow) (Level AA) | Supports | Content reflows into a single scrollable column at 320px viewport width with no horizontal scrolling required. |
| [1.4.11 Non-text Contrast](https://www.w3.org/TR/WCAG21/#non-text-contrast) (Level AA) | Supports | UI components including buttons, input borders, checkboxes, radio buttons, and focus indicators meet the required 3:1 contrast ratio against adjacent colors. |
| [1.4.12 Text Spacing](https://www.w3.org/TR/WCAG21/#text-spacing) (Level AA) | Supports | Increasing line height, letter spacing, word spacing, and paragraph spacing to WCAG-specified maximums does not cause content loss, overlap, or clipping. |
| [1.4.13 Content on Hover or Focus](https://www.w3.org/TR/WCAG21/#content-on-hover-or-focus) (Level AA) | Partially Supports | Tooltip and balloon content triggered on hover is persistent and hoverable — users can move the pointer over tooltip content without it disappearing. However, tooltips cannot currently be dismissed using the Escape key without moving the pointer. Escape dismissal is planned for a future release. |
| [2.4.5 Multiple Ways](https://www.w3.org/TR/WCAG21/#multiple-ways) (Level AA) | Supports | Multiple methods are available to locate content, including a sitemap, header and footer navigation, in-page links, and icon search. Documentation includes a keyboard-triggered search interface. |
| [2.4.6 Headings and Labels](https://www.w3.org/TR/WCAG21/#headings-and-labels) (Level AA) | Supports | Headings and form labels are descriptive and clearly communicate the purpose of each section and input field. |
| [2.4.7 Focus Visible](https://www.w3.org/TR/WCAG21/#focus-visible) (Level AA) | Supports | A visible focus indicator is present on all interactive elements throughout the site. No instances of invisible or missing focus indicators were identified during testing. |
| [3.1.2 Language of Parts](https://www.w3.org/TR/WCAG21/#language-of-parts) (Level AA) | Not Applicable | All human-language content on fontawesome.com is in English. No content in other languages is present. |
| [3.2.3 Consistent Navigation](https://www.w3.org/TR/WCAG21/#consistent-navigation) (Level AA) | Supports | Main navigation appears in the same location and order across all pages of the site. |
| [3.2.4 Consistent Identification](https://www.w3.org/TR/WCAG21/#consistent-identification) (Level AA) | Supports | Components that perform the same function are identified consistently across pages. Search inputs, copy buttons, and download buttons use consistent labeling throughout the site. |
| [3.3.3 Error Suggestion](https://www.w3.org/TR/WCAG21/#error-suggestion) (Level AA) | Supports | Form validation error messages describe not only what went wrong but how to correct it, providing actionable guidance to users. |
| [3.3.4 Error Prevention (Legal, Financial, Data)](https://www.w3.org/TR/WCAG21/#error-prevention-legal-financial-data) (Level AA) | Supports | Subscription and purchase flows include a confirmation step before charges are made. Destructive actions such as canceling a subscription or deleting an account require explicit user confirmation. |
| [4.1.3 Status Messages](https://www.w3.org/TR/WCAG21/#status-messages) (Level AA) | Partially Supports | Some status messages such as form confirmations and notifications may not be fully announced to screen reader users via ARIA live regions. A full audit of aria-live and role="status" implementation across all dynamic status messages is underway, with remediation planned for a future release. |

---

## Revised Section 508 Report

### Chapter 3: Functional Performance Criteria (FPC)

| Criteria | Conformance Level | Remarks and Explanations |
|---|---|---|
| 302.1 Without Vision | Partially Supports | Screen reader users can access most site functionality. Known gaps include some keyboard navigation inconsistencies in the Style Toolkit, missing skip navigation, and status messages not fully announced via ARIA live regions. Remediation is in progress. |
| 302.2 With Limited Vision | Partially Supports | The site supports text resizing to 200%, reflow at 320px, and adequate contrast for most content. A small number of secondary decorative headings do not meet minimum contrast requirements. Remediation is planned. |
| 302.3 Without Perception of Color | Supports | Color is never used as the sole means of conveying information, indicating an action, or distinguishing content. All information conveyed with color is also available through text or other visual means. |
| 302.4 Without Hearing | Supports | All video content includes captions. No audio-only content is published. The site does not rely on audio to convey information. |
| 302.5 With Limited Hearing | Supports | Captions are provided for prerecorded video content. No functionality depends on the ability to hear audio. |
| 302.6 Without Speech | Not Applicable | No functionality on fontawesome.com requires speech input. |
| 302.7 With Limited Manipulation | Partially Supports | Most functionality is operable via keyboard without requiring fine motor control. Some interactions in the Style Toolkit have inconsistent keyboard behavior. Pointer cancellation is supported — actions trigger on mouse-up rather than mouse-down. Remediation of keyboard inconsistencies is planned. |
| 302.8 With Limited Reach and Strength | Partially Supports | The site does not require device motion or physical gestures. Keyboard navigation covers most functionality. Known keyboard inconsistencies in the Style Toolkit are being addressed. |
| 302.9 With Limited Language, Cognitive, and Learning Abilities | Supports | The site uses clear, consistent navigation, descriptive headings and labels, plain language, and helpful error messages that explain how to correct mistakes. No time limits are imposed on users except for the auto-cycling hero animation, which is being addressed. |

---

### Chapter 4: Hardware

| Criteria | Conformance Level | Remarks and Explanations |
|---|---|---|
| 402 Closed Functionality | Not Applicable | fontawesome.com is a web-based software product with no hardware component. |
| 403 Biometrics | Not Applicable | |
| 404 Preservation of Information Provided for Accessibility | Not Applicable | |
| 405 Privacy | Not Applicable | |
| 406 Standard Connections | Not Applicable | |
| 407 Operable Parts | Not Applicable | |
| 408 Display Screens | Not Applicable | |
| 409 Status Indicators | Not Applicable | |
| 410 Color Coding | Not Applicable | |
| 411 Audible Signals | Not Applicable | |
| 412 ICT with Two-Way Voice Communication | Not Applicable | |
| 413 Closed Caption Processing Technologies | Not Applicable | |
| 414 Audio Description Processing Technologies | Not Applicable | |
| 415 User Controls for Captions and Audio Descriptions | Not Applicable | |

---

### Chapter 5: Software

| Criteria | Conformance Level | Remarks and Explanations |
|---|---|---|
| [501.1 Scope – Incorporation of WCAG 2.x](https://www.access-board.gov/ict/#501.1) | See WCAG tables above | Conformance with WCAG 2.1 Level A and AA is documented in the WCAG 2.1 Report above. |
| [502.2.1 User Control of Accessibility Features](https://www.access-board.gov/ict/#502.2.1) | Not Applicable | fontawesome.com is not a platform or authoring tool in the traditional sense and does not expose platform-level accessibility settings for user configuration. However, Font Awesome as a toolkit proactively builds accessibility in by default for the developers who use it: icons are hidden from assistive technology via aria-hidden="true" by default, SVG icons injected via Kits automatically receive aria-hidden="true", animations respect the prefers-reduced-motion CSS media feature out of the box, and comprehensive accessibility guidance is provided in documentation at docs.fontawesome.com/web/dig-deeper/accessibility to help developers implement icons accessibly in their own products. |
| [502.2.2 No Disruption of Accessibility Features](https://www.access-board.gov/ict/#502.2.2) | Supports | The site does not interfere with accessibility features provided by the user's browser or operating system, including screen readers, zoom, high contrast mode, and reduced motion settings. |
| [502.3 Accessibility Services](https://www.access-board.gov/ict/#502.3) | Supports | The site uses standard HTML, ARIA, and browser accessibility APIs. Interactive elements expose appropriate names, roles, and states to assistive technologies. |
| [502.4 Platform Accessibility Features](https://www.access-board.gov/ict/#502.4) | Not Applicable | fontawesome.com is a web application. Platform accessibility is handled by the user's browser and operating system. |
| [503.2 User Preferences](https://www.access-board.gov/ict/#503.2) | Supports | The site respects user preferences including browser zoom, system font size, and OS-level reduced motion settings. |
| [503.3 Alternative User Interfaces](https://www.access-board.gov/ict/#503.3) | Not Applicable | No alternative user interfaces are offered. |
| [503.4 User Controls for Captions and Audio Description](https://www.access-board.gov/ict/#503.4) | Not Applicable | No time-based media requiring user-controlled captions or audio description playback controls is present. |

---

### Chapter 6: Support Documentation and Services

| Criteria | Conformance Level | Remarks and Explanations |
|---|---|---|
| [601.1 Scope](https://www.access-board.gov/ict/#601.1) | See below | |
| [602.2 Accessibility and Compatibility Features](https://www.access-board.gov/ict/#602.2) | Supports | Accessibility conformance information is documented in this VPAT and is publicly available. |
| [602.3 Electronic Support Documentation](https://www.access-board.gov/ict/#602.3) | Supports | Product documentation is available electronically at docs.fontawesome.com. Documentation uses semantic HTML, descriptive headings, and is navigable by keyboard and screen reader. |
| [602.4 Alternate Formats for Non-Electronic Support Documentation](https://www.access-board.gov/ict/#602.4) | Not Applicable | All support documentation is provided electronically. No print or non-electronic documentation is distributed. |
| [603.2 Accessibility of Support Services](https://www.access-board.gov/ict/#603.2) | Supports | Customer support is available via email and web-based contact forms, which do not require voice communication or other inaccessible means of contact. |
| [603.3 Provision of Accessible Support](https://www.access-board.gov/ict/#603.3) | Supports | Support staff are able to assist users with accessibility-related questions and issues via accessible communication channels. |

---

## Testing Methodology

**Testing approach:** This audit was conducted internally using a combination of automated scanning tools and manual testing across key pages and user flows on fontawesome.com and docs.fontawesome.com.

**Automated tools used:**
- WAVE (WebAIM) — browser extension, used for error detection and contrast checking
- Google Lighthouse — built-in Chrome DevTools, used for accessibility scoring and issue identification

**Manual testing:**
- Keyboard-only navigation tested in Chrome and Safari
- Visual checks for focus indicators, color contrast, reflow, and text spacing
- Form validation and error message review

**Assistive technologies tested:**
- VoiceOver with Safari (macOS)

**Pages / flows evaluated:**
- [x] Homepage (fontawesome.com)
- [x] Icon search and browse
- [x] Icon detail modal
- [x] Kit management
- [x] Account / billing
- [x] Sign up / sign in
- [x] Documentation (docs.fontawesome.com)

**Notes:** This VPAT reflects the state of the product as of the report date. Some criteria marked Partially Supports have active remediation in progress. The document will be updated as fixes are released.

---

## Known Issues and Remediation Roadmap

| Issue | Criterion | Severity | Status | Target Fix |
|---|---|---|---|---|
| Skip navigation link not present | 2.4.1 | Major | Open | 3.2 |
| Some keyboard interactions in the Style Toolkit are inconsistent | 2.1.1 | Major | Open | 3.2 |
| Tab behavior is inconsistent between Chrome and Safari; under investigation | 2.1.1 | Major | Open | 3.2 |
| Balloon tooltips cannot be dismissed with the Escape key | 1.4.13 | Minor | Open | 3.2 |
| Status messages (e.g. "Copied!", kit save confirmations) may not be fully announced via ARIA live regions | 4.1.3 | Minor | Open | 3.2 |
| Prerecorded homepage video does not have a dedicated audio description track | 1.2.5 | Minor | In Progress | 3.1.70 |

---

## Legal Disclaimer

*This document is provided for informational purposes only. The information provided in this VPAT accurately reflects Font Awesome's conformance with the listed standards as of the report date. Conformance levels noted as "Partially Supports" or "Does Not Support" represent known gaps that may be addressed in future releases. This report should not be construed as a legal guarantee of conformance.*

---

## Revision History

| Version | Date | Description |
|---|---|---|
| 1.0 | February 2026 | Initial report |
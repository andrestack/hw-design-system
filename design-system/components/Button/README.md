# Button

Pill-shaped link or button for the one action a section asks for.

- **Primary**: `accent` fill, `on-accent` text, `shadow-sm`. One per view: "Let's talk", "Get a quote", "Take the free audit".
- **Outline**: transparent, `foreground` text, 1px `border`; the border turns `accent` on hover. For the secondary path, such as "See the work".
- Always `radius-full`, `label` type, 12px × 22px padding, 2px `ring` focus outline offset 3px.
- The consumer provides the label (a verb phrase that says what happens) and the href or click handler.
- Don't stack two primaries side by side. Don't use cream text on teal.

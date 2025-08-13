React Password Generator
A sleek and modern password generator built with React. This application allows users to create secure, customizable passwords and copy them to the clipboard with a single click.

Features
Customizable Length: Generate passwords from 6 to 100 characters using a responsive slider.

Character Sets: Easily include or exclude numbers and special characters.

Instant Regeneration: The password automatically updates whenever the settings are changed.

One-Click Copy: A convenient button to copy the generated password to the clipboard.

Stack Used
React
Focusing on the effective use of hooks for state management, optimization, and side effects.

React Hooks Used
useState
Manages all dynamic data in the application. It holds the state for the password length, the boolean values for the number and special character checkboxes, and the final generated password string.

useEffect
Acts as the "engine" of the application. It listens for any changes in the password settings (length, numbers, or special characters) and automatically triggers the password generation function, ensuring the UI is always in sync.

useCallback
Optimizes performance by memoizing (remembering) the password generation and copy functions. This prevents these functions from being recreated on every single render, making the app more efficient.

useRef
Used to get a direct reference to the password input field. This allows the "Copy" button to programmatically select the text for a seamless user experience without needing to involve React state.

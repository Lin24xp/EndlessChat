📝 Changelog – EndlessChat v2.0
✅ v2.0 – April 17, 2025
🎨 UI Improvements
Added a dark mode layout with a modern, centered chatbox.

Increased chat input size and spacing for better accessibility and mobile use.

Enhanced responsiveness across screen sizes.

🧠 Chat Functionality
Removed the default message limit (previously 10 messages):

File: app/(chat)/api/history/route.ts

Change: const limit = parseInt(searchParams.get('limit') || '10'); → updated or removed.

🔐 Account & Auth
Integrated user login and registration (with authentication).

Users' chat histories are saved to their account and synced across devices.

🐛 Error Handling
Implemented error codes and human-readable error messages.

Added a public error reporting form (via GitHub Issues or an in-app form, depending on your setup).

🔒 Security
Fixed DOM-based XSS vulnerability:

Replaced unsafe innerHTML with textContent in static/script.js.

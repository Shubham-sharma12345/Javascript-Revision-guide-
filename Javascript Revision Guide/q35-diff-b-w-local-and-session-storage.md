# Q35-Diff B/W Local and Session Storage

| **Feature**          | **Local Storage**                                                                                   | **Session Storage**                                                                     |
| -------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| **Persistence**      | Data persists even after closing the browser.                                                       | Data is cleared when the page session ends (i.e., when the page is closed).             |
| **Scope**            | Data is available across different tabs and windows of the same origin.                             | Data is only available for the specific tab or window where it was set.                 |
| **Storage Capacity** | Typically 5-10 MB (varies by browser).                                                              | Typically 5-10 MB (varies by browser).                                                  |
| **Lifetime**         | Data remains until explicitly deleted by the user or script.                                        | Data is only available for the duration of the page session.                            |
| **Use Case**         | Storing long-term preferences, user settings, or any data that should be available across sessions. | Storing temporary data that should only last for the duration of a single page session. |

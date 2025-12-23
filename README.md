This was a practice project to learn core javascript concepts(not all yet) and also a touch on how to use local storage of browser.
The concepts learned I would want to share it to you:

> DOMContentLoaded
The project uses the DOMContentLoaded event to ensure that all HTML elements are fully loaded before JavaScript tries to access or manipulate them. Since JavaScript can execute before the DOM is constructed, this event prevents errors such as accessing elements that do not yet exist. It establishes a safe starting point for initializing the application logic.

> DOM Manipulation
This project dynamically creates, updates, and removes HTML elements using JavaScript instead of relying on static HTML. Each task is represented by a list item that is created at runtime, allowing the UI to change in response to user actions. This demonstrates how JavaScript can directly control the structure and content of a webpage.

> Data and UI Separation
The application maintains a clear separation between data and user interface. Tasks are stored as JavaScript objects inside an array, while the visual representation exists as DOM elements. Actions such as adding, completing, or deleting a task require updating both the data and the UI explicitly, reinforcing the concept that the browser does not automatically sync them.

> Local Storage and Persistence
The project uses localStorage to persist task data across page reloads. Since local storage can only store strings, task data is converted to and from JSON format. This ensures that user data remains available even after refreshing or reopening the browser, highlighting basic client-side persistence.

> Rendering from Stored State
When the application loads, previously saved tasks are rendered from local storage instead of starting with an empty UI. Each task’s completion status is restored visually to match its stored state. This emphasizes the importance of reconstructing the UI based on existing data rather than assuming a fresh state on every load.

> Event Handling
User interactions such as clicking buttons or list items are handled using event listeners. Different behaviors are assigned to different elements, such as toggling task completion or deleting a task. This shows how JavaScript responds to user actions and modifies both data and UI accordingly.

> Event Bubbling and Propagation Control
The delete button exists inside a clickable task element, which introduces event bubbling. The project explicitly stops propagation on the delete action to prevent unintended side effects, such as toggling completion while deleting. This demonstrates how event flow works in the DOM and why controlling it is sometimes necessary.

> Closures and Scope
Each task’s event handlers retain access to their specific task data and DOM element through closures. This allows actions like deletion or completion toggling to work correctly without searching the DOM or data array. It highlights how JavaScript functions remember variables from their creation context.

> Immutability and Array Methods
Instead of mutating the task list directly, the project uses array methods like filter to create updated versions of the data. This approach reduces side effects and makes state changes easier to reason about. It introduces a cleaner and more predictable way to manage application state.

> Synchronization Between State and View
Every change in the application—adding, completing, or deleting a task—is immediately reflected in both the stored data and the UI. This consistent synchronization prevents mismatches between what the user sees and what the application remembers. Understanding this relationship is fundamental to building reliable front-end applications.

More to come!!
Adapt it for a portfolio README

Just tell me 👍

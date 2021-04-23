# uicomponents - Getting Started

## Step 1 - Creating/Updating Components

1. Clone SHARED.UI project - `git clone https://github.com/Impakter/SHARED.UI.git`.

1. Create a new component or update the existing component in the appropriate sub-folder in _/components_ folder.

1. Add the component on _index.js_ file in _/components_ folder if new component is created.

1. Push the changes to _master_ branch


## Step 2 - Adding/Updating Component library

> Now that we have components in shared UI library, we can use those components anywhere in any other project. Make sure either the SHARED.UI library is already added to the project where you want to use the shared components.


**Check if the SHARED.UI is already added to  a project:**

You can confirm this by checking _package.json_ file of that project which should contain “uicomponents” in the list of dependencies.
Use `npm update` from CLI to fetch the latest changes from SHARED.UI library.

(or)

**If it’s a New Project:**

From the project where you want to use the Shared UI components, go to CLI and use 
`npm add https://github.com/Impakter/SHARED.UI.git —-save` to add the SHARED.UI library.





## Step 3 - Using Components
Use `import { ComponentName } from “uicomponents”` inside the parent component where you want to use SHARED.UI components.


***

## Example Usage:


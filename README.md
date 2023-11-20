# CS569 - Final Project - PetFinder API
Create an Angular application to browse the [Petfinder API](https://www.petfinder.com/developers/).
  
For users to be able to use the application they must log in first, which comes in the form of entering a **valid Petfinder API key**.
  
After they log in successfully, a `BreedService` will fetch the list of "Dog" breeds and persist it in the state + `localStorage`, to be used in the future without re-fetching the breeds.
  
The main navigation displays two features: `Search`, and `Bookmarks`. 

### Search Component
A search form will be displayed to search by the following fields:
* `name` (input)
* `type` (hidden field, set to "Dog")
* `breed` (multiple values checkboxes, values read from your BreedService)
* `size`(multiple values checkboxes: small, medium, large, xlarge)
* `gender` (multiple values checkboxes: male, female, unknown)
* `status` (multiple values checkboxes: adoptable, adopted, found)
* `house_trained` (radiobox true/false)
* `location` (read the user location and allow users to enter a new location)
* `distance` (number between 100 and 500)
The search results will be displayed in pages of 20 items per page (allow pagination). 
  
### Dog Details Component
When a Dog is clicked use the `Get Animal` API to display the full details and pictures of the animal. 
* Add a button to add/remove the animal to/from a bookmarks list. A `BookmarkService` will be used to persist the user's bookmarks. 
  
### Bookmarks Component
Display the full list of bookmarks and allow the user to browse to the dog details page.

### Application specifications and requirements
Your project must use the following:  
* State properties in all components and services should be declared as `Signals`.
* The app module has the login logic. Create a featured lazy-loaded module for the rest of the features.
* The project must have a proper UI that complies with the web standards.
* A daily push is required to track your code progress and measure your performance. 

## Final Evaluation 
The submission deadline is on Friday at 9:00 PM. I will meet with you on Saturday at 10:00 AM and evaluate the final project code.  

Good luck, and happy coding!

_Code Honor Submission Policy: Remember to respect the code honor submission policy. All written code must be original. Presenting any code as one’s own work when it came from another source is plagiarism, which includes any matching patterns and code snippets, and will affect your grade. The use of AI is not permitted in this assignment. For more details, check the full course policies in the syllabus._

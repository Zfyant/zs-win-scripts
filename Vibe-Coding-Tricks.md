# Vibe-Coding Core Tips (Froma near non-coder)

## Some stupid amazing trips to keep AI in line and you more sane:
- 1. If your API usage (funding) can keep up with this: Have a daily log that the model writes each finished request to; this helps track when your hitting a debugging wall in repetition. 
 (You can then use AI to view the big picture of all recent updates to pinpoint bigger issues)

- 2. Ensure each function & file has a summary of what it does before it starts.

- 3. Refactor & Prevent files over ~600 lines. (Our editors have a hard time doing entire code edits above this line-count)
- 3.1 Create a line counter script to batch all files in the directory into an MD file that gives you a descending list to track files getting close to this threshold.

- 4. Understand MD files are pretty hand documentation files for both the computer/AI and yourself to easily read and edit.
- 4.1 Get a nice browser extension that can parse MD files into a human-friendly view. (open the MD files in that browser)

- 5. Get familiar with setting up testing/debugging functions on larger projects to figure out where something is going wrong.

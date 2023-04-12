# Git Guideline


## Commit Message Guidelines
 ### Information in commit messages
- Describe why a change is being made.
- How does it address the issue?
- Do not assume the reviewer understands what the original problem was.
- Do not assume the code is self-evident/self-documenting.

### Rules of a great Git commit message
- Capitalize the commit message
  - This is as simple as it sounds. Begin all subject lines with a capital letter.
    - **For example:**  ```Fix typo in User model```
    - **Instead of:**  ```fix typo in user model```
- Do not end the subject line with a period
  - Trailing punctuation is unnecessary in subject lines. 
    - **For example:**  ```Refactor error handling```
    - **Instead of:**  ```Refactor error handling.```
- Describe what was done
  - Don't write a git commit subject line that talks about what you did, or what you are doing.
  - For Example: 
    - ```Fixed onboard page swipe crash```  -- Don't
    - ```Fixing onboard page swipe crash```  -- Don't
    - ```Fix onboard page swipe crash```   -- Do
  - A properly formed Git commit subject line should always be able to complete the following sentence:
    - If applied, this commit will **_your subject line here_**:
      - If applied, this commit will ```fix onboard page swipe crash```
      - If applied, this commit will ```remove deprecated methods```
    - Notice how this doesn’t work for the other non-imperative forms:
      - If applied, this commit will *~~fixing onboard page swipe crash~~*
      - If applied, this commit will *~~removed deprecated methods~~*

- The commit body must not contain more than 72 characters per line.
- The commit subject or body must not contain Emojis.


## MR Guidelines
- The change is as small as possible.
- The MR must include Before and After screenshots if UI changes are made.
- Clear title and description explaining the relevancy of the contribution.
- Description includes any steps or setup required to ensure reviewers can view the changes you’ve made (for example, include any information about feature flags).
- Always review code before committing it
- Name your sub branches by convention
  - Use a consistent naming convention for your feature branches to identify the work done in the branch. 
  - These are all good branch names:
       ``` - fix-onboard-screen-crash
           - add-author-profile
           - feature/app-analytics
           - bug/profile-button-editing
  

## Explaining git concepts
In this exercise, you will write an explanation for various git concepts.

- Don't assume any prior knowledge of git: imagine you are explaining these concepts to a brand new software developer. Because of this, try not to use jargon.
- Write full, complete prose. Bullet points can be useful, but not what we're after for this module.
- Test the explanation. Try your explanation on a non-technical friend before submitting it. <br>

We want explanations for:

### git: 
- Git is an Open Source Distributed Version Control System. Now that’s a lot of words to define Git. 
- Why is it needed? To ensure there are no code conflicts between the developers. Also, since projects change often, git allows developers to revert and go back to an older version of the code.

### repository: 
- Git stores information about the project’s progress on a repository. 
- A repository has commits to the project or a set of references to the commits called heads.
All this information is stored in the same folder as the project in a sub-folder called .git and will mostly be hidden by default in most systems.
### remote :
- A remote in Git is a common repository that all team members use to exchange their changes. 
- In most cases, such a remote repository is stored on a code hosting service like GitHub or on an internal server.
- In contrast to a local repository, a remote typically does not provide a file tree of the project's current state. Instead, it only consists of the .git versioning data.
### branching:
- Branching is a feature available in most modern version control systems.
- Branching in other VCS's can be an expensive operation in both time and disk space. In Git, branches are a part of your everyday development process. 
- Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes. 
- This makes it harder for unstable code to get merged into the main code base, and it gives you the chance to clean up your future's history before merging it into the main branch.
### merging: 
- Merging is a common practice for developers using version control systems. 
- Whether branches are created for testing, bug fixes, or other reasons, merging commits changes to another location.
- To be more specific, merging takes the contents of a source branch and integrates them with a target branch. 
- In this process, only the target branch is changed. The source branch history remains the same.
### merge conflicts: 
- Merge conflicts may occur if competing changes are made to the same line of a file or when a file is deleted that another person is attempting to edit.
- A merge conflict usually occurs when your current branch and the branch you want to merge into the current branch have diverged. 
- That is, you have commits in your current branch which are not in the other branch, and vice versa.
### the 3 git states:
 - modified:
    - Git views untracked and modified files similarly. Untracked means that the file is new to your Git project.
    - Modified means that the file has been seen before, but has been changed, so is not ready to be snapshotted by Git. Modification of a file occurs in your working directory.
 - staging:
    - When a file becomes staged, it's taken into the staging area. 
    - This is where Git is able to take a snapshot of it and store its current state to your local repository. 
    - This area is also known as the Index.
 - committed:
    - Committed means that Git has officially taken a snapshot of the files in the staging area, and stored a unique index in the Git directory.
    - The terms snapshotted and committed are very similar. The significance of being committed is that you can now revert back to this project's current state at any time in the future.

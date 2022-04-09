1. Develop using branches
	• Create a new branch for every task / small feature / bug fix.
	• Feature
	• Bugfix
	• Release
		• Example: feature-jj-add-testing-module
2. Perform these tasks frequently
	• Pull updates from the main branch into your current branch: git pull origin master/branch
	• Resolve any merge conflicts that may result from the above Structure and branch workflows to fit the project
3. Commit early and often.
4. Do not commit or push directly to the master branch.
5.  Write good, clear commit messages
	• Make sure everyone understands the reason for your change. Start with a Header of ~50 characters describing the change. In the body of the message, define the reason for the change and how it is different from previous versions. Use command words in the present tense for consistency with Git messages. Aim to be as clear and concise as possible. Everyone will benefit from being able to easily determine if they are reverting to the right file.Explain the why, not the what, in your commit message.
6. Use .gitignore File
	• You can avoid following types of files 
	• Files with sensitive information like configuration files, production passwords, etc.
	• Files with temporary information like log files 
	• Compiler code such as obj and dll files etc 
	• Do not commit dependencies, use a useful build/dependency tool.
		• Examples:
			• Maven for Java
			• Npm for node apps
			• Bower for JavaScript
			• NuGet for .NET
7. Merge/Pull Request
	• Publish branch
	• Create a detailed pull/merge request for code review and merge to master
8. Create tag for production deployment.
	1. Example: v1.0.1
	• Given a version number MAJOR.MINOR.PATCH, increment the:
		• MAJOR version when you make incompatible code changes,
		• MINOR version when you add functionality in a backwards compatible manner, and
		• PATCH version when you make backwards compatible bug fixes.
		• Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.
Stash, don’t commit, unfinished
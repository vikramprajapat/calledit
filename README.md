# calledit


Permission denied: If you get an error like “permission denied,” you may not have write access to the repository. Contact the repository owner/admin to delete the branch or grant you permissions.
Branch reappears: If the branch keeps coming back:
Check for open pull requests tied to the branch. Go to the “Pull requests” tab on GitHub, find any PRs for the branch, and close them. GitHub may restore the branch if a PR is open.
Check if CI/CD pipelines or automated processes (e.g., GitHub Actions) are recreating the branch.
Protected branch: If the branch is protected, you can’t delete it until protection is removed:
Go to the repository’s “Settings” tab.
Under “Branches,” find “Branch protection rules.”
Locate the rule for the branch and click “Edit” or “Delete.”
Save changes, then try deleting the branch again.
Default branch: If it’s the default branch (e.g., main), you must first set a new default branch:
In “Settings” > “Branches,” under “Default branch,” click “Change default branch.”
Select a new default branch and confirm.
Then delete the old default branch.
Ensure permanent deletion:
Once deleted, the branch is gone from the remote repository unless recreated by a process or user. GitHub doesn’t keep deleted branches unless they’re part of a pull request or tag.
If you suspect someone/something is recreating the branch, check the repository’s “Actions” tab or audit logs (if you have admin access) to identify the source.
If you’re still unable to delete the branch, share specific error messages or details about your setup (e.g., is it a protected branch, part of a PR, or tied to a specific workflow?), and I can dig deeper.


About READMEs
You can add a README file to your repository to tell other people why your project is useful, what they can do with your project, and how they can use it.

In this article
About READMEs
Auto-generated table of contents for README files
Section links in README files and blob pages
Relative links and image paths in README files
Wikis
Further reading
About READMEs
You can add a README file to a repository to communicate important information about your project. A README, along with a repository license, citation file, contribution guidelines, and a code of conduct, communicates expectations for your project and helps you manage contributions.

For more information about providing guidelines for your project, see Adding a code of conduct to your project and Setting up your project for healthy contributions.

A README is often the first item a visitor will see when visiting your repository. README files typically include information on:

What the project does
Why the project is useful
How users can get started with the project
Where users can get help with your project
Who maintains and contributes to the project
If you put your README file in your repository's hidden .github, root, or docs directory, GitHub will recognize and automatically surface your README to repository visitors.

If a repository contains more than one README file, then the file shown is chosen from locations in the following order: the .github directory, then the repository's root directory, and finally the docs directory.

When your README is viewed on GitHub, any content beyond 500 KiB will be truncated.

If you add a README file to the root of a public repository with the same name as your username, that README will automatically appear on your profile page. You can edit your profile README with GitHub Flavored Markdown to create a personalized section on your profile. For more information, see Managing your profile README.

Auto-generated table of contents for README files
For the rendered view of any Markdown file in a repository, including README files, GitHub will automatically generate a table of contents based on section headings. You can view the table of contents for a README file by clicking the  menu icon at the top left of the rendered page.

Screenshot of the README for a repository. In the upper-left corner, the "Table of contents" dropdown menu (list icon) is expanded.

Section links in README files and blob pages
You can link directly to any section that has a heading. To view the automatically generated anchor in a rendered file, hover over the section heading to expose the  icon and click the icon to display the anchor in your browser.

Screenshot of a README for a repository. To the left of a section heading, a link icon is outlined in dark orange.

For more detailed information about section links, see Section links.

Relative links and image paths in README files
You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:

[Contribution guidelines for this project](docs/CONTRIBUTING.md)
GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. The path of the link will be relative to the current file. Links starting with / will be relative to the repository root. You can use all relative link operands, such as ./ and ../.

Your link text should be on a single line. The example below will not work.

[Contribution
guidelines for this project](docs/CONTRIBUTING.md)
Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.

Wikis
A README should contain only the necessary information for developers to get started using and contributing to your project. Longer documentation is best suited for wikis. For more information, see About wikis.

Further reading

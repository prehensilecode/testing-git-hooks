# testing-git-hooks
Testing out Git hooks.

From [Atlassian tutorial](https://www.atlassian.com/git/tutorials/git-hooks):

## Scope of Hooks
Hooks are local to any given Git repository, and they are _not_ copied over 
to the new repository when you run `git clone`. And, since hooks are local,
they can be altered by anybody with access to the repository.

This has an important impact when configuring hooks for a team of developers.
First, you need to find a way to make sure hooks stay up-to-date amongst
your team members. Second, you can’t force developers to create commits that
look a certain way—you can only encourage them to do so.

Maintaining hooks for a team of developers can be a little tricky because the
`.git/hooks` directory isn’t cloned with the rest of your project, nor is it
under version control. A simple solution to both of these problems is to
store your hooks in the actual project directory (above the `.git`
directory). This lets you edit them like any other version-controlled file.
To install the hook, you can either create a symlink to it in `.git/hooks`,
or you can simply copy and paste it into the `.git/hooks` directory whenever
the hook is updated.
 

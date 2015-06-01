# Commit Hashtags

Commit messages tell the on-going story of a project. Each commit message is a chapter of the project's story, with a short title that summarises the changes and then a few descriptive sentences or paragraphs explaining each change.

Commit hashtags extend [existing commit messages](http://git-scm.com/book/ch5-2.html) with contextually meaningful hashtags, inspired by [Twitter hashtags](http://en.wikipedia.org/wiki/Hashtag). The commit hashtag/s appear after the commit message and provide a method of grouping and extracting meaningful data from commit messages.

Commits which contain commit hashtags can be analysed by scanning the git log and aggregating the commit hashtag usages over time periods, per author, or with other commit metrics.

## Sample git commit mesages

`Add new class to analyse raw image data #TDD`

`Refactor image processing logic #TDD #Refactor`

## Analysing git messages

The git commits can be analysed to retrieve development statistics. This can be done through the `git log` command in the console. Sample analysis commands are;

`git log --oneline --grep="#TDD"`
 
`git log --oneline --author="James Lawler" --grep="#TDD"`
 
`git log --oneline --author="James Lawler" --after="2015-01-01" --grep="#TDD"`

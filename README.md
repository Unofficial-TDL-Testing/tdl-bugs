# Unofficial 'The Dead Linger' Bug Tracker
Unofficial bug tracking project for '[The Dead Linger](http://www.thedeadlinger.com)' by
[Sandswept Studios](http://www.sandswept.net).

## Reporting a Bug

1. Select the issues tab on the sidebar
2. Search for an existing issue for your bug
  - If you find one comment there rather than creating a new report
3. Click 'New Issue' and add a descriptive title and labels for it
4. Referencing the [labels](#labels) section below set the correct labels for the issue
5. Set appropriate Milestone (generally the next build)
6. Copy and paste the [issue template](issue-template) into the issue description and fill out all the fields
7. Click 'Submit new issue'
8. Be sure to track your issue (subscribing on GitHub is a good idea) so that you can provide addition information as
needed

### Labels

Labels are a great way to get information about issues at a glance and makes it easier to search for issues that have a
specific severity or status. Using the following guide add the appropriate labels to the issue:

1. Add a severity label
```
Minor - A bug that is barely noticeable and/or has little effect on gameplay
Major - A bug that breaks immersion and/or has a large impact on gameplay
Critical - A game breaking bug which prevents player progress
Crash - A severe bug resulting in the game crashing or freezing
```

2. For issues specific to the Watertower utility add the 'watertower' tag

3. If the developers already know about the issue (such as if it was originally reported on the Sandswept forums) you
may need to add a status tag, see the [report lifecycle](#report-lifecycle) section for more information
```
In Progress - The developers have acknowledged the bug and stated that a fix is being worked on or will be in the next build
Verify - A potential fix has been released and should be verified before the issue is closed
```

### Issue Template

```
**Description:**

**Build:**

**Bug Type:**

**Severity:**

**Frequency:**

**Forum Link:**

**Steps to Reproduce:**

1. {FIRST STEP}

**External Links:**

- {IMAGE/VIDEO LINK}

**Crash Report/Error Message:**

{TEXT OR IMAGE LINK}

**Logs:**

- {PASTEBIN LINK}

**Additional Info:**

{ANYTHING USEFUL}
```

#### Issue Template Explanations

**Description:** A quick and clear description of the bug  
**Build:** State what build the bug was initially discovered in (eg. 16, 16ba, 17 ect.)  
**Bug Type:** Whether its a graphical bug, gameplay bug, crash, etc.  
**Severity:** How severe the issue is, should match the tag you added to the issue  
**Frequency:** State how often the bug occurs, this can mean during general play or just when performing a specific
in-game action depending on the bug  

- *Rare:* A bug that occurs no more than a couple times during extended play
- *Uncommon:* A bug that occurs once in a while
- *Frequent:* A bug that occurs very often but is not constant or every time for a specific action
- *Always:* A bug that is always present, or occurs every time a specific action is performed

**Forum Link:** A link to the associated bug report on the Sandswept or Steam forums, if it doens't exist create one  
**Steps to Reproduce:** State word by word how to reproduce the issue, if unknown then give a description of what you
were doing when the bug occurred even if doing the same actions did not reproduce it  
**External Links:** Images/Videos and so forth go here, imgur.com and youtube.com are useful resources for hosting
images and videos respectively  
**Crash Report/Error Message:** If it supplies a crash report or displays an error message add it here, text or images
are both acceptable  
**Logs:** If logs are available supply a link here, use pastebin.com or another website to store it rather than pasting
the entire log here  
**Additional Info:** Any additional info you can think off really, including more in depth description if applicable  

#### Example

```
**Description:** When picking up an axe, the game immediately crashes.

**Build:** 18c

**Bug Type:** Crash

**Severity:** Crash

**Frequency:** Always

**Reported Status:** Y

**Steps to Reproduce:**

1. When in game find an axe
2. Pick it up
3. Le crash

**External Links:**

- None

**Crash Report/Error Message:**

TDL.exe has stopped responding! ERROR 1337: OutOfAxesException

**Logs:**

- http://pastebin.com/JfdVDKPn

**Additional Info:**

I cannot chop down trees without an axe and it makes me sad.
```

## Information for Bug Managers

*This section is intended primarily for bug tracker managers who have the power to manage reports but will be useful to
anyone who wants to understand our bug tracking process.*

### Report Lifecycle

1. When a new issue is logged ensure that follows the format described above and update or ask for additional
information as needed. If the issue is determined to be a duplicate or not actually a bug then update it with the
appropriate label and close the issue, be sure to post an explanation of why the issue was closed.
2. If the developers state that they are actively investigating or in the process of fixing an issue then add the `in
progress` label and post a link to the relevant statement from the developers.
3. When the changelog for a build or a statement from a developer indicates that a bug has been fixed add the `verify`
label and post a link to where it is stated that the bug has been fixed.
4. If an issue is marked for verification and unclaimed then any tester can assign themselves to the issue and take
responsibility for checking whether the bug has been fixed. Posting proof of verification would be ideal but is not
required.
5. When the bug has been verified as resolved then the assigned tester should close the issue.
6. In the case that a bug turns out to have only been partially fixed or otherwise was incorrectly closed the existing
issue should be reopened rather than logging a new one.

### Feature Lifecycle

1. When a feature for an upcoming build is announced or appears in a changelog it should be added to the appropriate
feature file in the versions directory with an empty checkbox `[ ]`. However we should probably only do this for the
next build or two as the plans for builds beyond that may change at any time. This can be done directly in the GitHub
web editor for convenience, try to add a descriptive commit message rather than using the default.
2. Once a build is released any tester may add their name next to it to claim it for testing. For the sake of
thoroughness it is perfectly acceptable if more than one tester claims a feature.
3. If any bugs are encountered log issues for them and report them on the Sandswept forums following the instructions
above.
4. When a feature has been thoroughly tested mark it as completed by placing an 'x' in its checkbox `[x]`.

### Updating README.md

If you think that something could be improved in this README file or have suggestions to improve our process you can
submit a pull request to update it. A pull request can be done as follows:

1. Create a new branch using the dropdown labled `Branch: master` and entering a descriptive name in the textbox.
2. On your branch (not master!) edit the README.md file, either in the GitHub web editor or locally on your computer if
you know how. For help with formatting refer to
[GitHub's help pages](https://help.github.com/articles/markdown-basics/).
3. When your changes are ready press the green button next to the branch dropdown while on your branch. From this screen
you can review your changes one last time then press `Create Pull Request`.
4. Enter a descriptive title and a good description of what you want to change and why then submit your pull request.
5. Discussion will then happen on the pull request page and if people are satisfied with the change they should create
a comment saying +1 or :+1: to indicate their approval. (This makes it quick and easy to see/count approval.) If you're
not satisfied with a proposed change then please explain why on the pull request so that your concerns can be addressed.
6. Once everyone's concerns have been addressed and you have approval from an organization owner or two or more
Bug Managers/Admins then you can merge the pull request using the provided button (in some cases this may require manual
merging, contact [jpeg](https://github.com/jpeg) if you need help).
  - NOTE: This is just a quickly thrown together approval process. We should discuss how we want it to work in as a
  community at some point. If you have an idea you can always submit a pull request!
7. After merging double check the README.md file in master to ensure that the merge went as expected, sometimes
something may go wrong and need to be fixed.

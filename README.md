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

**Reported Status:** [Y]/[N]

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

**Steps to Reproduce:** State word by word how to reproduce the issue, if unknown then give a description of what you
were doing when the bug occurred even if doing the same actions did not reproduce it  
**External Links:** Images/Videos and so forth go here, imgur.com and youtube.com are useful resources for hosting
images and videos respectively  
**Crash Report/Error Message:** If it supplies a crash report or displays an error message add it here, text or images
are both acceptable  
**Logs:** If logs are available supply a link here, use pastebin.com or another website to store it rather than pasting
the entire log here  
**Reported Status:** Whether or not the issue has been reported on the Sandswept forums  
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

## Report Lifecycle

This section is intended primarily for bug tracker managers who have the power to manage reports but will be useful to
anyone who wants to understand our bug tracking process.

TODO

---
date: 2019-04-17
title: Spot Coverage Gaps Using the Gutter
topics:
  - testing
author: pwe
subtitle: Let the IDE help you spot coverage gaps in your testing.
seealso:
  - title: Viewing Code Coverage Results
    href: "https://www.jetbrains.com/help/pycharm/viewing-code-coverage-results.html"
  - title: Configuring Code Coverage Measurement
    href: >-
      https://www.jetbrains.com/help/pycharm/configuring-code-coverage-measurement.html
thumbnail: ./thumbnail.png
video: "https://youtu.be/HQ_bqOBXZ5w"
---

Note: Code coverage is available for PyCharm with Pro subscription.

Writing tests for your code is good, but how do you know when you've done enough testing? "Code coverage", via the [coverage package](https://pypi.org/project/coverage/), combines your tests and the execution of your code to see and report what spots get hit.

PyCharm makes this easy to set up. You just run the Run with Coverage action, for example by clicking the button in the toolbar, and PyCharm runs your tests
with the bundled `coverage.py` (or you can use a _coverage_ that is installed in your project interpreter.)

Once coverage runs, you'll get a tool window showing a filesystem-like view of your project with statistics at each level.

But better yet, and the subject of this tip, your editor's gutter will be color-coded with coverage information: green for covered and red for not covered. If you checked the preference for "branch coverage", the gutter decorations will include branches in your code.

Those gutter decorations are not just visual: click a line in the gutter to get a popup with some statistics.

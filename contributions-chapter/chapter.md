# Contributions for DESOSA 2017

This chapter outlines the conributions that each of the teams in the course were able to make to their open-source project. Contributions have been categorized and are presented below:

## Language/Typo/Link fixes
- This [pull request](https://github.com/elastic/kibana/pull/10709) fixes some language mistakes in the `FAQ.md` file of Kibana's documentation.
- This [pull request](https://github.com/elastic/kibana/pull/10714) fixes a typo in the `kbn_server.js` file in the Kibana project.
- This [pull request](https://github.com/elastic/kibana/pull/10715) fixes a broken link in Kibana's `CONTRIBUTING.md` file.

## Bug fixes
- This Kibana [issue](https://github.com/elastic/kibana/issues/9108) depicts a problem in Safari where exporting data would lead to a display of the JSON in the browser instead of a download action (labeled P3: nice to have bug-fixes). Investigation led to finding out it was a [bug](https://bugs.webkit.org/show_bug.cgi?id=102914) in Webkit that has recently been fixed. An upgraded version of Safari (10.1) should thus solve the problem. Workaround possibilities exist, but these are unreliable. Hence, this analysis was posted in the [issue](https://github.com/elastic/kibana/issues/9108) on Github along with a suggesion for the Kibana team to wait for the new version of Safari. For more info on the download library please visit this [link](eligrey/FileSaver.js#12).

## Technical debt
- the Kibana team is trying to remove unnecessary usage of the [Lodash](https://lodash.com) library. There are multiple methods in Lodash that can easily be replaced by very similar native ES6 methods. This [pull request](https://github.com/elastic/kibana/pull/10746) removes some of the unnecessary lodash methods.
- After analyzing Kibana using tools to look for technical debt, some syntax errors were found in the test code. There was an incorrect `.json` file and a quoting issue with a `.sh` file. This [pull request](https://github.com/elastic/kibana/pull/10747) solved these issues.

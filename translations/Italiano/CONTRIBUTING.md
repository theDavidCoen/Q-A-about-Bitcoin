# Guide to contributing

This book is developed collaboratively and openly, here on GitHub. I accept comments, contributions and corrections from everyone.

## Current Project STATUS
**Second edition IN PROGRESS**

You have access to the English version of the book. I will add draft and commit any new material.

## License and attribution

All contributions must be properly licensed and attributed. If you are contributing your own original work, then you are offering it under a CC-BY license (Creative Commons Attribution). *You are responsible for adding your own name or pseudonym in the [Acknowledgments](Acknowledgments.md), as attribution for your contribution.*

If you are sourcing a contribution from somewhere else, it must carry a compatible license. The book will initially be released under a CC-BY-NC-ND license which means that contributions must be licensed under open licenses such as MIT, CC0, CC-BY, etc. Contributions under a "share-alike" or GPL license are not compatible with the CC-BY-NC-ND license and therefore cannot be accepted. You need to indicate the original source and original license, by including a markdown comment above your contribution. For example, for this CONTRIBUTING.md file, I used part of the Andreas M. Antonopoulos CONTRIBUTING.md file available [here](https://github.com/lnbook/lnbook/blob/develop/CONTRIBUTING.md).

```
<!-- 
Source: https://github.com/lnbook/lnbook/blob/develop/CONTRIBUTING.md
License: CC-BY-SA
Added by: @aantonop
-->
```
## Translations

You will find translation folders inside [translations](tree/master/translations). If you don't see your language, please follow these steps:

1. Login with your GitHub account or create one now
2. Fork the `Q-A-about-Bitcoin` repository. Create your language folder under [translations](tree/master/translations) if not available. Copy the files and folders from the English version and paste them inside your language folder. Work on your fork. In particular you can clone it to your local computer with `git clone https://github.com/ADD_YOUR_GIT_USER_NAME_HERE/Q-A-about-Bitcoin.git`
IF the language folder is already available and it has already files inside, please work on the single markdown, one at the time. DO NOT put a question mark in the file name.
3. If possible, please do one pull request PER markdown file, to avoid large merges. Edit the markdown file where you want to make a change or create a new markdown file in the [messy](/messy) directory if you're not sure where your contribution might fit.
4. Edit [Acknowledgments](Acknowledgments.md) and add your own name to the list of contributors under the Contributions section. Use your name, or a GitHub username, or a pseudonym.
5. Commit your change. Include a commit message describing the correction.
6. Submit a pull request against the Q-A-about-Bitcoin repository.
7. I currently use one line per sentence to make reviewing of pull requests and diffs easier. Make sure to follow this style guide and **turn off auto formatting** of your editor.

## Contributing with new material or corrections

Do the steps above without creating language folders but working on the already available files. Edit the markdown file where you want to make a change or create a new markdown file in the [messy](/messy) directory if you're not sure where your contribution might fit.

## Contributing with an issue

If you find a mistake and you're not sure how to fix it, or you don't know how to do a pull request, then you can file an Issue. Filing an Issue will help me see the problem and fix it.

Create a [new Issue](https://github.com/theDavidCoen/Q-A-about-Bitcoin/issues/new/choose) now!

## Heading styles, anchors and references

Adjust heading style in each section as follows:

1. Only the chapter/section should be level 2, everything else should be level 3 and below (level 1 is the book title itself). Each markdown file should start with a "##" heading.
2. Headings should be all lower case, except for first letter, proper nouns and acronyms. "What is Bitcoin?", "What is the blockchain?" etc.
3. Acronyms are spelled out, capitalized, with the acronym in parentheses (e.g. "Hash Time-Locked Contract (HTLC)"). Once you have spelled out an acronym in one heading, we can keep it as an acronym only in subsequent headings.
4. No period at the end of headings. Question mark if it is a question.
5. Headings should be followed by a blank line.
6. Often it seems useful to link to a webpage / url. Since the research community figured out that every year about 50% of all outstanding url's become invalid we encourage you to use the wayback machine / Web Archive at: http://web.archive.org and provide a link to a saved copy of the web page.

Complete Example:

```
QUESTION 1-What is Bitcoin?.md
## What is Bitcoin? ##

This is the intro paragraph.

As we saw in [intro](/intro.md), the intro paragraph is superb!

```



## Thanks

With your help, this will be a great second edition that can help thousands of users get started and eventually embrace the Bitcoin revolution. Thank you!

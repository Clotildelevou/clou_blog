# Contributing to the blog

This blog is a public space for anyone willing to contribute. The topic
of the article can be anything as the article respects the rules specified 
later. This document details the contributing procedure for the blog and
how to write a post. If you have any question, feel free to ask with
the Gitlab issue tracker or by email to the blog maintainers.

## Writing rules

Here are some rules to follow when writing a post:
- The post must:
  - be written in English for in depth posts.
  - use the Markdown syntax
  - respect the UTF-8 encoding
  - have a title, a summary, a date, tags and a requirement section for
  technical subjects
  - have an author following the format *Firstname Lastname*
  - use tags that are already used in the blog or create new ones if necessary
  - be within a 80 columns limit

- The post must not:
  - contain any personal information except the author's name
  - contain any advertisement for a product or service
  - be political or religious in nature
  - contain any offensive content (racism, sexism, transphobia, etc.)
  - plagiarize any content from another source (Except if the source is cited
    and the content is used with the author's permission depending of the
    content license)
  - encourage illegal activities or promote illegal content
  - pornographic or sexually explicit content
  - advocate for violence
  - denigrate others work or personnalities
  - use any language that is not respectful

- The post can:
  - contain links to external resources

Please note that the blog is a public space. The content of the posts is the
responsibility of the author. The blog moderation team reserves the right to
remove any post that does not respect these rules and the right to ban any user
who does not comply with these rules.

## Add a new post into the blog

The blog is hosted on a Github repository. You can contribute by
first creating an issue an then a merge request.

Here's a quick guide to create a merge request for the blog:
- Make a new issue with the tag `post` and the title of your post with the "POST"
  prefix on the Gitlab issue tracker.
- Make a new merge request with the issue number in the title. This should be
  made automatically by clicking on the button "Create a branch"
  in the right sidebar under "Development".
- Clone the repository and switch to your new branch.
- Move to the `sources` folder.
- Create a new post using the hugo command
  `hugo new posts/author-YYYY-MM-DD-<post-name>.md`,
  - `author` - Your name or nickname
  - `YYYY` - Year of the post
  - `MM` - Month of the post
  - `DD` - Day of the post
  - `post-name` - Short name of the post (use underscore instead of spaces)
- The file should start with the following header (See `demo_post.md` for an
  example):
  ```
  ---
  title: "<post-title>"
  date: <post-date>
  author: "<Firstname Lastname>"
  summary: "<summary of the article>"
  # Mind this option bellow! If let to `false` you will not see your article.
  draft: false
  ---
  ```
- Write your post in [Markdown](https://www.markdownguide.org/).
- We advice you to follow the ["one sentence per line"](https://sive.rs/1s) rule
- Check that your post is valid by running `hugo server` and checking that the
  post is displayed correctly.
- Check if your post respect the writing rules.
- Commit your changes and push them to the repository.

Don't forget to preview your post before submitting it.

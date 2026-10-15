# smallnodeapp — what changed, in plain words

Newest first.

## October 2026

**smallnodeapp #5: the change log catches up on entries it missed** · [PR #5](https://github.com/travis-horton/smallnodeapp/pull/5) · merged 26.1015.0728 · v1.0.2
- Behind the scenes: the robot that writes this file after each change now also writes in any earlier finished change it missed, oldest first, with a "recorded late" note when it is more than an hour late. If GitHub won't answer one of its lookups, it skips only that one, records the newest change anyway, and fills the gap on a later run.

**smallnodeapp #4: the project's past, written down** · [PR #4](https://github.com/travis-horton/smallnodeapp/pull/4) · merged 26.1010.1210 · v1.0.1
- Behind the scenes: the history file now covers the whole project, from its first version to 26.1010, not just today's changes.

**smallnodeapp #3: security update for the web server** · [PR #3](https://github.com/travis-horton/smallnodeapp/pull/3) · merged 26.1010.1150 · v1.0.0
- Behind the scenes: brought the web server that hands out the site's page up to its makers' patched version, replacing 2 separate automatic update requests. Known security warnings go from 8 to none, and the page loads the same as before.
  Behind the scenes: the project now keeps a plain-language history that adds an entry by itself each time a change is merged.

## June 2019

**A footer that doesn't show** · [commit](https://github.com/travis-horton/smallnodeapp/commit/a138050) · merged 19.0613.1812 · v0.1.2
- Behind the scenes: tried adding a footer line meant to appear on every page, written in PHP, a language some web servers run to build pages. This server doesn't run PHP, so the footer never appears; the page still shows only "Hello, world!".

**Getting ready for a hosting service** · [commits](https://github.com/travis-horton/smallnodeapp/commits/master?since=2019-06-12&until=2019-06-12) · merged 19.0612.1753 · v0.1.1
- **[Start instructions for the host](https://github.com/travis-horton/smallnodeapp/commit/25b7608)** · merged 19.0612.1733
  Behind the scenes: added the one-line file a hosting service such as Heroku reads to know how to start the app, and a list of things the project should never store (downloaded packages, logs, a private settings file).
- **[Choosing the port](https://github.com/travis-horton/smallnodeapp/commit/e5c9c9a)** · merged 19.0612.1741
  Behind the scenes: three quick tries, six minutes apart, at how the app picks the port (the numbered door it listens on). It ended up using the port a hosting service hands it, and 8080 when there isn't one.
- **[Settings file](https://github.com/travis-horton/smallnodeapp/commit/6513cfe)** · merged 19.0612.1753
  Behind the scenes: added a small library that reads private settings from a local file, "to see what it does"; the app now prints its port setting when it starts.

**Hello, world** · [commit](https://github.com/travis-horton/smallnodeapp/commit/2b6b046) · merged 19.0611.1923 · v0.1.0
- New: a tiny web app: a server, listening on port 8080, that hands out one page saying "Hello, world!", plus a script that prints "Hello, world! (In the console this time!)" in the browser's developer tools.

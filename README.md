# gerrit Tools

A few scripts to make code review via [Gerrit Code Review](http://gerrit.googlecode.com) easier for developers.

## gerrit-cherry-pick

This is a script that allows you to cherry-pick a particular patch from Gerrit, so that it can be reviewed easily. It comes with Gerrit, but is included here because Gerrit 2.1.1.1 does not yet contain support for the `--latest` option.

## gerrit-setup

Gerrit-setup will attempt to convert a repository cloned from github to use Gerrit as the origin instead.

## git-review

Git-review is a wrapper script to make creating, reviewing, and approving Gerrit changes very simple. In the simplest case, you can have an entire Git workflow that looks like this for people creating a new changeset:

    git review push

And looks like this for people reviewing someone else's changeset:

    git review 123
    rake && git review approve
    git review reset

You may find it helpful to alias `gr` to `git review`.

## Contributing

Feel free to fork and send a pull request if you think you've improved anything.

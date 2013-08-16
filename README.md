glazier-github-repositories
===========================

This card lists repositories that the current user owns.

## Adding to glazier

    # in `glazier/cards/`
    ln -s your/path/to/glazier-github-repositories github-repositories

    # in `glazier/`
    grunt ingestCards

    # in `glazier/glazier-server/`
    bundle exec rails console

    # add the Pane to the dashboard of your choosing
    db = Dashboard.where(repository: 'emberjs/ember.js').first
    db.add_pane('glazier-github-repositories')


## Running Tests
  grunt autotest

  # view in browser
  open dist/dev/github-repositories/test.html

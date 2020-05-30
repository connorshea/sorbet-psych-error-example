# README

An example for this issue: https://github.com/sorbet/sorbet/issues/3125

To reproduce the issue, just clone this repo, run `bundle install`, and then `bundle exec srb init`.

I used Ruby 2.6.5, but it probably fails on most other versions as well. (You'll need Ruby 2.5+ for Rails 6 to work)

The repo was created with the following commands:

- `rails new sorbet-psych-error-example --skip-action-cable --skip-active-storage --skip-action-text --skip-action-mailbox`
  - Disables a few extra features just because they're not relevant to the issue.
- `cd sorbet-psych-error-example/`
- `bundle add sorbet`

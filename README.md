# YADAs

YADA (Yet Another Data migration App)  is a collection Ruby on Rails gems for handling migrating data into your Ruby on Rails apps. With data migration we mean tasks that change data on your database but not the database schema, for example back-filling a column to which you are going to add a `NOT NULL` constraint.

YADA migration is a gem for having scheduled data migrations ran in between your schema migrations in organized manner for keeping separate databases in sync (for example in multi-developer setup) or to run all database tasks with one command for small scale app.

YADA task is a gem for creating data migration tasks that can be run whenever and removed whenever.

YADA core is the muscle behind these that takes care of splitting records into batches that will be updated on ActiveJob runner.

## Installation

```
bundle add yada_migration yada_task
bin/rails generate yada_core:install
```

## Usage

TODO: Write usage instructions here

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/zharrowed/yadas.

# Rails::Fullcalendar
## Installation

Add this line to your application's Gemfile:

```ruby
gem 'rails-fullcalendar'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install rails-fullcalendar

## Usage

```
//= require moment
//= require fullcalendar
```
(turbolinks)
Then in you application.js file add the following:

```
function eventCalendar() {
  return $('#calendar').fullCalendar({
    header: {
        left: 'prev,next today myCustomButton',
        center: 'title',
        right: 'month,agendaWeek,agendaDay'
    }
  });
};
$(document).on('turbolinks:load', eventCalendar);
```

If you have disabled turbolinks just add to application.js:

```
$('#calendar').fullCalendar({});
```


## Development

This first version has not been tested as it only includes the assets, future versions will include tests

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/robertosante/rails-fullcalendar. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Rails::Fullcalendar project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/rails-fullcalendar/blob/master/CODE_OF_CONDUCT.md).

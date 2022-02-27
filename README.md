# my_framework

Following this [tutorial](https://launchschool.medium.com/growing-your-own-web-framework-with-rack-part-1-8c4c630c5faf)

## Notes

Rack is used with Ruby web frameworks and provides an interface that allows a Ruby app to communicate with a web server.

The command to start a Rack web application on port 9595: `bundle exec rackup config.ru -p 9595`

The rack application that we use in the rackup file (here `config.ru`) must be a Ruby object that responds to the method `call(env)`

The call method always returns an array of three elements:
- a status code (string)
- headers (a hash)
- response body (needs to be an object that responds to each method--therefore an array works)

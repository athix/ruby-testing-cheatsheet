# Testing Rails Applications with RSpec

This assumes that you're using the latest versions of Rails and RSpec. If you
are on older versions, focus on getting to the latest versions first.

## TL;DR

DO USE:

* Integration Tests
  * `spec/requests`
  * `spec/system`
* Unit Tests
  * `spec/helpers`
  * `spec/jobs`
  * `spec/mailers`
  * `spec/models`
  * `spec/validators`

DON'T USE:

* `spec/controller`
  * For API controllers, use request specs
  * Otherwise, use system specs
* `spec/views`
  * Use system specs
* `spec/routing`
  * Use system specs
* `spec/features`
  * Use system specs

## Integration Tests

Always test using the domain language of the user. For request specs, this means
always sending requests to the API endpoint, and making assertions directly
against the response. For system specs, this means interacting using the GUI,
and making your assertions directly against the GUI. Do **NOT** make any
assertions against the database, e.g. asserting that a model was changed by a
request. That is the responsibility of your unit tests.

### Request Specs

TODO

### System Specs

TODO

## Unit Tests

TODO

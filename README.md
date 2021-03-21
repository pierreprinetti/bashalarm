# Bashalarm

A collection of Bash functions supposedly useful for testing.

I have coded this for making sure my website is online.

## Use

Change the test array:

```
declare -a tests=(
	"response_code GET https://www.github.com 301"
	"response_contains GET https://github.com 'Built for developers'"
)
```

Then run:

```
./bashalarm || send_notification
```

The exit code is greater than 0 if there are failing tests.

Note that `send_notification` is not part of this repository.

# Bashalarm

Change the test array:

```
declare -a tests=(
	"response_code GET https://www.github.com 301"
	"response_contains GET https://github.com 'Built for developers'"
)
```

Then run:

```
./bashalarm
```

The exit code is greater than 0 if there are failing tests.

# Run shell commands

## Decription

This action provides a base image to run shell commands.
It has a pre-installed set of tools, such as :

- openssh-client

## Example:

```
action "My Action" {
  uses = "docker://simonvadee/action-shell:latest"
  # uses = "simonvadee/actions/shell@master"
  args = [
      "ls -l",
      "echo 'test'"
  ]
}
```

## Environment variables

NONE

## Secrets

NONE

## Required arguments

NONE

## Optional arguments

NONE

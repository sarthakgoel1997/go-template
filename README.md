# go-template

## Introduction
An initial template repository for a Go project

## Running the code
``` shell
go run main.go
```

## Structure

``` shell
$ tree
.
|____go.mod         # dependencies
|____LICENSE		
|____Makefile       # make test, fmt….
|____README.md
|____.gitignore
|____.circleci	    # CI configuration
|____main.go	    # main function
|____pkg            # Components
|____.golangci.yml  # golangci-lint Configuration
```

## Components Example
Calculator Component is the Interface exposed to the user. 
+ It gives the user an encapsulated calculator object which receives operands.

Operator Component is the internal library for the Calculator. 
+ It gives the calculator some operator objects which implements the real calculations.

Please edit it for your projects.

## CI Steps
1. Install dependency and tools (golangci-lint)
2. Run unit tests
3. Code static analysis and format check

## Tools 
1. Language: Golang@1.21.3
2. Package Management Tool: go mod
3. Code Format Tool: golangci-lint@1.55.2
4. Static Analysis Tool: golangci-lint@1.55.2
5. CI Tool: CircleCI@2.1

## Getting Started

You have to prepare tools with make.

``` shell
make tools
```

Also, you can run lint, format and test with make before making a pull request.

``` shell
# test 
make test

# lint
make lint

# format
make format
```

## Contributing
+ [pull_request_template.md](./pull_request_template.md)
+ [issue_template.md](./issue_template.md)

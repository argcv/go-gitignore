# go-gitignore

## Changes from Original

This is a fork of the original `sabhiram/go-gitignore` repository with the following updates:

**Why this fork?** The original repository is no longer actively maintained. The original author used Git tag `1.0.2` instead of `v1.0.2` (required by Go module rules). These updates ensure compatibility with modern Go versions, fix deprecation warnings, and maintain the project's usability for current Go developers.

### Module & Dependencies
- **Module name**: Changed to `github.com/argcv/go-gitignore`
- **Go version**: Upgraded to 1.23
- **Testify**: Upgraded to v1.10.0

### Code Modernization
- Replaced deprecated `ioutil` functions with `os` equivalents:
  - `ioutil.ReadFile` → `os.ReadFile`
  - `ioutil.WriteFile` → `os.WriteFile`
- Fixed code formatting in `ignore.go` comments
- Reorganized imports in test files

### Repository Updates
- Updated `go.mod` and `go.sum` with new dependencies
- Added `/vendor/` directory to `.gitignore` to exclude vendored dependencies
- Removed `version_gen.go` file as it's no longer needed

## Original README

[![Build Status](https://travis-ci.org/sabhiram/go-gitignore.svg)](https://travis-ci.org/sabhiram/go-gitignore) [![Coverage Status](https://coveralls.io/repos/github/sabhiram/go-gitignore/badge.svg?branch=master)](https://coveralls.io/github/sabhiram/go-gitignore?branch=master)

A gitignore parser for `Go`

## Install

```shell
go get github.com/sabhiram/go-gitignore
```

## Usage

For a quick sample of how to use this library, check out the tests under `ignore_test.go`.

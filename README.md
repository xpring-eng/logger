# `@xpring-eng/logger`

![NPM version badge](https://img.shields.io/npm/v/@xpring-eng/logger)

A TypeScript logger utilizing Log4JS.

## Usage

This enum was designed to remove "magic numbers" of HTTP status codes from our codebases. Instead, you can access a human-readable alias for any numeric HTTP status code using `HttpStatus.Status`.

```ts
import HttpStatus from '@xpring-eng/http-status'

console.log(HttpStatus.NotFound) // Logs 404
```

## Status Codes

All official HTTP status codes are included, as well as popular status codes used by NGINX, Microsoft, Twitter, etc.

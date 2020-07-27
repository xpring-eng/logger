# `@xpring-eng/logger`

![NPM version badge](https://img.shields.io/npm/v/@xpring-eng/logger)

A TypeScript logger utilizing Log4JS.

## Usage

This logger library was designed to be a zero-config way to use Log4JS using the `xpring-eng` defaults for logging.

```ts
import createLogger from '@xpring-eng/logger'

// The log level you pass to createLogger()
// will be the level of logs that actually get emitted.
const logger = createLogger('INFO')

export default logger
```

## Log Levels

There are multiple valid log levels:

```ts
// Log Levels
//
// OFF    Designates no log messages should be shown
// MARK   Designates an event that will almost always be logged. Useful for temporary logging.
// FATAL  Designates very severe error events that will presumably lead the application to abort.
// ERROR  Designates error events that might still allow the application to continue running.
// WARN   Designates potentially harmful situations.
// INFO   Designates informational messages that highlight the progress of the application at coarse-grained level.
// DEBUG  Designates fine-grained informational events that are most useful to debug an application.
// TRACE  Designates finer-grained informational events than the DEBUG.
// ALL    Designates all log events should be shown (equivalent to TRACE)

enum LogLevel {
  OFF = 'OFF',
  MARK = 'MARK',
  FATAL = 'FATAL',
  ERROR = 'ERROR',
  WARN = 'WARN',
  INFO = 'INFO',
  DEBUG = 'DEBUG',
  TRACE = 'TRACE',
  ALL = 'ALL',
}
```

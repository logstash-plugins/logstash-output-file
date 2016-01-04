## 2.2.3
  - Rename Dir.exists? to Dir.exist? to fix deprecation warning
  - Allow setting dir and file permissions

## 2.2.1
 - Fixed specs to not depend on pipeline ordering

## 2.2.1
 - Fixed Time specs

## 2.2.0
 - Add support for codec, using **json_lines** as default codec to keep default behavior.
   Ref: https://github.com/logstash-plugins/logstash-output-file/pull/9

## 2.1.0
 - Add create_if_deleted option to create a destination file in case it
   was deleted by another agent in the machine. In case of being false
   the system will add the incomming messages to the failure file.

## 2.0.0
 - Plugins were updated to follow the new shutdown semantic, this mainly allows Logstash to instruct input plugins to terminate gracefully,
   instead of using Thread.raise on the plugins' threads. Ref: https://github.com/elastic/logstash/pull/3895
 - Dependency on logstash-core update to 2.0

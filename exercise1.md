In the Rust ecosystem, linting is typically done with rust-clippy, which provides all the standard linting features that exist in other languages. The Rust compiler itself is also very strict with formatting, so that many style rules which are usually enforced by linters in other languages are enforced at the compiler level in Rust.

Test functions in Rust are written similarly to JavaScript, by composing special test functions and marking them with a modifier. Tests are run via cargo, the all-in-one tool that most Rust programmers use for developing and building programs. The command “cargo build” compiles the program into a binary executable.

For CI, the cargo documentation suggests Travis CI, GitLab CI, and builds.sr.ht.

A decision of whether to self-host or host in the cloud would be based on the scope of the project as well as platform-specific needs. The cargo tool takes special steps to compile for systems other than the one on which it is running, e.g. compiling high-quality Windows builds on Linux or vice-versa, which would likely make cloud options a good choice for automated building on many standardized platforms. Rust compilation can also be quite intensive and take a long time for large programs, which would make it difficult to use with cloud options. In the end it would depend on the specific details of the project.

# Issues Found Before Static Code Analysis Fixes

## 1. Pylint Issues

| S.No | Issue | Description |
| --- | --- | --- |
| 1 | Missing docstrings | Module and function docstrings were missing. |
| 2 | Naming convention violations | Names did not follow the recommended conventions. |
| 3 | Mutable default argument | A mutable object was used as a default argument value. |
| 4 | Bare except statement | `except:` used without specifying an exception type. |
| 5 | Unnecessary comparison with None | Comparison with `None` done using `==` instead of `is`. |
| 6 | Unused variables and imports | Variables and imports were declared but never used. |
| 7 | Use of eval() | `eval()` can execute arbitrary expressions. |
| 8 | Missing final newline | The file did not end with a newline character. |
| 9 | Formatting and readability issues | Code formatting reduced readability. |

## 2. Bandit Security Issues

| S.No | Test ID | Issue | Description |
| --- | --- | --- | --- |
| 1 | B110 | Try-except-pass | Exceptions were silently ignored. |
| 2 | B307 | Use of eval() | Potential arbitrary code execution. |
| 3 | B324 | Use of MD5 | Weak cryptographic hash algorithm. |
| 4 | B311 | Use of random | `random` used for security-sensitive values. |
| 5 | B605 | Use of os.system() | Potential command execution risk. |
| 6 | B105 | Hardcoded password | A password or secret was hardcoded in the source. |

## 3. Flake8 Issues

| S.No | Issue | Description |
| --- | --- | --- |
| 1 | Unused imports | Imported modules were never used. |
| 2 | Long lines | Lines exceeded the recommended maximum length. |
| 3 | Bare except statement | `except:` used without specifying an exception type. |
| 4 | Unused variables | Variables were assigned but never used. |
| 5 | Unnecessary comparison with None | Comparison with `None` done using `==` instead of `is`. |
| 6 | Missing final newline | The file did not end with a newline character. |

## Summary of Issues by Tool

| Tool | Focus Area | Number of Issues |
| --- | --- | --- |
| Pylint | Code quality and style | 9 |
| Bandit | Security vulnerabilities | 6 |
| Flake8 | Formatting and PEP 8 compliance | 6 |
| **Total** |  | **21** |

## Conclusion

Static analysis identified code-quality, formatting, and security issues in the original gym membership program. The code was improved, and the analysis tools were run again to verify the changes.

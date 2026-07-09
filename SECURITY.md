# Security Policy

## Supported Version

| Version | Supported |
| ------- | --------- |
| v1.x    | Yes       |

## Security Model

Fitness Tracker v1 is a static, local-first web app.

- There is no backend server.
- There is no authentication system.
- There is no cloud database.
- User data is stored locally in the browser.

## Reporting a Vulnerability

If you discover a bug or security issue, please open a GitHub issue in this repository.

Do not include private personal data in public issue reports.

## Data Safety Notes

Because the app stores progress in localStorage, clearing browser data may erase saved progress.

Future versions may add export/import backup support.

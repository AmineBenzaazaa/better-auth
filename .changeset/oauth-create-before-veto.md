---
"better-auth": patch
---

Fix OAuth sign-up crashing with a `TypeError` when a `user.create.before` database hook returns `false`. The callback now aborts with a `FAILED_TO_CREATE_USER` error, matching email sign-up.

### Hi there 👋

I am a open-source security researcher finding and reporting security vulnerabilities affecting various open-source projects

### My CVEs

Note: I use huntr.dev as a CNA (Certificate Numbering Authority), so CVE numbers are allocated close to one another.

CVE Count: 19

| CVE-ID | Summary | Project | Report Link | My Thoughts |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| CVE-2021-3838 | Pending Fix  |  [dompdf/dompdf](https://www.github.com/dompdf/dompdf) | Pending Fix | Pending Fix |
| CVE-2021-3902 | Pending Fix  |  [dompdf/dompdf](https://www.github.com/dompdf/dompdf) | Pending Fix | Pending Fix |
| CVE-2021-3874 | Path Traversal via link expansion in PDF exports  |  [bookstackapp/bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/ac268a17-72b5-446f-a09a-9945ef58607a/ | Exploiting path traversals in Laravel apps require a slightly different proof-of-concept than usual! |
| CVE-2021-4119 | Improper Access Control + SQL Wildcard injection leads to dumping of user details |  [bookstackapp/bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/135f2d7d-ab0b-4351-99b9-889efac46fca/ | This one required whitebox techniques! |
| CVE-2021-4026 | (Improper Access Control) Attachments of draft pages can be accessed via API |  [bookstackapp/bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/c6dfa80d-43e6-4b49-95af-cc031bb66b1d/ | Always check the APIs available! |
| CVE-2021-3944 | Login CSRF via password reset links |  [bookstackapp/bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/65551490-5ade-49aa-8b8d-274c2ca9fdc9/ | - |
| CVE-2021-4089 | (Improper Access Control) Asset Model Cloning form endpoint can be accessed without "view" and "create" permissions |  [snipe/snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/19453ef1-4d77-4cff-b7e8-1bc8f3af0862/ | There is an assumption that forms do not require access control checks. However, cloning and duplication forms definitely need at least "view" access control checks to prevent leak of data. |
| CVE-2021-4075 | POST-based SSRF in Slack Webhooks as admin | [snipe/snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/4386fd8b-8c80-42bb-87b8-b506c46597de/ | - |

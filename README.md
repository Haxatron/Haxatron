### Hi there 👋

I am a open-source security researcher finding and reporting security vulnerabilities affecting various open-source projects

If you would like me to take a look at you repository (for free), you can contact me at haxatron1@gmail.com with the name of your repository. Security issues will be reported via [huntr.dev](https://huntr.dev/policy/)

Factors I take into account when deciding whether to review:

- Ease of Installation (Dockerfiles are great!)
- Number of stars / forks (should be 2000+)

### My CVEs

Note: I use huntr.dev as a CNA (Certificate Numbering Authority), so CVE numbers are allocated close to one another.

CVE Count: 22

|  CVE-ID | Summary | Project | Report Link | My Thoughts |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| CVE-2021-43856 | XSS via other dangerous filetypes (XML/HTM) |  [wiki.js](https://www.github.com/requarks/wiki) | https://github.com/Requarks/wiki/security/advisories/GHSA-rhpf-929m-7fm2 | - |
| CVE-2021-43855 | XSS via bypassing SVG sanitization with user-controlled MIME type  |  [wiki.js](https://www.github.com/requarks/wiki) | https://github.com/Requarks/wiki/security/advisories/GHSA-4893-pj5w-3hq9 | - |
| CVE-2021-3838 | Pending Fix  |  [dompdf](https://www.github.com/dompdf/dompdf) | Pending Fix | Pending Fix |
| CVE-2021-3902 | Pending Fix  |  [dompdf](https://www.github.com/dompdf/dompdf) | Pending Fix | Pending Fix |
| CVE-2021-3874 | Path Traversal via link expansion in PDF exports  |  [bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/ac268a17-72b5-446f-a09a-9945ef58607a/ | Exploiting path traversals in Laravel apps require a slightly different proof-of-concept than usual! |
| CVE-2021-3906 | Uploaded Files with broken extensions will be served as Content-Type: text/html leading to XSS / Phishing vector |  [bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/f115bdf5-c06b-4627-a6fa-ba6904a43ba3/ | This one required a bit of experimentation - and of course, source-code review |
| CVE-2021-4119 | Improper Access Control + SQL Wildcard injection leads to dumping of user details |  [bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/135f2d7d-ab0b-4351-99b9-889efac46fca/ | I've never heard of SQL wildcard injection before writing this report. This one required source-code review |
| CVE-2021-4026 | (Improper Access Control) Attachments of draft pages can be accessed via API |  [bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/c6dfa80d-43e6-4b49-95af-cc031bb66b1d/ | Always check the APIs available! |
| CVE-2021-3944 | Login CSRF via password reset links |  [bookstack](https://www.github.com/bookstackapp/bookstack) | https://huntr.dev/bounties/65551490-5ade-49aa-8b8d-274c2ca9fdc9/ | - |
| CVE-2021-4089 | (Improper Access Control) Asset Model Cloning form endpoint can be accessed without "view" and "create" permissions |  [snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/19453ef1-4d77-4cff-b7e8-1bc8f3af0862/ | There is an assumption that forms do not require access control checks. However, cloning and duplication forms definitely need at least "view" access control checks to prevent leak of data. |
| CVE-2021-4075 | POST-based SSRF in Slack Webhooks as admin | [snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/4386fd8b-8c80-42bb-87b8-b506c46597de/ | - |
| CVE-2021-4130 | CSRF to disrupt request tracking | [snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/ccf073cd-7f54-4d51-89f2-6b4a2e4ae81e/ | - |
| CVE-2021-3931 | CSRF to modify custom fields| [snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/03b21d69-3bf5-4b2f-a2cf-872dd677a68f/ | - |
| CVE-2021-3938 | Self-XSS in bulk-audit logs| [snipe-it](https://www.github.com/snipe/snipe-it) | https://huntr.dev/bounties/198a0d67-9189-4170-809b-0f8aea43b063/ | Sadly, could not escalate any further due to stringent CSRF checks. |
| CVE-2021-3992 | (Improper Access Control) Previewing invoices do not have fine-grained access control checks | [kimai2](https://www.github.com/kevinpapst/kimai2) | https://huntr.dev/bounties/a0c438fb-c8e1-40cf-acc6-c8a532b80b93/ | Very interesting finding. DAC and RBAC checks were usually implemented on viewing invoices. However, it was observed that only RBAC checks were enforced in invoice previews |
| CVE-2021-3963 | CSRF to delete invoice templates | [kimai2](https://www.github.com/kevinpapst/kimai2) | https://huntr.dev/bounties/3abf308b-7dbd-4864-b1a9-5c45b876def8/ | - |
| CVE-2021-3976 | CSRF related to "duplicate" action | [kimai2](https://www.github.com/kevinpapst/kimai2) | https://huntr.dev/bounties/0567048a-118c-42ec-9f94-b55533017406/ | - |
| CVE-2021-4033 | CSRF to disrupt invoice tracking + modify search favorites | [kimai2](https://www.github.com/kevinpapst/kimai2) | https://huntr.dev/bounties/e05be1f7-d00c-4cfd-9390-ccd9d1c737b7/ | - |
| CVE-2021-4005 | CSRF to disable 2FA | [firefly-iii](https://www.github.com/firefly-iii/firefly-iii) | https://huntr.dev/bounties/bf4ef581-325a-492d-a710-14fcb53f00ff/ | - |
| CVE-2021-3900 | CSRF to modify rules / rule groups | [firefly-iii](https://www.github.com/firefly-iii/firefly-iii) | https://huntr.dev/bounties/909e55b6-ef02-4143-92e4-bc3e8397db76/ | - |
| CVE-2021-4015 | CSRF related to transactions | [firefly-iii](https://www.github.com/firefly-iii/firefly-iii) | https://huntr.dev/bounties/b698d445-602d-4701-961c-dffe6d3009b1/ | - |
| CVE-2021-41273 | CSRF allows sending test emails and generation of keys | [pterodactyl](https://github.com/pterodactyl/panel) | https://github.com/pterodactyl/panel/security/advisories/GHSA-wwgq-9jhf-qgw6 | - |
### My Interesting Reports (Without CVEs)

| Summary | Project | Report Link | My Thoughts |
| ------------- | ------------- | ------------- | ------------- | 
| One-click RCE in an ElectronJS Application | [google-voice-desktop-app (3rd party)](https://www.github.com/jerrod-lankford/google-voice-desktop-app) | https://huntr.dev/bounties/1e56ac67-6a41-490e-a9d3-6fe154ca3688/ | A good primer to ElectronJS exploitation! |
| Reflected XSS using double-URL encoding | [admidio](https://www.github.com/admidio/admidio) | https://huntr.dev/bounties/b6047e20-c60a-41c3-8fc5-fbe1e47d283e/ | - |
| Reflected XSS fix bypass using triple-URL encoding | [admidio](https://www.github.com/admidio/admidio) | https://huntr.dev/bounties/f502537e-97b3-4f7c-b51c-1d0706b22fd2/ | - |
| (Improper Access Control) Access drafts of restricted pages in the same namespace using conflicting cache names | [dokuwiki](https://www.github.com/splitbrain/dokuwiki) | https://huntr.dev/bounties/eeb1508f-a986-45cb-9aaf-312deb225a84/ | Source code reviews reveal interesting findings. |

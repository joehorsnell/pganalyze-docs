---
title: 'Enterprise Edition: Troubleshooting'
backlink_href: /docs/enterprise
backlink_title: 'pganalyze Enterprise Edition'
---

## Error: License Invalid or Expired

If you see the notice `Error: License Invalid or Expired` when logging into pganalyze,
it means that pganalyze Enterprise Edition wasn't able to verify the `LICENSE_KEY` that
is passed.

**Step 1:** Verify that you are passing `LICENSE_KEY` to the Docker container. Your license
key is identical to the download password that is used to download the image. Reach out
to support in case you don't have your license key available.

**Step 2:** Make sure that the pganalyze container is able to send a HTTPS request to port 443 on `enterprise-license-check.pganalyze.com`, which is needed to verify the license key.

**Step 3:** Try restarting the container, and check whether the same error recurs.

If the error is still occurring, please run `rake enterprise:self_check`, which will return more details like this:

```
$ docker run ... quay.io/pganalyze/enterprise:[version] rake enterprise:self_check

Testing database connection... Success!
Testing Redis connection... Success!
Skipping LDAP test.
Verifying enterprise license... FAILED
  License file exists: No

  ERROR: You need to specify the LICENSE_KEY environment variable
```

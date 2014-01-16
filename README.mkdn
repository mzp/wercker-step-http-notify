# http-notify

Send http request to specified url(a.k.a. webhook)

## Options
### required

 * `url` - Your webhook url

## Passed parameters

 * `result` - result of step. `passed` or not.
 * `type` - type of step. `build` or `deploy`.
 * `application_owner_name`
 * `application_name`
 * `build_url`
 * `git_branch`
 * `started_by`

## Example

Add HOOK_URL as deploy target or application environment variable.

    build:
       after-steps:
          - mzp/http-notify:
              url: $HOOK_URL


---
rank: 223
category_id: box-relay
subcategory_id: null
is_index: true
id: box-relay
type: guide
total_steps: 2
sibling_id: guides
parent_id: guides
next_page_id: ''
previous_page_id: box-relay/start-workflow
source_url: >-
  https://github.com/box/developer.box.com/blob/main/content/guides/box-relay/index.md
---
# Box Relay

[Box Relay][boxrelay] is a workflow automation application that enables Box
power users to automate and accelerate business processes centered
around content. Currently, there are two API [endpoints][workflow] developers
can use with more planned to be released in the future. Both were created to
work directly with [manual start flows][manualstart].

## Required Scopes

The following [scopes][scopes] must be enabled for an application before use of
Box Relay's endpoints.

- [Read all files and folders stored in Box][read]
- [Write all files and folders stored in Box][write]
- [Manage Box Relay][relay]

<Message type='warning'>

Depending on the selected authentication method and enterprise's settings,
your application may require Admin authorization or re-authorization before
successful use of any newly selected scopes.

</Message>

## Rate Limits

Please see our [rate limit guide][ratelimit] for more information.

## Testing

Due to the feature parity, it may be useful to familiarize yourself with
[Box Relay functionality using the Box web app][webapp] before leveraging the
API. As with all API endpoints, we recommend testing via
[developer sandbox environment][sandbox] to eliminate the risk of impacting
production content.

[scopes]: g://api-calls/permissions-and-errors/scopes
[read]: g://api-calls/permissions-and-errors/scopes/#read-all-files-and-folders
[write]: g://api-calls/permissions-and-errors/scopes/#read-and-write-all-files-and-folders
[ratelimit]: g://api-calls/permissions-and-errors/rate-limits/#per-api-rate-limits
[webapp]: https://support.box.com/hc/en-us/articles/360044628853-Creating-and-Running-a-Manual-Start-Workflow
[sandbox]: https://support.box.com/hc/en-us/articles/360043697274-Managing-developer-sandboxes-for-Box-admins
[relay]: g://api-calls/permissions-and-errors/scopes/#manage-box-relay
[boxrelay]: https://support.box.com/hc/en-us/articles/360044196213-Introducing-Box-Relay
[workflow]: https://developer.box.com/reference/resources/workflow/
[manualstart]: https://support.box.com/hc/en-us/articles/360044628853-Creating-and-Running-a-Manual-Start-Workflow
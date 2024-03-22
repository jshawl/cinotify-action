# CI Notify JavaScript action

This action sends an email notification to the specified recipient.

**Motivation**:

- Zero domain/DNS configuration
- No need to give out SMTP credentials
- It Just Works™️

## Inputs

### `to`

**Required** The recipient of the email

### `subject`

Email subject

### `body`

Email body

### `type`

Email body MIME type

### `attachment`

Filename of the attachment

## Outputs

### `status`

"ok" if the notification sent successfully.

## Example usage

```yaml
uses: cinotify/github-action@main
with:
  to: 'example@example.com'
  subject: 'building main'
  body: '<em>This is a notification from GitHub actions.</em>'
  type: 'text/html'
  attachment: 'artifacts.zip'
```

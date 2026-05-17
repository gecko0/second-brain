# Automation Ideas

## Daily Cleanup Task

Run once per day:

1. Fetch recent unread or inbox emails.
2. Classify each email.
3. Apply safe labels.
4. Archive obvious low-value emails.
5. Flag risky decisions for review.
6. Produce a daily summary.

## Possible Categories

- Action required
- Waiting for reply
- Important reference
- Finance
- Travel
- Receipts
- Newsletter
- Notification
- Cold outreach
- Spam
- Unknown

## Safe Actions

- Add labels.
- Mark obvious newsletters as newsletter.
- Archive known low-value notifications.
- Create a review list.
- Summarize inbox changes.

## Risky Actions

- Delete email.
- Unsubscribe.
- Reply automatically.
- Mark as spam.
- Archive ambiguous work or personal email.

## Custom Workflow Sketch

```text
Gmail / Google Workspace
  -> googleworkspace/cli
  -> Codex scheduled task
  -> classify and decide
  -> apply labels/archive/delete only within allowed rules
  -> write daily report
```

## Guardrails

- Default to labeling before deleting.
- Keep a review label for uncertain decisions.
- Auto-delete only when confidence is very high and the sender/pattern is known.
- Log every automated action.
- Prefer archive over delete unless explicitly allowed.


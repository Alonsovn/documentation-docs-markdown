# How to Integrate GitHub with a Discord Channel for PR Notifications

You can integrate GitHub with a Discord channel to send a notification when a pull request (PR) is opened using GitHub Webhooks. Follow these steps:

---

## 1. Create a Discord Webhook

1. Open your Discord server.
2. Navigate to the channel where you want to receive the notifications.
3. Click the **gear icon** to open the channel settings.
4. Go to the **Integrations** tab and click **Create Webhook**.
5. Copy the webhook URL.

---

## 2. Set Up a GitHub Webhook

1. Go to your GitHub repository.
2. Click on **Settings** and then navigate to the **Webhooks** section.
3. Click **Add webhook**.
4. Paste the Discord Webhook URL into the "Payload URL" field.
5. Under "Content type", select `application/json`.
6. In the "Events" section:
   - Choose **Let me select individual events**.
   - Check the **Pull request** event.
7. Save the webhook.

---

## 3. Customize the Payload (Optional)

By default, GitHub sends a payload to the Discord webhook when the specified event occurs. If you want to format the notification message further:

1. Use a server or service (e.g., **Zapier**, **IFTTT**) to intercept and format the message.
2. Process the payload into a more Discord-friendly format.
3. Forward the formatted message to the Discord webhook.

---

## Additional Resources

For more advanced solutions, refer to GitHub's official documentation:

- [Responding to Webhook Events](https://docs.github.com/en/apps/creating-github-apps/writing-code-for-a-github-app/building-a-github-app-that-responds-to-webhook-events)

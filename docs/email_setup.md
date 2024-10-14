# Email Setup in Microsoft Outlook

This guide will help you configure your Hetzner email to work with Microsoft Outlook.

## Prerequisites

- You have a Hetzner email account.
- You have Microsoft Outlook installed on your computer.

## Step-by-Step Setup

1. **Open Outlook**
   - Launch Microsoft Outlook on your computer.

2. **Add Account**
   - Go to **File** > **Add Account**.
   - Enter your Hetzner email address and click **Connect**.

3. **Choose Account Type**
   - Choose **IMAP** or **POP**.
   - **IMAP** is recommended to keep emails synchronized across all devices.

4. **Incoming Server Settings**
   - **IMAP**:
     - Server: `mail.yourdomain.com` (replace `yourdomain.com` with your actual domain)
     - Port: `993`
     - Encryption: `SSL/TLS`
   - **POP**:
     - Server: `mail.yourdomain.com`
     - Port: `995`
     - Encryption: `SSL/TLS`

5. **Outgoing Mail Server (SMTP) Settings**
   - Server: `mail.yourdomain.com`
   - Port: `465` (or `587`)
   - Encryption: `SSL/TLS` or `STARTTLS`

6. **Authentication**
   - Username: Your full email address.
   - Password: Your email password.
   - Make sure **Require logon using Secure Password Authentication (SPA)** is unchecked.

7. **Finish Setup**
   - Click **Next**.
   - Outlook will test the account settings. If successful, click **Finish**.

## Troubleshooting

- Make sure your domain's DNS settings include correct **MX** records for email delivery.
- Verify the **username** and **password** are entered correctly.
- Ensure your **firewall** or **antivirus** is not blocking the required ports.

## Notes

- IMAP keeps messages in sync across all devices, while POP downloads them to one device.
- For further assistance, check Hetzner's email documentation or contact their support.

# Computer Engineering Lab: Server Access Guide

Follow these steps to request an account, configure your network, and connect to the lab server.

## 1. Request an Account

1. Fill out the [Request Server Resources Form](https://docs.google.com/forms/d/e/1FAIpQLSfFOzJfnDgjfVuQWXwDcQWGydQRhDzzjRSm2s5Nu7HtcmDoDA/viewform) with your details.
2. Wait for a confirmation email. This email will contain your assigned server `username`, `password`, the `Tailscale IP address`, and an `Invitation Link`.

(_**Note:** You can change your password at any time by running the `passwd` command once you are connected to the server._)

## 2. Configure Network Access

We use Tailscale to manage secure remote access to the lab resources. You will need to install the client on your personal computer.

1. Go to [Tailscale](https://tailscale.com) and create a free personal account.
2. Download and install Tailscale for your operating system:
   - **Windows / macOS:** Download the app from the [Tailscale Download Page](https://tailscale.com/download) and install it.
   - **Linux:** Open your terminal and run the following command:
     ```bash
     curl -fsSL https://tailscale.com/install.sh | sh
     ```
3. Once Tailscale is installed and running, log in to your account.
4. Click the **Invitation Link** from your confirmation email to accept the shared machine and authenticate it to your personal network.

## 3. Connect via SSH

Ensure Tailscale is running on your machine and you are logged in. Open your terminal and run the following command to connect to the server:

```bash
ssh <USERNAME>@<TAILSCALE_IP_ADDRESS>
```

(_**Note:** You can also use [VSCode Remote SSH Extensions](https://github.com/amornthepc/kosen-docs/settings/pages)_)

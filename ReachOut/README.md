<div align="center">

# **ReachOut**

Meet **ReachOut**, the world’s leading open-source AI wearable plugin that lets you stay connected with friends, family, and partners. Simply pair with your contacts and send notifications with phrases like “I miss you” or “Ping [Name],” all hands-free through your Omi device.

<p align="center">
  <img src="https://github.com/user-attachments/assets/834d3fdb-31b5-4f22-ae35-da3d2b9a8f59" alt="Omi" width="49%" />
  <img src="https://github.com/user-attachments/assets/fdad4226-e5ce-4c55-b547-9101edfa3203" alt="Image" width="49%" />
</p>

![CleanShot 2025-02-08 at 18 22 23](https://github.com/user-attachments/assets/7a658366-9e02-4057-bde5-a510e1f0217a)

<h3>
[Site](https://omi.me/) | [Download](https://omi.me/download) | [Docs](https://docs.omi.me/) | [Buy Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) | [Buy Omi Glass Dev Kit](https://www.omi.me/glass)
</h3>

</div>

---

## ReachOut Plugin

**ReachOut** is a community-built plugin that lets your Omi device listen for personalized phrases like **“I miss you [Name]”** or **“Ping [Name] [Message]”**, and send notifications to paired contacts instantly.

This plugin uses a simple webhook to process voice input and send replies through Omi notifications, giving you a seamless hands-free connection experience.

### How It Works

1. Omi streams real-time speech to your webhook endpoint.  
2. The plugin detects trigger phrases such as **“I miss you”** or **“Ping [Name]”**.  
3. The spoken phrase is transcribed and processed.  
4. A notification is sent to the paired contact with the appropriate message.  

You can customize this behavior by editing the webhook logic on your server.

### Quick Deploy

Deploy your own version easily:

```bash
git clone https://github.com/rojansapkota/omi-plugins
cd reachout
pip install -r requirements.txt
uvicorn main:app --reload

Then copy your server URL (e.g., `https://your-domain.com/webhook`) into the **Omi App** webhook field.

---

## Example Response

> **You:** "I miss you Alex"  
> **ReachOut:** "Alex, [Your Name] misses you!"

> **You:** "Ping Alex What's up bro"  
> **ReachOut:** "[Your Name] says: What's up bro!"

---

## License

This plugin is released under the **MIT License**, following the spirit of openness in the Omi ecosystem.

---

## Contributions

- Join the [Discord](http://discord.omi.me) community.  
- Build your own [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).
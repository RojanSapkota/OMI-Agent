<div align="center">

# **omi**

Meet Omi, the world’s leading open-source AI wearable that captures conversations, gives summaries, action items and does actions for you. Simply connect Omi to your mobile device and enjoy automatic, high-quality
transcriptions of meetings, chats, and voice memos wherever you are.

<p align="center">
  <img src="https://github.com/user-attachments/assets/834d3fdb-31b5-4f22-ae35-da3d2b9a8f59" alt="Omi" width="49%" />
  <img src="https://github.com/user-attachments/assets/fdad4226-e5ce-4c55-b547-9101edfa3203" alt="Image" width="49%" />

</p>

![CleanShot 2025-02-08 at 18 22 23](https://github.com/user-attachments/assets/7a658366-9e02-4057-bde5-a510e1f0217a)

<h3>

[Site](https://omi.me/) |   [Download](https://omi.me/download)   | [Docs](https://docs.omi.me/) | [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) | [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

</h3>

</div>

## Omi Agent Plugin

Omi Agent is a community-built plugin that lets your Omi device listen for trigger phrases like **“Omi”**, understands your question, and respond naturally.

This plugin uses a simple webhook to process voice input and send replies through Omi notifications, giving you a hands-free conversational experience.

### How it works

1. Omi streams real-time speech to your webhook endpoint.  
2. The plugin detects trigger phrases such as **“Omi”**.  
3. The spoken question is transcribed and sent for processing.  
4. A short, relevant reply is generated and sent back to Omi.  

You can customize this behavior by editing the webhook logic in your server.

### Quick Deploy

You can deploy your own version easily with:

```bash
git clone https://github.com/rojansapkota/omi-plugins
cd omi-agent
pip install -r requirements.txt
uvicorn main:app --reload
```

Then copy your server URL (e.g. `https://your-domain.com/webhook`) into the **Omi App** webhook field.

---

## Example Response

> **You:** "Omi, What's the Capital of USA"  
> **Omi:** "The capital of the United States of America is Washington, D.C. (short for District of Columbia)."

---

## License

This plugin is released under the **MIT License**, following the spirit of openness in the Omi ecosystem.


## Contributions

- Join the [Discord](http://discord.omi.me).
- Build your own [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).
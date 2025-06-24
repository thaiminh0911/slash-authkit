---
icon: telegram
---

# For Telegram

{% hint style="info" %}
Currently, for Telegram, you can use **AppVerify Code API** to send OTP codes to users via [**AVCBot**](https://t.me/AppVerifyCode_bot).
{% endhint %}

{% hint style="warning" %}
* To obtain **Chat ID** for verifying Telegram users, you need to ask them to start [**AVCBot**](https://t.me/AppVerifyCode_bot) so that **AppVerify Code** can identify the user according to [**Telegram's Official Documentation**](https://core.telegram.org/bots/#how-are-bots-different-from-users). Then, instruct them to retrieve the **Chat ID** from the message sent by **AVCBot** after they start the bot.
* If you use this API on a Telegram dApp, you only need to ask users to start the bot, as their **Chat ID** is already provided to the application when they running the dApp.
{% endhint %}

{% openapi-operation spec="avcapi-telegram" path="/api/telegram/otpVerification" method="post" %}
[OpenAPI avcapi-telegram](https://cdn.jsdelivr.net/gh/thaiminh0911/avcapi-file@latest/openapi-specs/avcapi-telegram.yaml)
{% endopenapi-operation %}

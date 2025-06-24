---
icon: envelope-open-text
---

# For Email

{% hint style="info" %}
Currently, for Email, you can use **AppVerify Code API** to send OTP codes.
{% endhint %}

{% hint style="danger" %}
**AppVerify Code API** currently uses only one email address to send messages to users: a**ppverifycode@gmail.com**. Any other email addresses are fraudulent.
{% endhint %}

{% openapi-operation spec="avcapi-email" path="/api/email/otpVerification" method="post" %}
[OpenAPI avcapi-email](https://cdn.jsdelivr.net/gh/thaiminh0911/avcapi-file@latest/openapi-specs/avcapi-email.yaml)
{% endopenapi-operation %}

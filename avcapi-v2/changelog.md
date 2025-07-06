---
icon: arrows-rotate
---

# Changelog

{% hint style="info" %}
**AppVerify Code API v2** has not been released yet. The expected launch date is Dec**ember 12, 2025**. You can experience its Beta version when a new announcement is made.
{% endhint %}

<mark style="color:green;">`NEW`</mark> [Use **`X.509`** certificates in **AppVerify Code API v2**](#user-content-fn-1)[^1]

* Public **`X.509`** Certificate ([`.avc-pubcert`](#user-content-fn-2)[^2]): Used to authenticate API request actions.
* Private **`X.509`** Certificate ([`.avc-privcert`](#user-content-fn-3)[^3]): Used to manage applications on **AVCManager**.

<mark style="color:green;">`NEW`</mark> Some API endpoints will be added

* `/api/tg/captcha`: Captcha verification via **AVCBot.**
* `/api/url/tg` : Verify Telegram users by using a redirect URL to **AVCBot** and confirming their identity.
* `/api/url/email`: Verify whether that email belongs to the person by requesting them to access the confirmation URL in the email.

<mark style="color:green;">`NEW`</mark> : Use an additional MySQL Database server as the second server.

<mark style="color:green;">`NEW`</mark> : New module created to make it easier to use **AppVerify Code API v2** for **Python**.

<mark style="color:purple;">`CHANGE`</mark> Modify some API endpoints

* `/api/telegram/otpVerification` ⇒ `/api/tg/otp`
* `/api/email/otpVerification` ⇒ `/api/email/otp`&#x20;
* `/api/getData` ⇒ ∅[^4]

<mark style="color:purple;">`CHANGE`</mark> Modify request parameter components to API endpoints

* `authkey` (Param) ⇒ `Authkey` (Header).
* `chatid` (Param) ⇒ `ChatID` (Header).
* `email` (Param) ⇒ `Email` (Header).

[^1]: We'll have separate documentation on the **`X.509`** certificate information used in the upcoming version of **AppVerify Code API v2**.

[^2]: This is the public **`X.509`** certificate file format created for **AppVerify Code API v2**. You can obtain it by exporting the `.avc-pubcert` file via **AVCManager**.

[^3]: This is the private **`X.509`** certificate file format created for **AppVerify Code API v2**. You can obtain it by exporting the `.avc-privcert` file via **AVCManager**.

[^4]: This API will be migrated to **AVCManager**

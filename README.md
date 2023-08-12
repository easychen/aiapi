# AiAPI


> This is the download and support page for the software

[简体中文](./README-CN.md) | [English](./README.md)

AiAPI is a cross-platform client that converts the Claude website into an OpenAI-compatible API, allowing you to use Claude's 100k context capability in any OpenAI-compatible software. What's even better is that it's free. Thanks to Claude.

# Key Features

1. Cross-platform, works on Mac and Windows
2. Based on Claude2, provides 100k context
3. Compatible with OpenAI API, allowing direct reuse of existing OpenAI tools
4. Supports the CookieCloud browser extension, which can automatically refresh and synchronize cookies

# Download

Please go to the [Releases section of the repository](https://github.com/easychen/aiapi/releases).

# Interface and Functionality

![](images/20230810113755.png)

![](images/20230810113811.png)

![](images/20230810113831.png)


# User Guide

1. Register and log in to your account at <https://claude.ai>.
1. Go to the page <https://claude.ai/chats>, open DevTools by pressing F12, and navigate to Applications → Cookies. Copy the sessionKey.
![](images/20230811122810.png)
1. Paste the sessionKey into the Settings panel and save.
![](images/20230811123049.png)
1. Change the OpenAI API Endpoint to http://127.0.0.1:3456 (if there is a /v1/... at the end, include it as well).
1. You can enter any API Key, but some clients may have format validation. You can use this key: `sk-1234567890ULScvLPEHbT3B3bkFJ34mOSRJSVf9fMWP8UXyw`.
1. ~~This interface currently only supports stream mode, so please enable the "Stream Output" option.~~ added in version 1.0.2


# Compatibility Notes

1. Currently, only the `/v1/chat/completions` endpoint and the `messages` parameter are supported. The model used is `claude-2`.
2. Continuous conversation is supported, and the `messages` parameter will be automatically concatenated.

# Project used AiAPI

1. [book-by-ai](https://github.com/easychen/book-by-ai) : Generate high-quality books with AI

# Disclaimer for Software Usage

1. This software is provided to users for self-installation and use, and the developer does not provide any form of technical support.
2. Users assume all risks and responsibilities when using this software, including but not limited to improper use, data loss, system crashes, etc.
3. The developer does not make any express or implied warranties regarding the applicability, accuracy, reliability, completeness, and timeliness of this software.
4. Users should understand and comply with relevant laws, regulations, and website user agreements when using this software. The developer shall not be liable for any legal disputes or losses caused by the user's violation of relevant provisions.
5. This software may be subject to anti-crawling mechanisms of target websites. Users should bear the risks of account suspension, IP blocking, and other consequences that may arise from using this software.
6. The developer shall not be liable for any direct, indirect, special, incidental, or consequential losses or damages that may result from the user's use of this software, including but not limited to loss of profits, data loss, business interruption, etc.
7. Users are solely responsible for any liabilities arising from their use of this software, including but not limited to infringement of third-party rights, illegal activities, etc.
8. The developer reserves the right to modify, suspend, or terminate this software at any time without prior notice, and shall not be liable for any consequences arising from it.
9. By using this software, users agree to comply with all provisions of this disclaimer. If you do not agree with any part of this disclaimer, please stop using this software immediately.

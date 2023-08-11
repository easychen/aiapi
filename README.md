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
2. Go to the <https://claude.ai/chats> page, open DevTools by pressing F12, navigate to Applications, then Cookies, and copy the sessionKey.
![](images/20230811122810.png)
3. Paste the sessionKey into the Settings panel and save.
![](images/20230811123049.png)
4. Change the OpenAI API Endpoint to http://127.0.0.1:3456 (if there is a /v1/... at the end, include that as well).

# Compatibility Notes

1. Currently, only the `/v1/chat/completions` endpoint and the `messages` parameter are supported. The model used is `claude-2`. `Stream` mode only.
2. Continuous conversation is supported, and the `messages` parameter will be automatically concatenated.


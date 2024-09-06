+++
title = "3. CORS Proxy URL"
weight = 3
+++


Since our [Notion to Markdown website](https://notion-to-md.bamidev.com/) is 100% running on Github Static Pages, we **WILL NOT** save any of your information, your information always stay in your browser, all the requests will be called directly from YOUR browser.


Unfortunately, this kind of request is [violate Notion CORS policy and won’t be support](https://github.com/makenotion/notion-sdk-js/issues/96#issuecomment-852542180), but that’s ok, we will use a CORS Proxy as a middle man to bypass this policy.


To use the **free CORS Proxy**, we input our free CORS Proxy URL.


(Optional part) For convenient, I’ve add a free proxy note.


When click, it will auto fill in [`https://cors-anywhere.herokuapp.com/`](https://cors-anywhere.herokuapp.com/) and open a new tab.


![image.png](/images/002-ii-level-1-notion-to-md/001-1-setup-notion-integration/004-2-setup-notion-page/10-193341-image.png)


![image.png](/images/002-ii-level-1-notion-to-md/001-1-setup-notion-integration/004-2-setup-notion-page/10-831229-image.png)


On the new tab, we will click “Request temporary access…” to allow us to use this free CORS Proxy.


![image.png](/images/002-ii-level-1-notion-to-md/001-1-setup-notion-integration/004-2-setup-notion-page/10-751784-image.png)


**DISCLAIMER:** 

1. **CORS Proxy is a middle man, means it can read all your requests & responses credentials. So choose a safe CORS Proxy to use, or built your own for the highest security protection.**
2. In this tutorial, we’ll use a **Free CORS Proxy URL** for the highest convenient and **accept the risk of losing our NOTION credentials (with request & response too).**
3. But to be honest I’m not afraid at all, because we’ve already **limit** our **Notion token permissions** to **Read content** with **No user information**, also the **Notion URL is a published page** (already public). So even in the worst case when we actually lose **our Notion credentials (with request & response)**, the hacker **cannot update nor delete** **anything, can it can only read my public and selected pages.**
4. If you’re still afraid about the security, you can use **your own CORS Proxy URL** or your **trusted CORS Proxy URL**, you’re very welcome to do so.
5. The only time we use this **CORS Proxy** is when we **click “Convert”** to get Notion page information, **no any other features/actions will use this CORS Proxy.**

	![image.png](/images/002-ii-level-1-notion-to-md/001-1-setup-notion-integration/004-2-setup-notion-page/10-520608-image.png)



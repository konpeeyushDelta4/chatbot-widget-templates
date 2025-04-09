### Dark Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 0 0% 6%;
  --yourgptChatbotSurfaceColorHsl: 0 0% 6%;
  --yourgptChatbotTextColorHsl: 0 0% 80%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 80%;
  --yourgptChatbotBotMessageBgColorHsl: 0 0% 8%;
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 80%;
  --yourgptChatbotUserMessageBgColorHsl: 0 0% 8%;
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 80%;
}

.ygpts-widgetBtn {
  background-color: transparent !important;
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 100%, 0.1);
  border: 1px solid hsla(0, 0%, 100%, 0.1);
}

.ygpts-widgetBtn:hover {
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 100%, 0.2);
  border: 1px solid hsla(0, 0%, 100%, 0.2);
}

/* if you want Glassmorphism effect on widget body */
.ygpts-frame {
  background-color: hsla(0, 0%, 10%, 0.45);
  backdrop-filter: blur(13px);
}

/* If you want to make your avatar in header round */
.ygc-avatar {
  border-radius: 9999px;
  overflow: hidden;
}
```

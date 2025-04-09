### Light Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```

.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 0 0% 100%;
  --yourgptChatbotSurfaceColorHsl: 0 0% 100%;
  --yourgptChatbotTextColorHsl: 0 0% 10%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 10%;
  --yourgptChatbotBotMessageBgColorHsl: 0 0% 100%;
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 10%;
  --yourgptChatbotUserMessageBgColorHsl: 0 0% 100%;
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 10%;
}

.ygpts-widgetBtn {
  background-color: transparent !important;
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 0%, 0.1);
  border: 1px solid hsla(0, 0%, 0%, 0.1);
}

.ygpts-widgetBtn:hover {
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 0%, 0.2);
  border: 1px solid hsla(0, 0%, 0%, 0.2);
}

.ygpts-frame {
  background-color: hsla(0, 0%, 90%, 0.5);
  backdrop-filter: blur(16px);
}

/* If you want to make your avatar in header round */
.ygc-avatar {
  border-radius: 9999px;
  overflow: hidden;
}

.refreshIcon,
.closeIcon {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.8) !important;
  transition: all 0.2s ease-in-out;

  &:hover {
    background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.15) !important;
  }
}

.footer{
background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
}

```

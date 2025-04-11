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
  background-color: hsla(0, 0%, 100%, 0.4);
  backdrop-filter: blur(15px);
}

/* If you want to make your avatar in header round */
.ygc-avatar {
  border-radius: 9999px;
  overflow: hidden;
}

.refreshIcon,
.closeIcon,
.languagePickerBtn {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.8) !important;
  transition: all 0.2s ease-in-out;

  &:hover {
    background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.15) !important;
  }
}

.tabItem {
  color: hsl(var(--yourgptChatbotTextColorHsl) / 0.6);
  transition: all 0.2s ease-in-out;
  &:hover {
    color: hsl(var(--yourgptChatbotTextColorHsl));
  }
  &.active {
    color: hsl(var(--yourgptChatbotTextColorHsl));
  }
}

.sectionHeader,
.chatHeader,
.homeHeader {
  box-shadow: 0 1px 17px 1px hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
}

.homeWrapper {
  .homeHeader {
    .homeHeaderCloseBtn,
    .languagePickerBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      transition: all 0.2s ease-in-out;
    }

    .homeHeaderCloseBtn:hover,
    .languagePickerBtn:hover {
      background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.05) !important;
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;
    &:hover {
      background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    }
  }

  .HomeElementLink {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;
    &:hover {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.7) !important;
    }
  }
}

.sessionsWrapper {
  .sessionsList {
    .sessionItem {
      &:hover {
        background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.05) !important;
      }
      .countBox {
        background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
      }
    }
  }
  .startNewConversationBtn {
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl));
    border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
  }
}

.chatContainer {
  .chatBackBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;

    &:hover {
      background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.05) !important;
    }
  }
  .chatMessagesList {
    background-color: hsla(0, 0%, 90%, 0.3);
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
      }
    }
  }
}

.footer {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl));

  .audioRecorderWrapper {
    background-color: transparent !important;
    .audioRecorderButton {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;

      .audioRecorderButtonText {
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.15) !important;
        transition: all 0.2s ease-in-out;

        &:hover {
          border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1) !important;
        }
      }
    }
  }
}
```

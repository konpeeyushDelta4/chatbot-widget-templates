### Dark Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 0 0% 6%;
  --yourgptChatbotSurfaceColorHsl: 0 0% 6%;
  --yourgptChatbotTextColorHsl: 0 0% 90%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 90%;
  --yourgptChatbotBotMessageBgColorHsl: 0 0% 8%;
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 90%;
  --yourgptChatbotUserMessageBgColorHsl: 0 0% 8%;
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 90%;
}

.ygpts-widgetBtn {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 100%, 0.1);
  border: 1px solid hsla(0, 0%, 100%, 0.1);
}

.ygpts-widgetBtn:hover {
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 100%, 0.15);
  border: 1px solid hsla(0, 0%, 100%, 0.15);
}

/* if you want Glassmorphism effect on widget body */
.ygpts-frame {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.45);
  backdrop-filter: blur(13px);

  /* Remove this if you don't want this border  */
  border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
}

/* If you want to make your avatar in header round */
.ygc-avatar {
  border-radius: 9999px;
  overflow: hidden;
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
  border-bottom: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
}

.chatContainer {
  .boxOuter2 {
    .boxOuter {
      .box {
        border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
      }
    }
  }
}

.languagePickerBtn {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.7) !important;
  transition: all 0.2s ease-in-out;
  &:hover {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1) !important;
  }
}

.languagePickerPopup {
  border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1) !important;
}

.homeWrapper {
  .homeHeader {
    .homeHeaderCloseBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      transition: all 0.2s ease-in-out;
      &:hover {
        background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1) !important;
      }
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;
    &:hover {
      background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1) !important;
    }
  }

  .HomeElementLink {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;
    &:hover {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl/0.7)) !important;
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
    background: hsl(var(--yourgptChatbotPrimaryColorHsl));
    border: 1px solid hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.1);
  }
}

.footer {
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

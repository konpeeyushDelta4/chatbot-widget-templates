### Black & White Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 0 0% 0%;
  --yourgptChatbotSurfaceColorHsl: 0 0% 100%;
  --yourgptChatbotTextColorHsl: 0 0% 0%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 100%;
  --yourgptChatbotBotMessageBgColorHsl: 0 0% 95%;
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotUserMessageBgColorHsl: 0 0% 0%;
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 100%;
}

.ygpts-widgetBtn {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 0%, 0.1);
  border: 1px solid hsla(0, 0%, 0%, 0.1);
}

.ygpts-widgetBtn:hover {
  box-shadow: 1px 1px 16px 3px hsla(0, 0%, 0%, 0.2);
  border: 1px solid hsla(0, 0%, 0%, 0.2);
}

.ygpts-frame {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl));
  border: 1px solid hsl(var(--yourgptChatbotTextColorHsl) / 0.1);
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
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl));
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl));
}

.refreshIcon,
.closeIcon {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  transition: all 0.2s ease-in-out;

  &:hover {
    background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.15) !important;
  }
}

.chatContainer {
  .chatBackBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;

    &:hover {
      background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.15) !important;
    }
  }

  .chatMessagesList {
    background-color: hsl(var(--yourgptChatbotSurfaceColorHsl));
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 1px solid hsl(var(--yourgptChatbotTextColorHsl) / 0.1);
      }
    }
  }
}

.homeWrapper {
  .homeHeader {
    .homeHeaderCloseBtn,
    .languagePickerBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      transition: all 0.2s ease-in-out;
      &:hover {
        background-color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl) / 0.15) !important;
      }
    }

    .languagePickerPopup {
      border: 1px solid hsl(var(--yourgptChatbotTextColorHsl) / 0.1) !important;
      background-color: hsl(var(--yourgptChatbotSurfaceColorHsl));
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    transition: all 0.2s ease-in-out;
    &:hover {
      opacity: 0.9;
    }
  }

  .HomeElementLink {
    color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
    transition: all 0.2s ease-in-out;
    &:hover {
      color: hsl(var(--yourgptChatbotTextColorHsl) / 0.7) !important;
    }
  }
}

.sessionsWrapper {
  .sessionsList {
    .sessionItem {
      &:hover {
        background-color: hsl(var(--yourgptChatbotTextColorHsl) / 0.05) !important;
      }

      .countBox {
        background-color: hsl(var(--yourgptChatbotTextColorHsl) / 0.1);
      }
    }
  }

  .startNewConversationBtn {
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl));
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl));
  }
}

.footer {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl));

  .audioRecorderWrapper {
    background-color: transparent !important;
    .audioRecorderButton {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

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

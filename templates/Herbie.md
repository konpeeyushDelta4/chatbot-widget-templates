![Herbie Theme Preview](https://assets.yourgpt.ai/widget/widget-themes-styles/yourgpt-widget-herbie-theme.png)

[▶️ Watch Video Demo](https://assets.yourgpt.ai/widget/widget-themes-styles/yourgpt-widget-herbie-Fantastic4.mp4)

### Herbie Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
.ygpt-chatbot.ygpt-chatbot {
  /* Fantastic 4 Color Palette */
  --yourgptChatbotPrimaryColorHsl: 200 85% 35%; /* Fantastic 4 Blue */
  --yourgptChatbotSurfaceColorHsl: 0 0% 98%; /* Light Background */
  --yourgptChatbotTextColorHsl: 210 100% 15%; /* Dark Blue Text */
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 100%; /* White Text on Blue */
  --yourgptChatbotBotMessageBgColorHsl: 200 85% 95%; /* Light Blue for Bot */
  --yourgptChatbotBotMessageTextColorHsl: 210 100% 15%; /* Dark Blue Text */
  --yourgptChatbotUserMessageBgColorHsl: 210 100% 97%; /* Very Light Blue for User */
  --yourgptChatbotUserMessageTextColorHsl: 210 100% 15%; /* Dark Blue Text */
  --fantastic4AccentColorHsl: 25 100% 50%; /* Fantastic 4 Orange (The Thing) */
  --fantastic4SecondaryBlueHsl: 195 100% 45%; /* Secondary Lighter Blue */
  --fantastic4GlowColor: rgba(0, 157, 220, 0.5); /* Blue Glow */
}

/* Widget Button - Cosmic Power Style */
.ygpts-widgetBtn {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border: 2px solid white !important;
  border-radius: 50% !important; /* Circular like the F4 logo */
  box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl)),
    0 0 15px var(--fantastic4GlowColor) !important;
  transition: all 0.3s ease-in-out !important;
  transform: translateY(0) !important;

  & img {
    filter: brightness(1.1) contrast(1.1) !important;
  }
}

.ygpts-widgetBtn:hover {
  transform: translateY(-5px) !important;
  box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl)),
    0 0 20px var(--fantastic4GlowColor), 0 0 40px var(--fantastic4GlowColor) !important;
}

.ygpts-widgetBtn:active {
  transform: translateY(0) !important;
  box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl)),
    0 0 10px var(--fantastic4GlowColor) !important;
}

/* Main Chat Frame - Baxter Building Style */
.ygpts-frame {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border-radius: 16px !important;
  box-shadow: 0 4px 20px var(--fantastic4GlowColor),
    0 0 0 1px rgba(0, 157, 220, 0.2) !important;
  overflow: hidden !important;
}

/* Avatar - Rounded for team unity */
.ygc-avatar {
  border-radius: 50% !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  box-shadow: 0 0 10px var(--fantastic4GlowColor) !important;
  overflow: hidden !important;
}

/* Tab Navigation - Cosmic Control Panel */
.ygc-tabs {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border-bottom: 1px solid rgba(0, 157, 220, 0.3) !important;
  padding: 8px 16px !important;

  .ygc-tabItem {
    color: hsl(var(--yourgptChatbotTextColorHsl) / 0.7) !important;
    font-weight: 600 !important;
    padding: 6px 12px !important;
    border-radius: 8px !important;
    transition: all 0.2s ease-in-out !important;
    position: relative !important;

    &:hover {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      background-color: hsl(
        var(--yourgptChatbotPrimaryColorHsl) / 0.1
      ) !important;
    }

    &.active {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      background-color: hsl(
        var(--yourgptChatbotPrimaryColorHsl) / 0.15
      ) !important;

      &:after {
        content: "" !important;
        position: absolute !important;
        bottom: -8px !important;
        left: 50% !important;
        transform: translateX(-50%) !important;
        width: 20px !important;
        height: 3px !important;
        background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        border-radius: 3px !important;
      }
    }
  }
}

/* Headers - Fantastic Leadership */
.sectionHeader,
.chatHeader,
.ygc-homeHeader {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-bottom: none !important;
  font-weight: 600 !important;
  padding: 12px 16px !important;
  box-shadow: 0 2px 10px rgba(0, 117, 177, 0.3) !important;
  position: relative !important;
  overflow: hidden !important;
}

/* Cosmic background effect for headers */
.sectionHeader:after,
.chatHeader:after,
.ygc-homeHeader:after {
  content: "" !important;
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  right: 0 !important;
  bottom: 0 !important;
  background: radial-gradient(
      circle at 30% 50%,
      hsl(var(--fantastic4SecondaryBlueHsl) / 0.6) 0%,
      transparent 60%
    ),
    radial-gradient(
      circle at 70% 50%,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 0%,
      hsl(205 90% 30%) 100%
    ) !important;
  z-index: -1 !important;
}

/* Action Buttons - Reed Richards' Tech */
.refreshIcon,
.closeIcon,
.chatBackBtn,
.homeHeaderCloseBtn,
.languagePickerBtn,
.sessionCloseBtn {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-radius: 8px !important;
  transition: all 0.2s ease-in-out !important;
  padding: 6px !important;

  &:hover {
    background-color: rgba(255, 255, 255, 0.2) !important;
    transform: translateY(-2px) !important;
  }

  &:active {
    transform: translateY(0) !important;
  }
}

/* Help Container - Reed's Lab */
.helpContainer {
  .sectionHeader {
    .helpBackBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      border-radius: 8px !important;
      transition: all 0.2s ease-in-out !important;

      &:hover {
        background-color: rgba(255, 255, 255, 0.2) !important;
      }
    }
  }

  .helpSearchBox {
    .helpSearchInput {
      background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
      border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
      border-radius: 8px !important;
      padding: 10px 16px !important;
      transition: all 0.2s ease-in-out !important;

      &:focus,
      &:hover {
        border-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2) !important;
      }
    }
  }

  .helpList {
    .helpArticleItem,
    .helpCategoryItem {
      border-radius: 8px !important;
      transition: all 0.15s ease-in-out !important;

      &:hover {
        background-color: hsl(
          var(--yourgptChatbotPrimaryColorHsl) / 0.1
        ) !important;
        transform: translateX(4px) !important;
      }
    }
  }
}

/* Language Picker - Universal Translator */
.languagePickerPopup {
  border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
  border-radius: 12px !important;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1),
    0 0 0 1px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2) !important;
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  overflow: hidden !important;
}

/* Chat Messages - Fantastic Communication */
.chatContainer {
  .chatMessagesList {
    background-color: hsl(200 30% 97%) !important; /* Very slight blue tint */
    padding: 16px !important;
  }

  /* Bot Message - Reed Richards Style */
  .botMessage {
    background-color: hsl(var(--yourgptChatbotBotMessageBgColorHsl)) !important;
    color: hsl(var(--yourgptChatbotBotMessageTextColorHsl)) !important;
    border-radius: 16px !important;
    border-top-left-radius: 4px !important;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05),
      0 0 0 1px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.15) !important;
    position: relative !important;
  }

  /* User Message - The Thing Rock Style */
  .userMessage {
    background-color: hsl(var(--fantastic4AccentColorHsl) / 0.1) !important;
    color: hsl(var(--yourgptChatbotUserMessageTextColorHsl)) !important;
    border-radius: 16px !important;
    border-top-right-radius: 4px !important;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05),
      0 0 0 1px hsl(var(--fantastic4AccentColorHsl) / 0.2) !important;
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
        border-radius: 8px !important;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05) !important;
      }
    }
  }
}

/* Home Wrapper - Fantastic HQ */
.homeWrapper {
  .homeQueryBox {
    .homeQueryTextArea {
      background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
      border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
      border-radius: 12px !important;
      padding: 12px 16px !important;
      transition: all 0.2s ease-in-out !important;

      &:focus,
      &:hover {
        border-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2) !important;
      }
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border-radius: 8px !important;
    padding: 8px 16px !important;
    transition: all 0.3s ease-in-out !important;
    transform: translateY(0) !important;
    font-weight: 600 !important;

    &:hover {
      background-color: hsl(195 100% 40%) !important; /* Slightly darker blue */
      transform: translateY(-2px) !important;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1) !important;
    }

    &:active {
      transform: translateY(0) !important;
      box-shadow: none !important;
    }
  }

  .homeElementContainer {
    gap: 16px !important;
    padding: 16px 0 !important;

    .HomeElementLink {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      font-weight: 500 !important;
      transition: all 0.2s ease-in-out !important;

      &:hover {
        color: hsl(var(--fantastic4SecondaryBlueHsl)) !important;
        text-decoration: underline !important;
      }
    }

    .homeElementCard {
      border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.15) !important;
      border-radius: 10px !important;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05) !important;
      transition: all 0.3s ease-in-out !important;
      overflow: hidden !important;

      .ygc-item {
        border: none !important;
        border-radius: 0 !important;
      }

      &:hover {
        transform: translateY(-4px) !important;
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1),
          0 0 0 1px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
      }
    }

    .featuredArticles {
      padding: 16px 8px !important;

      .articleSearchButton {
        border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
        border-radius: 8px !important;
        transition: all 0.2s ease-in-out !important;
        background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;

        &:hover,
        &:focus {
          border-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
          box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2) !important;
        }
      }

      .homeArticleList {
        padding: 8px 0 !important;
      }
    }
  }
}

/* Sessions - Mission Log */
.sessionsWrapper {
  .sessionsList {
    .sessionItem {
      border-radius: 8px !important;
      margin: 4px 0 !important;
      transition: all 0.2s ease-in-out !important;

      &:hover {
        background-color: hsl(
          var(--yourgptChatbotPrimaryColorHsl) / 0.1
        ) !important;
        transform: translateX(4px) !important;
      }

      .ygc-sessionItem-countBox {
        background-color: hsl(
          var(--yourgptChatbotPrimaryColorHsl) / 0.2
        ) !important;
        color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        border-radius: 6px !important;
        font-weight: 600 !important;
      }
    }
  }

  .startNewConversationBtn {
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    border: none !important;
    border-radius: 8px !important;
    padding: 10px 16px !important;
    font-weight: 600 !important;
    transition: all 0.3s ease-in-out !important;
    transform: translateY(0) !important;

    &:hover {
      background-color: hsl(195 100% 40%) !important;
      transform: translateY(-2px) !important;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1) !important;
    }

    &:active {
      transform: translateY(0) !important;
      box-shadow: none !important;
    }
  }
}

/* Footer - Cosmic Power Station */
.ygc-footer {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border-top: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.15) !important;
  padding: 8px !important;

  /* Message Input - Cosmic Communicator */
  .messageInput {
    background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
    border: 1px solid hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3) !important;
    border-radius: 12px !important;
    padding: 12px 16px !important;
    transition: all 0.2s ease-in-out !important;

    &:focus,
    &:hover {
      border-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      box-shadow: 0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2) !important;
    }
  }

  /* Send Button - Flame On! */
  .sendBtn {
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    border-radius: 8px !important;
    transition: all 0.2s ease-in-out !important;

    &:hover {
      background-color: hsl(195 100% 40%) !important;
      transform: scale(1.05) !important;
    }

    &:active {
      transform: scale(1) !important;
    }
  }

  .audioRecorderWrapper {
    background-color: transparent !important;

    .audioRecorderButton {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

      .audioRecorderButtonText {
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        border-radius: 6px !important;
        font-weight: 500 !important;
        transition: all 0.2s ease-in-out !important;

        &:hover {
          background-color: hsl(195 100% 40%) !important;
          transform: translateY(-1px) !important;
        }
      }
    }

    .audioRecorderCloseBtn {
      background-color: hsl(var(--fantastic4AccentColorHsl)) !important;
      border-radius: 50% !important;

      svg {
        fill: white !important;
      }
    }
  }
}

/* Quick Access Button - Molecular Expansion */
.ygc-quickAccessButton {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border: none !important;
  border-radius: 50% !important;
  color: white !important;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15),
    0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl)),
    0 0 15px var(--fantastic4GlowColor) !important;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1) !important;

  &:hover {
    transform: scale(1.1) !important;
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2),
      0 0 0 2px hsl(var(--yourgptChatbotPrimaryColorHsl)),
      0 0 20px var(--fantastic4GlowColor) !important;
  }

  &:active {
    transform: scale(0.95) !important;
  }
}

```

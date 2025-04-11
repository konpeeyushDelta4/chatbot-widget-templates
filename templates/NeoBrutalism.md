### NeoBrutalism Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 0 0% 0%;
  --yourgptChatbotSurfaceColorHsl: 60 100% 99%;
  --yourgptChatbotTextColorHsl: 0 0% 0%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 100%;
  --yourgptChatbotBotMessageBgColorHsl: 120 100% 97%;
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotUserMessageBgColorHsl: 47 100% 95%;
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotBrutalAccentColorHsl: 37 92% 65%;

  ::-webkit-scrollbar {
    width: 2px;
  }

  ::-webkit-scrollbar-track {
    background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
    width: 2px !important;
  }

  ::-webkit-scrollbar-thumb {
    background: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    width: 2px !important;
  }
}

.ygpts-frame {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border-radius: 10px !important;
  box-shadow: 7px 7px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
}

.ygpts-widgetBtn {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
  border-radius: 10px !important;
  transform: translate(0, 0);
  transition: all 0.1s ease-in-out !important;

  & img {
    border-radius: 8px !important;
  }
}

.ygpts-widgetBtn:hover {
  transform: translate(-2px, -2px);
  box-shadow: 6px 6px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
}

.ygpts-widgetBtn:active {
  transform: translate(2px, 2px);
  box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
}

/* Square avatar for neo-brutalist style */
.ygc-avatar {
  border-radius: 10px !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
}

.tabs {
  gap: 5px !important;
  padding: 5px 5px !important;

  .tabItem {
    color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
    font-weight: bold !important;
    padding: 8px 16px !important;
    border: 2px solid transparent;
    transition: all 0.1s ease-in-out;
    border-radius: 999px !important;
    height: fit-content !important;

    .tabText {
      display: none !important;
    }

    &:hover {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      box-shadow: 3px 3px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }

    &.active {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      box-shadow: 3px 3px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }
  }
}

.sectionHeader,
.chatHeader,
.homeHeader {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-bottom: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
}

.helpContainer {
  .sectionHeader {
    .helpBackBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      border: 2px solid transparent !important;
      border-radius: 5px !important;
      transition: all 0.1s ease-in-out !important;

      &:hover {
        background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      }
    }
  }

  .helpSearchBox {
    .helpSearchInput {
      background-color: transparent;
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.1s ease-in-out !important;
      &:focus,
      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }

  .helpList {
    .helpArticleItem:hover,
    .helpCategoryItem:hover {
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.3) !important;
    }
  }
}

.refreshIcon,
.closeIcon,
.chatBackBtn,
.homeHeaderCloseBtn,
.languagePickerBtn,
.sessionCloseBtn {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border: 2px solid transparent !important;
  border-radius: 5px !important;
  transition: all 0.1s ease-in-out !important;

  &:hover {
    background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
  }
}

.chatContainer {
  .chatMessagesList {
    background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        // border-radius: 0 !important;
        box-shadow: 3px 3px 0 0px hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }
}

.homeWrapper {
  .homeHeader {
    .languagePickerPopup {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 0 !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
    }
  }

  .homeQueryBox {
    .homeQueryTextArea {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.1s ease-in-out !important;
      &:focus,
      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border-radius: 5px !important;
    box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    transform: translate(-2px, -2px);
    transition: all 0.1s ease-in-out !important;

    &:hover {
      transform: translate(0, 0);
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }

    &:active {
      transform: translate(20, 0);
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }
  }

  .homeElementContainer {
    gap: 15px !important;
    padding: 15px 0 !important;

    .HomeElementLink {
      color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
      font-weight: bold !important;
      text-decoration: none !important;
      transition: all 0.1s ease-in-out;

      &:hover {
        opacity: 0.7 !important;
      }
    }

    .homeElemenCard {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 0 !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      transition: all 0.1s ease-in-out !important;

      .item {
        border: none;
      }

      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }

    .featuredArticles {
      padding: 15px 5px 15px 0 !important;

      .articleSearchButton {
        border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        border-radius: 5px !important;
        box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
        transition: all 0.1s ease-in-out !important;
        background-color: transparent !important;

        &:hover,
        &:focus {
          box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
        }
      }

      .homeArticleList {
        padding: 5px 0 !important;
      }
    }
  }
}

.sessionsWrapper {
  .sessionsList {
    .sessionItem {
      border-top: 2px solid transparent;
      border-bottom: 2px solid transparent;
      transition: all 0.1s ease-in-out;

      &:hover {
        border-top: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        border-bottom: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.3) !important;
      }

      .countBox {
        background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        border-radius: 0 !important;
        font-weight: bold !important;
        border-radius: 999px !important;
      }
    }
  }

  .startNewConversationBtn {
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border-radius: 5px !important;
    box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    transform: translate(-2px, -2px) scale(1) !important;

    transition: all 0.1s ease-in-out !important;

    &:hover {
      transform: translate(0, 0) scale(1) !important;
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }

    &:active {
      transform: translate(0, 0) scale(1) !important;
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }
  }
}

.footer {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border-top: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

  .audioRecorderWrapper {
    background-color: transparent !important;

    .audioRecorderButton {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

      .audioRecorderButtonText {
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        border-radius: 2px !important;
        font-weight: bold !important;
        transition: all 0.1s ease-in-out;

        &:hover {
          background-color: hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.5) !important;
        }
      }
    }

    .audioRecorderCloseBtn {
      background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

      svg {
        fill: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      }
    }
  }
}.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 0 0% 0%;
  --yourgptChatbotSurfaceColorHsl: 60 100% 100%;
  --yourgptChatbotTextColorHsl: 0 0% 0%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 100%;
  --yourgptChatbotBotMessageBgColorHsl: 120 100% 97%;
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotUserMessageBgColorHsl: 47 100% 95%;
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotBrutalAccentColorHsl: 37 92% 65%;

  ::-webkit-scrollbar {
    width: 2px;
  }

  ::-webkit-scrollbar-track {
    background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
    width: 2px !important;
  }

  ::-webkit-scrollbar-thumb {
    background: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    width: 2px !important;
  }
}

.ygpts-frame {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border-radius: 10px !important;
  box-shadow: 7px 7px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
}

.ygpts-widgetBtn {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
  border-radius: 10px !important;
  transform: translate(0, 0);
  transition: all 0.1s ease-in-out !important;

  & img {
    border-radius: 8px !important;
  }
}

.ygpts-widgetBtn:hover {
  transform: translate(-2px, -2px);
  box-shadow: 6px 6px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
}

.ygpts-widgetBtn:active {
  transform: translate(2px, 2px);
  box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
}

.ygc-avatar {
  border-radius: 10px !important;
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  overflow: hidden !important;
}

.tabs {
  gap: 5px !important;
  padding: 5px 5px !important;

  .tabItem {
    color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
    font-weight: bold !important;
    padding: 8px 16px !important;
    border: 2px solid transparent;
    transition: all 0.1s ease-in-out;
    border-radius: 999px !important;
    height: fit-content !important;

    .tabText {
      display: none !important;
    }

    &:hover {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      box-shadow: 3px 3px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }

    &.active {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      box-shadow: 3px 3px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }
  }
}

.sectionHeader,
.chatHeader,
.homeHeader {
  background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-bottom: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
}

.helpContainer {
  .sectionHeader {
    .helpBackBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      border: 2px solid transparent !important;
      border-radius: 5px !important;
      transition: all 0.1s ease-in-out !important;

      &:hover {
        background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      }
    }
  }

  .helpSearchBox {
    .helpSearchInput {
      background-color: transparent;
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.1s ease-in-out !important;
      &:focus,
      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }

  .helpList {
    .helpArticleItem:hover,
    .helpCategoryItem:hover {
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.3) !important;
    }
  }
}

.refreshIcon,
.closeIcon,
.chatBackBtn,
.homeHeaderCloseBtn,
.languagePickerBtn,
.sessionCloseBtn {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border: 2px solid transparent !important;
  border-radius: 5px !important;
  transition: all 0.1s ease-in-out !important;

  &:hover {
    background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
  }
}

.chatContainer {
  .chatMessagesList {
    background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        // border-radius: 0 !important;
        box-shadow: 3px 3px 0 0px hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }
}

.languagePickerPopup {
  border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  border-radius: 7px !important;
  box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;

  .inputField {
    padding: unset !important;
    border: none !important;
    border-radius: 7px 7px 0 0 !important;
    border-bottom: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;

    input {
      background-color: transparent !important;
    }
  }

  .item {
    transition: all 0.1s ease-in-out !important;
    &:hover {
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.3) !important;
    }
    &.active {
      background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.5) !important;
    }
  }
}

.homeWrapper {
  .homeQueryBox {
    .homeQueryTextArea {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.1s ease-in-out !important;
      &:focus,
      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border-radius: 5px !important;
    box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    transform: translate(-2px, -2px);
    transition: all 0.1s ease-in-out !important;

    &:hover {
      transform: translate(0, 0);
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }

    &:active {
      transform: translate(20, 0);
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }
  }

  .homeElementContainer {
    gap: 15px !important;
    padding: 15px 0 !important;

    .HomeElementLink {
      color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
      font-weight: bold !important;
      text-decoration: none !important;
      transition: all 0.1s ease-in-out;

      &:hover {
        opacity: 0.7 !important;
      }
    }

    .homeElemenCard {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 0 !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      transition: all 0.1s ease-in-out !important;

      .item {
        border: none;
      }

      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }

    .featuredArticles {
      padding: 15px 5px 15px 0 !important;

      .articleSearchButton {
        border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        border-radius: 5px !important;
        box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
        transition: all 0.1s ease-in-out !important;
        background-color: transparent !important;

        &:hover,
        &:focus {
          box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
        }
      }

      .homeArticleList {
        padding: 5px 0 !important;
      }
    }

    .homeVideoContainer {
      border: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
      border-radius: 5px !important;
      box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.1s ease-in-out !important;

      &:hover {
        box-shadow: 2px 2px 0 0 hsl(var(--yourgptChatbotTextColorHsl)) !important;
      }
    }
  }
}

.sessionsWrapper {
  .sessionsList {
    .sessionItem {
      border-top: 2px solid transparent;
      border-bottom: 2px solid transparent;
      transition: all 0.1s ease-in-out;

      &:hover {
        border-top: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        border-bottom: 2px solid hsl(var(--yourgptChatbotTextColorHsl)) !important;
        background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.3) !important;
      }

      .countBox {
        background-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        border-radius: 0 !important;
        font-weight: bold !important;
        border-radius: 999px !important;
      }
    }
  }

  .startNewConversationBtn {
    background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    border: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border-radius: 5px !important;
    box-shadow: 4px 4px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    transform: translate(-2px, -2px) scale(1) !important;

    transition: all 0.1s ease-in-out !important;

    &:hover {
      transform: translate(0, 0) scale(1) !important;
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }

    &:active {
      transform: translate(0, 0) scale(1) !important;
      box-shadow: 0px 0px 0 0 hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    }
  }
}

.footer {
  background-color: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  border-top: 2px solid hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

  .audioRecorderWrapper {
    background-color: transparent !important;

    .audioRecorderButton {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

      .audioRecorderButtonText {
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
        border-radius: 2px !important;
        font-weight: bold !important;
        transition: all 0.1s ease-in-out;

        &:hover {
          background-color: hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.5) !important;
        }
      }
    }

    .audioRecorderCloseBtn {
      background-color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

      svg {
        fill: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      }
    }
  }
}
```

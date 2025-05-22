![Doom Theme Preview]()

[▶️ Watch Video Demo]()

### Doom Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
.ygpt-chatbot.ygpt-chatbot {
  /* Gritty Metallic Dr. Doom Color Palette */
  --yourgptChatbotPrimaryColorHsl: 45 15% 25%; /* Dark Bronze/Metal */
  --yourgptChatbotSurfaceColorHsl: 45 8% 12%; /* Very Dark Metal Background */
  --yourgptChatbotTextColorHsl: 45 20% 75%; /* Light Bronze Text */
  --yourgptChatbotTextOnPrimaryColorHsl: 45 25% 85%; /* Lighter Bronze Text */
  --yourgptChatbotBotMessageBgColorHsl: 45 12% 18%; /* Dark Metal for Bot */
  --yourgptChatbotBotMessageTextColorHsl: 45 20% 75%; /* Light Bronze Text */
  --yourgptChatbotUserMessageBgColorHsl: 45 10% 15%; /* Slightly Different Metal for User */
  --yourgptChatbotUserMessageTextColorHsl: 45 20% 75%; /* Light Bronze Text */
  --fantastic4AccentColorHsl: 45 25% 35%; /* Brighter Bronze Accent */
  --fantastic4SecondaryBlueHsl: 45 18% 30%; /* Secondary Metal Tone */
  --fantastic4GlowColor: rgba(139, 118, 78, 0.4); /* Bronze Glow */
  --doomBorderColor: rgba(139, 118, 78, 0.3); /* Metal Border */
  --doomShadowColor: rgba(0, 0, 0, 0.8); /* Deep Shadow */
}

/* Widget Button - Doom's Gauntlet */
.ygpts-widgetBtn {
  background: linear-gradient(135deg, 
    hsl(var(--yourgptChatbotPrimaryColorHsl)), 
    hsl(45 12% 20%)) !important;
  border: 2px solid hsl(var(--fantastic4AccentColorHsl)) !important;
  border-radius: 50% !important;
  box-shadow: 
    0 0 0 1px var(--doomBorderColor),
    0 4px 12px var(--doomShadowColor),
    inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;
  transition: all 0.3s ease-in-out !important;
  transform: translateY(0) !important;
  position: relative !important;

  & img {
    filter: brightness(1.2) contrast(1.3) sepia(0.2) !important;
  }

  &:before {
    content: "" !important;
    position: absolute !important;
    top: 2px !important;
    left: 2px !important;
    right: 2px !important;
    bottom: 2px !important;
    border-radius: 50% !important;
    background: radial-gradient(circle at 30% 30%, 
      rgba(139, 118, 78, 0.1) 0%, 
      transparent 70%) !important;
    pointer-events: none !important;
  }
}

.ygpts-widgetBtn:hover {
  transform: translateY(-3px) !important;
  box-shadow: 
    0 0 0 1px var(--doomBorderColor),
    0 6px 16px var(--doomShadowColor),
    0 0 20px var(--fantastic4GlowColor),
    inset 0 1px 0 rgba(139, 118, 78, 0.3) !important;
}

.ygpts-widgetBtn:active {
  transform: translateY(-1px) !important;
  box-shadow: 
    0 0 0 1px var(--doomBorderColor),
    0 2px 8px var(--doomShadowColor),
    inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
}

/* Main Chat Frame - Doom's Fortress Interface */
.ygpts-frame {
  background: linear-gradient(145deg, 
    hsl(var(--yourgptChatbotSurfaceColorHsl)), 
    hsl(45 6% 8%)) !important;
  border: 1px solid var(--doomBorderColor) !important;
  border-radius: 12px !important;
  box-shadow: 
    0 8px 32px var(--doomShadowColor),
    inset 0 1px 0 rgba(139, 118, 78, 0.1),
    0 0 0 1px rgba(0, 0, 0, 0.5) !important;
  overflow: hidden !important;
/*   position: relative !important; */

  &:before {
    content: "" !important;
    position: absolute !important;
    top: 0 !important;
    left: 0 !important;
    right: 0 !important;
    bottom: 0 !important;
    background: 
      radial-gradient(circle at 20% 20%, rgba(139, 118, 78, 0.03) 0%, transparent 50%),
      radial-gradient(circle at 80% 80%, rgba(139, 118, 78, 0.02) 0%, transparent 50%) !important;
    pointer-events: none !important;
    z-index: 0 !important;
  }
}

/* Avatar - Doom's Mask */
.ygc-avatar {
  border-radius: 50% !important;
  border: 2px solid var(--doomBorderColor) !important;
  box-shadow: 
    0 0 15px var(--fantastic4GlowColor),
    inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;
  overflow: hidden !important;
  position: relative !important;

  &:after {
    content: "" !important;
    position: absolute !important;
    top: 0 !important;
    left: 0 !important;
    right: 0 !important;
    bottom: 0 !important;
    background: radial-gradient(circle at 30% 30%, 
      rgba(139, 118, 78, 0.1) 0%, 
      transparent 70%) !important;
    pointer-events: none !important;
  }
}

/* Tab Navigation - Doom's Control Panel */
.ygc-tabs {
  background: linear-gradient(180deg, 
    hsl(45 10% 15%), 
    hsl(var(--yourgptChatbotSurfaceColorHsl))) !important;
  border-bottom: 1px solid var(--doomBorderColor) !important;
  padding: 8px 16px !important;
  position: relative !important;

  .ygc-tabItem {
    color: hsl(var(--yourgptChatbotTextColorHsl) / 0.8) !important;
    font-weight: 600 !important;
    padding: 8px 16px !important;
    border-radius: 6px !important;
    transition: all 0.2s ease-in-out !important;
    position: relative !important;
    background: transparent !important;
    border: 1px solid transparent !important;

    &:hover {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      background: linear-gradient(135deg, 
        hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.3),
        hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.1)) !important;
      border-color: var(--doomBorderColor) !important;
      box-shadow: inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
    }

    &.active {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      background: linear-gradient(135deg, 
        hsl(var(--yourgptChatbotPrimaryColorHsl)),
        hsl(var(--fantastic4SecondaryBlueHsl))) !important;
      border-color: hsl(var(--fantastic4AccentColorHsl)) !important;
      box-shadow: 
        inset 0 1px 0 rgba(139, 118, 78, 0.2),
        0 2px 4px rgba(0, 0, 0, 0.3) !important;

      &:after {
        content: "" !important;
        position: absolute !important;
        bottom: -9px !important;
        left: 50% !important;
        transform: translateX(-50%) !important;
        width: 24px !important;
        height: 2px !important;
        background: linear-gradient(90deg, 
          transparent, 
          hsl(var(--fantastic4AccentColorHsl)), 
          transparent) !important;
        border-radius: 2px !important;
      }
    }
  }
}

/* Headers - Doom's Command Bridge */
.sectionHeader,
.chatHeader,
.ygc-homeHeader {
  background: linear-gradient(135deg, 
    hsl(var(--yourgptChatbotPrimaryColorHsl)), 
    hsl(var(--fantastic4SecondaryBlueHsl))) !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-bottom: 1px solid var(--doomBorderColor) !important;
  font-weight: 600 !important;
  padding: 16px 20px !important;
  box-shadow: 
    0 4px 12px var(--doomShadowColor),
    inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;
  position: relative !important;
  overflow: hidden !important;
}

/* Metallic texture effect for headers */
.sectionHeader:after,
.chatHeader:after,
.ygc-homeHeader:after {
  content: "" !important;
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  right: 0 !important;
  bottom: 0 !important;
  background: 
    radial-gradient(circle at 25% 25%, rgba(139, 118, 78, 0.1) 0%, transparent 50%),
    radial-gradient(circle at 75% 75%, rgba(139, 118, 78, 0.05) 0%, transparent 50%),
    linear-gradient(45deg, transparent 48%, rgba(139, 118, 78, 0.02) 50%, transparent 52%) !important;
  z-index: 0 !important;
}

/* Action Buttons - Doom's Controls */
.refreshIcon,
.closeIcon,
.chatBackBtn,
.homeHeaderCloseBtn,
.languagePickerBtn,
.sessionCloseBtn {
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-radius: 6px !important;
  transition: all 0.2s ease-in-out !important;
  padding: 8px !important;
  background: transparent !important;
  border: 1px solid transparent !important;
  position: relative !important;
  z-index: 1 !important;

  &:hover {
    background: linear-gradient(135deg, 
      rgba(139, 118, 78, 0.2), 
      rgba(139, 118, 78, 0.1)) !important;
    border-color: var(--doomBorderColor) !important;
    transform: translateY(-1px) !important;
    box-shadow: 
      0 2px 4px rgba(0, 0, 0, 0.3),
      inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
  }

  &:active {
    transform: translateY(0) !important;
    box-shadow: inset 0 1px 0 rgba(0, 0, 0, 0.2) !important;
  }
}

/* Help Container - Doom's Archive */
.helpContainer {
  .sectionHeader {
    .helpBackBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      border-radius: 6px !important;
      transition: all 0.2s ease-in-out !important;
      background: transparent !important;
      border: 1px solid transparent !important;

      &:hover {
        background: linear-gradient(135deg, 
          rgba(139, 118, 78, 0.2), 
          rgba(139, 118, 78, 0.1)) !important;
        border-color: var(--doomBorderColor) !important;
      }
    }
  }

  .helpSearchBox {
    .helpSearchInput {
      background: linear-gradient(145deg, 
        hsl(var(--yourgptChatbotSurfaceColorHsl)), 
        hsl(45 8% 10%)) !important;
      border: 1px solid var(--doomBorderColor) !important;
      border-radius: 8px !important;
      padding: 12px 16px !important;
      color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.2s ease-in-out !important;
      box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.3) !important;

      &:focus,
      &:hover {
        border-color: hsl(var(--fantastic4AccentColorHsl)) !important;
        box-shadow: 
          inset 0 2px 4px rgba(0, 0, 0, 0.3),
          0 0 0 2px rgba(139, 118, 78, 0.2) !important;
      }

      &::placeholder {
        color: hsl(var(--yourgptChatbotTextColorHsl) / 0.6) !important;
      }
    }
  }

  .helpList {
    .helpArticleItem,
    .helpCategoryItem {
      border-radius: 6px !important;
      transition: all 0.15s ease-in-out !important;
      border: 1px solid transparent !important;

      &:hover {
        background: linear-gradient(135deg, 
          hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2),
          hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.1)) !important;
        border-color: var(--doomBorderColor) !important;
        transform: translateX(4px) !important;
        box-shadow: 
          0 2px 4px rgba(0, 0, 0, 0.2),
          inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
      }
    }
  }
}

/* Language Picker - Doom's Translator */
.languagePickerPopup {
  border: 1px solid var(--doomBorderColor) !important;
  border-radius: 10px !important;
  box-shadow: 
    0 8px 32px var(--doomShadowColor),
    0 0 0 1px rgba(0, 0, 0, 0.5) !important;
  background: linear-gradient(145deg, 
    hsl(var(--yourgptChatbotSurfaceColorHsl)), 
    hsl(45 6% 8%)) !important;
  overflow: hidden !important;
}

/* Chat Messages - Doom's Communication */
.chatContainer {
  .chatMessagesList {
    background: linear-gradient(180deg, 
      hsl(45 8% 12%), 
      hsl(45 6% 10%)) !important;
    padding: 20px !important;
  }

  /* Bot Message - Doom's Voice */
  .botMessage {
    background: linear-gradient(135deg, 
      hsl(var(--yourgptChatbotBotMessageBgColorHsl)), 
      hsl(45 10% 16%)) !important;
    color: hsl(var(--yourgptChatbotBotMessageTextColorHsl)) !important;
    border-radius: 16px !important;
    border-top-left-radius: 4px !important;
    border: 1px solid var(--doomBorderColor) !important;
    box-shadow: 
      0 4px 8px rgba(0, 0, 0, 0.3),
      inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
    position: relative !important;

    &:before {
      content: "" !important;
      position: absolute !important;
      top: 0 !important;
      left: 0 !important;
      right: 0 !important;
      bottom: 0 !important;
      background: radial-gradient(circle at 20% 20%, 
        rgba(139, 118, 78, 0.03) 0%, 
        transparent 60%) !important;
      border-radius: inherit !important;
      pointer-events: none !important;
    }
  }

  /* User Message - User's Input */
  .userMessage {
    background: linear-gradient(135deg, 
      hsl(var(--fantastic4AccentColorHsl) / 0.3), 
      hsl(var(--yourgptChatbotUserMessageBgColorHsl))) !important;
    color: hsl(var(--yourgptChatbotUserMessageTextColorHsl)) !important;
    border-radius: 16px !important;
    border-top-right-radius: 4px !important;
    border: 1px solid hsl(var(--fantastic4AccentColorHsl) / 0.5) !important;
    box-shadow: 
      0 4px 8px rgba(0, 0, 0, 0.3),
      inset 0 1px 0 rgba(139, 118, 78, 0.15) !important;
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 1px solid var(--doomBorderColor) !important;
        border-radius: 8px !important;
        background: linear-gradient(145deg, 
          hsl(var(--yourgptChatbotSurfaceColorHsl)), 
          hsl(45 6% 8%)) !important;
        box-shadow: 
          0 4px 8px rgba(0, 0, 0, 0.2),
          inset 0 1px 0 rgba(139, 118, 78, 0.05) !important;
      }
    }
  }
}

/* Home Wrapper - Doom's Command Center */
.homeWrapper {
  .homeQueryBox {
    .homeQueryTextArea {
      background: linear-gradient(145deg, 
        hsl(var(--yourgptChatbotSurfaceColorHsl)), 
        hsl(45 8% 10%)) !important;
      border: 1px solid var(--doomBorderColor) !important;
      border-radius: 12px !important;
      padding: 16px 20px !important;
      color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
      transition: all 0.2s ease-in-out !important;
      box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.3) !important;

      &:focus,
      &:hover {
        border-color: hsl(var(--fantastic4AccentColorHsl)) !important;
        box-shadow: 
          inset 0 2px 4px rgba(0, 0, 0, 0.3),
          0 0 0 2px rgba(139, 118, 78, 0.2) !important;
      }

      &::placeholder {
        color: hsl(var(--yourgptChatbotTextColorHsl) / 0.6) !important;
      }
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background: linear-gradient(135deg, 
      hsl(var(--yourgptChatbotPrimaryColorHsl)), 
      hsl(var(--fantastic4SecondaryBlueHsl))) !important;
    border: 1px solid hsl(var(--fantastic4AccentColorHsl)) !important;
    border-radius: 8px !important;
    padding: 12px 20px !important;
    transition: all 0.3s ease-in-out !important;
    transform: translateY(0) !important;
    font-weight: 600 !important;
    box-shadow: 
      0 4px 8px rgba(0, 0, 0, 0.2),
      inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;

    &:hover {
      background: linear-gradient(135deg, 
        hsl(45 18% 30%), 
        hsl(45 15% 25%)) !important;
      transform: translateY(-2px) !important;
      box-shadow: 
        0 6px 12px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(139, 118, 78, 0.3) !important;
    }

    &:active {
      transform: translateY(0) !important;
      box-shadow: 
        0 2px 4px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(0, 0, 0, 0.1) !important;
    }
  }

  .homeElementContainer {
    gap: 16px !important;
    padding: 16px 0 !important;

    .HomeElementLink {
      color: hsl(var(--fantastic4AccentColorHsl)) !important;
      font-weight: 500 !important;
      transition: all 0.2s ease-in-out !important;

      &:hover {
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        text-decoration: underline !important;
        text-shadow: 0 0 4px var(--fantastic4GlowColor) !important;
      }
    }

    .homeElementCard {
      border: 1px solid var(--doomBorderColor) !important;
      border-radius: 10px !important;
      background: linear-gradient(145deg, 
        hsl(var(--yourgptChatbotSurfaceColorHsl)), 
        hsl(45 6% 8%)) !important;
      box-shadow: 
        0 4px 12px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(139, 118, 78, 0.05) !important;
      transition: all 0.3s ease-in-out !important;
      overflow: hidden !important;

      .ygc-item {
        border: none !important;
        border-radius: 0 !important;
        background: transparent !important;
      }

      &:hover {
        transform: translateY(-4px) !important;
        border-color: hsl(var(--fantastic4AccentColorHsl)) !important;
        box-shadow: 
          0 8px 24px rgba(0, 0, 0, 0.4),
          0 0 0 1px var(--doomBorderColor),
          inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
      }
    }

    .featuredArticles {
      padding: 16px 8px !important;

      .articleSearchButton {
        border: 1px solid var(--doomBorderColor) !important;
        border-radius: 8px !important;
        transition: all 0.2s ease-in-out !important;
        background: linear-gradient(145deg, 
          hsl(var(--yourgptChatbotSurfaceColorHsl)), 
          hsl(45 8% 10%)) !important;
        color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
        box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.2) !important;

        &:hover,
        &:focus {
          border-color: hsl(var(--fantastic4AccentColorHsl)) !important;
          box-shadow: 
            inset 0 2px 4px rgba(0, 0, 0, 0.2),
            0 0 0 2px rgba(139, 118, 78, 0.2) !important;
        }
      }

      .homeArticleList {
        padding: 8px 0 !important;
      }
    }
  }
}

/* Sessions - Doom's Mission Logs */
.sessionsWrapper {
  .sessionsList {
    .sessionItem {
      border-radius: 8px !important;
      margin: 4px 0 !important;
      transition: all 0.2s ease-in-out !important;
      border: 1px solid transparent !important;

      &:hover {
        background: linear-gradient(135deg, 
          hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.2),
          hsl(var(--yourgptChatbotPrimaryColorHsl) / 0.1)) !important;
        border-color: var(--doomBorderColor) !important;
        transform: translateX(4px) !important;
        box-shadow: 
          0 2px 4px rgba(0, 0, 0, 0.2),
          inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;
      }

      .ygc-sessionItem-countBox {
        background: linear-gradient(135deg, 
          hsl(var(--yourgptChatbotPrimaryColorHsl)), 
          hsl(var(--fantastic4SecondaryBlueHsl))) !important;
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        border-radius: 6px !important;
        font-weight: 600 !important;
        border: 1px solid var(--doomBorderColor) !important;
        box-shadow: inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;
      }
    }
  }

  .startNewConversationBtn {
    background: linear-gradient(135deg, 
      hsl(var(--yourgptChatbotPrimaryColorHsl)), 
      hsl(var(--fantastic4SecondaryBlueHsl))) !important;
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    border: 1px solid hsl(var(--fantastic4AccentColorHsl)) !important;
    border-radius: 8px !important;
    padding: 12px 20px !important;
    font-weight: 600 !important;
    transition: all 0.3s ease-in-out !important;
    transform: translateY(0) !important;
    box-shadow: 
      0 4px 8px rgba(0, 0, 0, 0.2),
      inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;

    &:hover {
      background: linear-gradient(135deg, 
        hsl(45 18% 30%), 
        hsl(45 15% 25%)) !important;
      transform: translateY(-2px) !important;
      box-shadow: 
        0 6px 12px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(139, 118, 78, 0.3) !important;
    }

    &:active {
      transform: translateY(0) !important;
      box-shadow: 
        0 2px 4px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(0, 0, 0, 0.1) !important;
    }
  }
}

/* Footer - Doom's Control Interface */
.ygc-footer {
  background: linear-gradient(180deg, 
    hsl(var(--yourgptChatbotSurfaceColorHsl)), 
    hsl(45 6% 8%)) !important;
  border-top: 1px solid var(--doomBorderColor) !important;
  padding: 12px !important;
  box-shadow: inset 0 1px 0 rgba(139, 118, 78, 0.1) !important;

  /* Message Input - Doom's Communicator */
  .messageInput {
    background: linear-gradient(145deg, 
      hsl(var(--yourgptChatbotSurfaceColorHsl)), 
      hsl(45 8% 10%)) !important;
    border: 1px solid var(--doomBorderColor) !important;
    border-radius: 12px !important;
    padding: 12px 16px !important;
    color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
    transition: all 0.2s ease-in-out !important;
    box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.3) !important;

    &:focus,
    &:hover {
      border-color: hsl(var(--fantastic4AccentColorHsl)) !important;
      box-shadow: 
        inset 0 2px 4px rgba(0, 0, 0, 0.3),
        0 0 0 2px rgba(139, 118, 78, 0.2) !important;
    }

    &::placeholder {
      color: hsl(var(--yourgptChatbotTextColorHsl) / 0.6) !important;
    }
  }

  /* Send Button - Doom's Command */
  .sendBtn {
    background: linear-gradient(135deg, 
      hsl(var(--yourgptChatbotPrimaryColorHsl)), 
      hsl(var(--fantastic4SecondaryBlueHsl))) !important;
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    border: 1px solid hsl(var(--fantastic4AccentColorHsl)) !important;
    border-radius: 8px !important;
    transition: all 0.2s ease-in-out !important;
    box-shadow: 
      0 2px 4px rgba(0, 0, 0, 0.2),
      inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;

    &:hover {
      background: linear-gradient(135deg, 
        hsl(45 18% 30%), 
        hsl(45 15% 25%)) !important;
      transform: scale(1.05) !important;
      box-shadow: 
        0 4px 8px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(139, 118, 78, 0.3) !important;
    }

    &:active {
      transform: scale(1) !important;
      box-shadow: 
        0 1px 2px rgba(0, 0, 0, 0.3),
        inset 0 1px 0 rgba(0, 0, 0, 0.1) !important;
    }
  }

  .audioRecorderWrapper {
    background-color: transparent !important;

    .audioRecorderButton {
      color: hsl(var(--fantastic4AccentColorHsl)) !important;

      .audioRecorderButtonText {
        color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
        background: linear-gradient(135deg, 
          hsl(var(--yourgptChatbotPrimaryColorHsl)), 
          hsl(var(--fantastic4SecondaryBlueHsl))) !important;
        border: 1px solid var(--doomBorderColor) !important;
        border-radius: 6px !important;
        font-weight: 500 !important;
        transition: all 0.2s ease-in-out !important;
        box-shadow: inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;

        &:hover {
          background: linear-gradient(135deg, 
            hsl(45 18% 30%), 
            hsl(45 15% 25%)) !important;
          transform: translateY(-1px) !important;
          box-shadow: 
            0 2px 4px rgba(0, 0, 0, 0.2),
            inset 0 1px 0 rgba(139, 118, 78, 0.3) !important;
        }
      }
    }

    .audioRecorderCloseBtn {
      background: linear-gradient(135deg, 
        hsl(var(--fantastic4AccentColorHsl)), 
        hsl(45 20% 30%)) !important;
      border: 1px solid var(--doomBorderColor) !important;
      border-radius: 50% !important;
      box-shadow: 
        0 2px 4px rgba(0, 0, 0, 0.2),
        inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;

      svg {
        fill: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      }
    }
  }
}

/* Quick Access Button - Doom's Power Core */
.ygc-quickAccessButton {
  background: linear-gradient(135deg, 
    hsl(var(--yourgptChatbotPrimaryColorHsl)), 
    hsl(var(--fantastic4SecondaryBlueHsl))) !important;
  border: 2px solid hsl(var(--fantastic4AccentColorHsl)) !important;
  border-radius: 50% !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  box-shadow: 
    0 6px 16px var(--doomShadowColor),
    0 0 0 1px var(--doomBorderColor),
    0 0 20px var(--fantastic4GlowColor),
    inset 0 2px 0 rgba(139, 118, 78, 0.3) !important;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1) !important;
  position: relative !important;

  &:before {
    content: "" !important;
    position: absolute !important;
    top: 3px !important;
    left: 3px !important;
    right: 3px !important;
    bottom: 3px !important;
    border-radius: 50% !important;
    background: radial-gradient(circle at 30% 30%, 
      rgba(139, 118, 78, 0.2) 0%, 
      transparent 70%) !important;
    pointer-events: none !important;
  }

  &:hover {
    transform: scale(1.1) !important;
    background: linear-gradient(135deg, 
      hsl(45 18% 30%), 
      hsl(45 15% 25%)) !important;
    box-shadow: 
      0 8px 20px var(--doomShadowColor),
      0 0 0 1px var(--doomBorderColor),
      0 0 30px var(--fantastic4GlowColor),
      inset 0 2px 0 rgba(139, 118, 78, 0.4) !important;
  }

  &:active {
    transform: scale(0.95) !important;
    box-shadow: 
      0 4px 12px var(--doomShadowColor),
      0 0 0 1px var(--doomBorderColor),
      inset 0 1px 0 rgba(0, 0, 0, 0.2) !important;
  }
}

/* Scrollbars - Doom's Interface Elements */
.ygpt-chatbot * {
  &::-webkit-scrollbar {
    width: 8px !important;
    height: 8px !important;
  }

  &::-webkit-scrollbar-track {
    background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
    border-radius: 4px !important;
    box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.2) !important;
  }

  &::-webkit-scrollbar-thumb {
    background: linear-gradient(135deg, 
      hsl(var(--yourgptChatbotPrimaryColorHsl)), 
      hsl(var(--fantastic4SecondaryBlueHsl))) !important;
    border-radius: 4px !important;
    border: 1px solid var(--doomBorderColor) !important;
    box-shadow: inset 0 1px 0 rgba(139, 118, 78, 0.2) !important;

    &:hover {
      background: linear-gradient(135deg, 
        hsl(45 18% 30%), 
        hsl(45 15% 25%)) !important;
    }
  }

  &::-webkit-scrollbar-corner {
    background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  }
}

/* Loading States - Doom's Processing */
.ygpt-chatbot .loading,
.ygpt-chatbot .spinner {
  &:after {
    border-color: hsl(var(--fantastic4AccentColorHsl)) transparent transparent transparent !important;
  }
}

/* Selection Highlighting - Doom's Focus */
.ygpt-chatbot *::selection {
  background: hsl(var(--fantastic4AccentColorHsl) / 0.3) !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
}
```

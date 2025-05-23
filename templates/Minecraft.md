![Minecraft Theme Preview]()

[▶️ Watch Video Demo]()

### Herbie Theme

---

Copy the code below and paste in the CSS in branding section in Widget settings

You can always modify the colors according to your needs

```
@import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

.ygpt-chatbot.ygpt-chatbot {
  --yourgptChatbotPrimaryColorHsl: 37 69% 33%; /* Dirt Brown #593A1D */
  --yourgptChatbotSurfaceColorHsl: 44 38% 86%; /* Parchment #F4F1E6 */
  --yourgptChatbotTextColorHsl: 0 0% 0%;
  --yourgptChatbotTextOnPrimaryColorHsl: 0 0% 100%;
  --yourgptChatbotBotMessageBgColorHsl: 83 52% 67%; /* Grass Green #7FB238 */
  --yourgptChatbotBotMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotUserMessageBgColorHsl: 36 47% 67%; /* Wood Tan #B48A5B */
  --yourgptChatbotUserMessageTextColorHsl: 0 0% 0%;
  --yourgptChatbotBrutalAccentColorHsl: 48 100% 62%; /* Gold Accent #FFD83D */
  --yourgptChatbotStoneColorHsl: 0 0% 63%; /* Stone Gray #A1A1A1 */

  font-family: 'Press Start 2P', 'Courier New', monospace !important;

  ::-webkit-scrollbar {
    width: 8px;
  }

  ::-webkit-scrollbar-track {
    background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
    border: 2px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  }

  ::-webkit-scrollbar-thumb {
    background: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    border: 2px outset hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
    image-rendering: pixelated;
  }
}

/* Minecraft-style pixelated border utility */
.minecraft-border {
  border: 4px solid;
  border-color: 
    hsl(var(--yourgptChatbotStoneColorHsl)) 
    hsl(var(--yourgptChatbotPrimaryColorHsl)) 
    hsl(var(--yourgptChatbotPrimaryColorHsl)) 
    hsl(var(--yourgptChatbotStoneColorHsl));
  border-image: none;
  image-rendering: pixelated;
}

.minecraft-inset {
  border: 3px inset hsl(var(--yourgptChatbotStoneColorHsl));
  image-rendering: pixelated;
}

.minecraft-outset {
  border: 3px outset hsl(var(--yourgptChatbotStoneColorHsl));
  image-rendering: pixelated;
}

.ygpts-frame {
  background: 
    linear-gradient(to bottom, 
      hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 0%, 
      hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 8px,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 8px,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 100%
    ) !important;
  border: 4px solid !important;
  border-color: 
    hsl(var(--yourgptChatbotStoneColorHsl)) 
    hsl(35 40% 25%) 
    hsl(35 40% 25%) 
    hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  border-radius: 0 !important;
  box-shadow: 
    inset 2px 2px 0 rgba(255,255,255,0.3),
    inset -2px -2px 0 rgba(0,0,0,0.3),
    4px 4px 8px rgba(0,0,0,0.5) !important;
  image-rendering: pixelated;
}

.ygpts-widgetBtn {
  background: 
    linear-gradient(135deg, 
      hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 0%,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 100%
    ) !important;
  border: 3px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  border-radius: 0 !important;
  box-shadow: 
    2px 2px 4px rgba(0,0,0,0.5) !important;
  transform: translate(0, 0);
  transition: all 0.1s ease-in-out !important;
  image-rendering: pixelated;

  & img {
    border-radius: 0 !important;
    image-rendering: pixelated;
    filter: contrast(1.1) saturate(1.2);
  }
}

.ygpts-widgetBtn:hover {
  border: 3px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  transform: translate(1px, 1px);
  box-shadow: 1px 1px 2px rgba(0,0,0,0.7) !important;
}

.ygpts-widgetBtn:active {
  border: 3px inset hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
  transform: translate(2px, 2px);
  box-shadow: inset 2px 2px 4px rgba(0,0,0,0.5) !important;
}

/* Square avatar for Minecraft mob style */
.ygc-avatar {
  border-radius: 0 !important;
  border: 3px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  image-rendering: pixelated;
  background: hsl(var(--yourgptChatbotPrimaryColorHsl));
}

.ygc-tabs {
  gap: 4px !important;
  padding: 8px !important;
  background: 
    repeating-linear-gradient(
      90deg,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 0px,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 16px,
      hsl(35 40% 25%) 16px,
      hsl(35 40% 25%) 17px
    );

  .ygc-tabItem {
    color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
    font-weight: normal !important;
    font-size: 8px !important;
    padding: 6px 12px !important;
    border: 2px outset hsl(var(--yourgptChatbotStoneColorHsl));
    transition: all 0.1s ease-in-out;
    border-radius: 0 !important;
    height: fit-content !important;
    background: hsl(var(--yourgptChatbotSurfaceColorHsl));
    image-rendering: pixelated;

    .ygc-tabText {
      display: block !important;
      text-transform: uppercase;
    }

    &:hover {
      border: 2px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
      background: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      transform: translate(1px, 1px);
    }

    &.active {
      border: 2px inset hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      background: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      box-shadow: inset 1px 1px 2px rgba(0,0,0,0.3) !important;
    }
  }
}

.sectionHeader,
.chatHeader,
.ygc-homeHeader {
  background: 
    linear-gradient(to bottom,
      hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 0%,
      hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 60%,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 60%,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 100%
    ) !important;
  color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
  border-bottom: 4px solid hsl(35 40% 25%) !important;
  font-size: 10px !important;
  text-shadow: 2px 2px 0 rgba(0,0,0,0.8);
  image-rendering: pixelated;
}

.helpContainer {
  .sectionHeader {
    .helpBackBtn {
      color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      border: 2px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
      border-radius: 0 !important;
      transition: all 0.1s ease-in-out !important;
      background: hsl(var(--yourgptChatbotSurfaceColorHsl));
      padding: 4px 8px;

      &:hover {
        border: 2px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
        background: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      }
    }
  }

  .helpSearchBox {
    .helpSearchInput {
      background: hsl(var(--yourgptChatbotSurfaceColorHsl));
      border: 3px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
      border-radius: 0 !important;
      box-shadow: inset 2px 2px 4px rgba(0,0,0,0.3) !important;
      transition: all 0.1s ease-in-out !important;
      font-family: 'Press Start 2P', monospace;
      font-size: 8px;
      
      &:focus,
      &:hover {
        background: white;
        box-shadow: inset 1px 1px 2px rgba(0,0,0,0.5) !important;
      }
    }
  }

  .helpList {
    .helpArticleItem:hover,
    .helpCategoryItem:hover {
      background: 
        linear-gradient(90deg, 
          transparent 0%, 
          hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.3) 50%,
          transparent 100%
        ) !important;
      border-left: 4px solid hsl(var(--yourgptChatbotBrutalAccentColorHsl));
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
  border: 2px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  border-radius: 0 !important;
  transition: all 0.1s ease-in-out !important;
  background: hsl(var(--yourgptChatbotSurfaceColorHsl));
  image-rendering: pixelated;

  &:hover {
    border: 2px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
    background: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    transform: translate(1px, 1px);
  }
}

.chatContainer {
  .chatMessagesList {
    background: 
      radial-gradient(circle at 50% 50%, 
        hsl(var(--yourgptChatbotSurfaceColorHsl)) 0%,
        hsl(44 35% 82%) 100%
      ) !important;
    background-image: 
      repeating-linear-gradient(
        0deg,
        transparent,
        transparent 2px,
        rgba(139, 119, 101, 0.1) 2px,
        rgba(139, 119, 101, 0.1) 4px
      );
  }

  .boxOuter2 {
    .boxOuter {
      .box {
        border: 3px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
        border-radius: 0 !important;
        box-shadow: 2px 2px 4px rgba(0,0,0,0.3) !important;
        background: 
          linear-gradient(135deg,
            rgba(255,255,255,0.8) 0%,
            rgba(255,255,255,0.4) 100%
          );
        image-rendering: pixelated;
        
        /* Minecraft speech bubble styling */
        &[data-message-type="bot"] {
          background: 
            linear-gradient(135deg,
              hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 0%,
              hsl(83 45% 60%) 100%
            );
          border-color: hsl(83 60% 40%);
        }
        
        &[data-message-type="user"] {
          background: 
            linear-gradient(135deg,
              hsl(var(--yourgptChatbotUserMessageBgColorHsl)) 0%,
              hsl(36 40% 60%) 100%
            );
          border-color: hsl(36 55% 45%);
        }
      }
    }
  }
}

.languagePickerPopup {
  border: 4px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
  border-radius: 0 !important;
  box-shadow: 4px 4px 8px rgba(0,0,0,0.5) !important;
  background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
  image-rendering: pixelated;
}

.homeWrapper {
  .homeQueryBox {
    .homeQueryTextArea {
      border: 3px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
      border-radius: 0 !important;
      box-shadow: inset 2px 2px 4px rgba(0,0,0,0.3) !important;
      transition: all 0.1s ease-in-out !important;
      background: 
        linear-gradient(45deg,
          #FFF8DC 0%,
          #F4F1E6 100%
        );
      font-family: 'Press Start 2P', monospace;
      font-size: 8px;
      line-height: 1.4;
      
      &:focus,
      &:hover {
        background: white;
        box-shadow: inset 1px 1px 2px rgba(0,0,0,0.5) !important;
        border-color: hsl(var(--yourgptChatbotBrutalAccentColorHsl));
      }
    }
  }

  .homeSendBtn {
    color: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
    background: 
      linear-gradient(135deg,
        hsl(var(--yourgptChatbotBrutalAccentColorHsl)) 0%,
        hsl(48 90% 55%) 100%
      ) !important;
    border: 3px outset hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
    border-radius: 0 !important;
    box-shadow: 2px 2px 4px rgba(0,0,0,0.5) !important;
    transform: translate(0, 0);
    transition: all 0.1s ease-in-out !important;
    font-family: 'Press Start 2P', monospace;
    font-size: 8px;
    text-shadow: 1px 1px 0 rgba(0,0,0,0.5);
    image-rendering: pixelated;

    &:hover {
      border: 3px inset hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
      transform: translate(1px, 1px);
      box-shadow: 1px 1px 2px rgba(0,0,0,0.7) !important;
    }

    &:active {
      transform: translate(2px, 2px);
      box-shadow: inset 2px 2px 4px rgba(0,0,0,0.3) !important;
    }
  }

  .homeElementContainer {
    gap: 12px !important;
    padding: 12px 0 !important;

    .HomeElementLink {
      color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
      font-weight: normal !important;
      text-decoration: none !important;
      transition: all 0.1s ease-in-out;
      font-size: 8px;
      text-shadow: 1px 1px 0 rgba(255,255,255,0.5);

      &:hover {
        color: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        text-shadow: 1px 1px 0 rgba(0,0,0,0.3);
      }
    }

    .homeElementCard {
      border: 3px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
      border-radius: 0 !important;
      box-shadow: 2px 2px 4px rgba(0,0,0,0.3) !important;
      transition: all 0.1s ease-in-out !important;
      background: 
        linear-gradient(135deg,
          hsl(var(--yourgptChatbotSurfaceColorHsl)) 0%,
          hsl(44 30% 80%) 100%
        );
      image-rendering: pixelated;

      .ygc-item {
        border: none;
        border-radius: 0;
        font-size: 8px;
      }

      &:hover {
        border: 3px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
        transform: translate(1px, 1px);
        box-shadow: 1px 1px 2px rgba(0,0,0,0.5) !important;
      }
    }

    .featuredArticles {
      padding: 12px 4px 12px 0 !important;

      .articleSearchButton {
        border: 3px outset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
        border-radius: 0 !important;
        box-shadow: 2px 2px 4px rgba(0,0,0,0.3) !important;
        transition: all 0.1s ease-in-out !important;
        background: hsl(var(--yourgptChatbotSurfaceColorHsl)) !important;
        font-family: 'Press Start 2P', monospace;
        font-size: 8px;

        &:hover,
        &:focus {
          border: 3px inset hsl(var(--yourgptChatbotStoneColorHsl)) !important;
          transform: translate(1px, 1px);
          box-shadow: 1px 1px 2px rgba(0,0,0,0.5) !important;
        }
      }

      .homeArticleList {
        padding: 4px 0 !important;
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
        border: 2px solid hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        background: 
          linear-gradient(90deg,
            transparent 0%,
            hsl(var(--yourgptChatbotBrutalAccentColorHsl) / 0.2) 50%,
            transparent 100%
          ) !important;
        box-shadow: inset 0 0 8px rgba(0,0,0,0.1);
      }

      .ygc-sessionItem-countBox {
        background: 
          linear-gradient(135deg,
            hsl(var(--yourgptChatbotBrutalAccentColorHsl)) 0%,
            hsl(48 90% 55%) 100%
          ) !important;
        color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
        border: 2px outset hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        border-radius: 0 !important;
        font-weight: normal !important;
        font-size: 8px;
        text-shadow: 1px 1px 0 rgba(0,0,0,0.3);
        image-rendering: pixelated;
      }
    }
  }

  .startNewConversationBtn {
    background: 
      linear-gradient(135deg,
        hsl(var(--yourgptChatbotBotMessageBgColorHsl)) 0%,
        hsl(83 45% 60%) 100%
      ) !important;
    color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
    border: 3px outset hsl(var(--yourgptChatbotBotMessageBgColorHsl)) !important;
    border-radius: 0 !important;
    box-shadow: 2px 2px 4px rgba(0,0,0,0.5) !important;
    transform: translate(0, 0) !important;
    transition: all 0.1s ease-in-out !important;
    font-family: 'Press Start 2P', monospace;
    font-size: 8px;
    text-shadow: 1px 1px 0 rgba(0,0,0,0.3);
    image-rendering: pixelated;

    &:hover {
      border: 3px inset hsl(var(--yourgptChatbotBotMessageBgColorHsl)) !important;
      transform: translate(1px, 1px) !important;
      box-shadow: 1px 1px 2px rgba(0,0,0,0.7) !important;
    }

    &:active {
      transform: translate(2px, 2px) !important;
      box-shadow: inset 2px 2px 4px rgba(0,0,0,0.3) !important;
    }
  }
}

.ygc-footer {
  background: 
    linear-gradient(to top,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 0%,
      hsl(var(--yourgptChatbotPrimaryColorHsl)) 80%,
      hsl(var(--yourgptChatbotSurfaceColorHsl)) 80%,
      hsl(var(--yourgptChatbotSurfaceColorHsl)) 100%
    ) !important;
  border-top: 4px solid hsl(35 40% 25%) !important;
  image-rendering: pixelated;

  .audioRecorderWrapper {
    background: transparent !important;

    .audioRecorderButton {
      color: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;

      .audioRecorderButtonText {
        color: hsl(var(--yourgptChatbotTextColorHsl)) !important;
        background: hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        border: 2px outset hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
        border-radius: 0 !important;
        font-weight: normal !important;
        font-family: 'Press Start 2P', monospace;
        font-size: 6px;
        transition: all 0.1s ease-in-out;
        text-shadow: 1px 1px 0 rgba(0,0,0,0.3);

        &:hover {
          border: 2px inset hsl(var(--yourgptChatbotBrutalAccentColorHsl)) !important;
          transform: translate(1px, 1px);
        }
      }
    }

    .audioRecorderCloseBtn {
      background: hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      border: 2px outset hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      border-radius: 0 !important;

      svg {
        fill: hsl(var(--yourgptChatbotTextOnPrimaryColorHsl)) !important;
      }

      &:hover {
        border: 2px inset hsl(var(--yourgptChatbotPrimaryColorHsl)) !important;
      }
    }
  }
}

/* Additional Minecraft-specific enhancements */
* {
  image-rendering: pixelated !important;
  image-rendering: -moz-crisp-edges !important;
  image-rendering: crisp-edges !important;
}

/* Pixelated text rendering for authenticity */
.ygpt-chatbot * {
  font-family: 'Press Start 2P', 'Courier New', monospace !important;
  font-size: 8px !important;
  line-height: 1.6 !important;
}

/* Special styling for message text to be more readable */
.chatContainer .boxOuter2 .boxOuter .box {
  font-size: 9px !important;
  line-height: 1.5 !important;
  padding: 8px 12px !important;
}

/* Header text styling */
.sectionHeader,
.chatHeader,
.ygc-homeHeader {
  font-size: 10px !important;
  padding: 8px 12px !important;
  font-weight: normal !important;
}
```

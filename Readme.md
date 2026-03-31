# WAR: The Economy Battle Card Game

A fast-paced, strategic card game where classic color-matching meets intense economic warfare. Start with a $500 bank account, deploy military assets, utilize an in-game shop, and bankrupt your opponents to claim victory.

---

## 🎮 Overview

**WAR** completely reimagines the traditional discard-pile card game format. Instead of just emptying your hand, your primary goal is to protect your economy while devastating your opponents'. Every card played has a real financial impact, making every turn a calculated risk.

* **Players:** 2 - 10 Players
* **Starting Bank:** $500 per player
* **Win Condition:** Bankrupt the opponent ($0). 
* **The Ultimate Victory:** Achieve exactly **$1** in your bank while the opponent hits $0. 

---

## 🏗️ Technical Architecture

This project is engineered to be lightweight, fast, and highly portable. 

* **Single-File Build:** The entire application (logic, styling, and markup) is contained within a single HTML file. This eliminates complex dependency management and allows for instant sharing and offline play.
* **Sprite Sheet Slicing:** Card graphics are rendered using an advanced CSS `background-position` slicer. By loading only one master sprite sheet and shifting coordinates, the game drastically reduces HTTP requests and memory usage. It is designed to run at maximum FPS on any mobile browser, keeping your processor running ice-cold even without a custom water or vapor cooling setup.
* **Mobile-Optimized:** The UI is specifically scaled for touch interfaces. Card hitboxes, shop buttons, and the dashboard flex naturally to fit mobile browser dimensions.

---

## 💰 The Economy & Card Suits

Each color represents a military branch and features its own unique economic rule.

| Suit / Color | Branch | Economic Rule | Strategy |
| :--- | :--- | :--- | :--- |
| **🔴 RED** | Air Force | **The Payday:** Playing any Red card instantly earns you **$67**. | Use Red to rebuild your bank after taking heavy hits. |
| **🔵 BLUE** | Navy | **The Thief:** Steals **$20** directly from the opponent's bank to yours. | Excellent for widening the economic gap between players. |
| **🟢 GREEN** | Army | **Heavy Artillery:** Deals the base card damage plus an extra **$30**. | The primary aggressive suit to bankrupt opponents quickly. |
| **🟡 YELLOW** | Defense | **The Bunker:** Protects your bank from being stolen on the next turn. | Essential for surviving mid-game attacks. |

---

## ⚔️ Special Action Cards

Action cards disrupt the flow of the game and penalize the opponent's bank.

* **DRAW 2:** The next player draws 2 cards, and the bank instantly deducts **$20** from their account for "training costs."
* **FRIENDLY FIRE (Reverse):** Reverses turn order. If played immediately after an attack, the damage bounces back to the attacker.
* **TAX SEASON (Skip):** The next player loses their turn and must pay a **$40** tax to the center jackpot.

---

## 🛒 The Black Market Shop

Players are not limited to the cards they draw; they can buy their way to dominance. During your turn, before playing a card, you can spend money from your bank to purchase special assets.

> **TACTICAL NUKE**
> * **Cost:** $200 (Deducted from your bank immediately)
> * **Effect:** Deals a massive **$100** damage to the opponent. Because it is a Red/Air asset, playing it also earns you the **$67** payday. 

---

## 🚀 Installation & Usage

1. Download the HTML file to your device.
2. Ensure you have an active internet connection (to load the sprite sheet from the cloud).
3. Open the file directly in any modern web browser.
4. Tap your cards to deploy assets and watch the opponent's bank drain!


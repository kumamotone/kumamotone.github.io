# Focus Launcher — Reddit & Product Hunt ローンチプラン

---

## 1. アカウント準備

### Reddit

**今すぐやること（リリースの1週間前 = 今日から）**

- https://www.reddit.com/register/ でアカウント作成
- ユーザー名: 個人名っぽいもの推奨（ブランド名はNG）。`kuma_dev` のような開発者っぽい名前がベスト。間違っても `FocusLauncherOfficial` にしない — 宣伝アカウントに見える
- プロフィールに短い自己紹介を書く（"Android developer based in Tokyo" 程度）
- **投稿前に最低3〜5日はコミュニティに参加する**。他の人の投稿にコメントしたり、質問に答えたりする。新規アカウントがいきなり宣伝投稿するとスパム扱いされる

**参加すべきSubreddit（優先順）**

| Subreddit | メンバー | 特徴 | 投稿タイミング |
|-----------|---------|------|---------------|
| r/SideProject | ~200k | 個人開発に寛容、最初のテストに最適 | アカウント作成後すぐOK |
| r/androidapps | ~1M | Androidユーザーが多い、機能重視 | 数日コミュニティに参加した後 |
| r/digitalminimalism | ~400k | ターゲット層ど真ん中 | 体験談として自然に |
| r/nosurf | ~200k | スマホ依存からの脱却 | 体験談として自然に |

**重要な注意点**
- 各Subredditの投稿ルールを必ず読む。r/androidapps は [DEV] タグが必要な場合がある
- 同じ投稿を複数のSubredditにコピペしない（クロスポスト検知でスパム扱い）
- 各コミュニティ向けにトーンを変える

---

### Product Hunt

**今すぐやること**

- https://www.producthunt.com/ でアカウント作成（Xアカウントでの連携も可能）
- プロフィール写真・自己紹介を埋める（空プロフィールだと信頼度が下がる）
- 「Coming Soon」ページを作成（https://www.producthunt.com/launch → 「Preparing for launch」）
  - Tagline、Description、スクリーンショットを設定
  - 公開するとフォロー（通知登録）を集められる
- **ローンチ日までに他のプロダクトにUpvoteやコメントをしておく**。アクティブなアカウントほどローンチ時のアルゴリズム評価が高い
- **Hunter（推薦人）を探す**: 自分でもローンチできるが、フォロワーの多いHunterに推薦してもらうと初動が伸びる。ただし必須ではない

**ローンチ日の選び方**
- ベスト: **水曜 > 火曜 > 木曜**
- 避ける: 月曜（混雑）、金曜（トラフィック少）、週末
- 時間: 太平洋時間の午前0:01にローンチが始まる。事前にスケジュール設定しておく

---

## 2. Reddit 投稿文（英語）

### ■ r/digitalminimalism / r/nosurf 向け（体験談ベース）

> **Title:** I was severely addicted to my phone, so I built an Android launcher to fix it
>
> ---
>
> A couple of years ago, I realized I was spending entire days scrolling through social media feeds and short-form videos without even noticing. That was my wake-up call.
>
> I started trying minimalist launchers, app blockers, and screen time trackers. The idea of making overused apps less visible really worked for me. But over time, I kept hitting walls:
>
> - **Conditional blocking was impossible.** I wanted to block Twitter only when I was on my home Wi-Fi (so I could still use it at work), but no single app could do that. I needed a launcher AND a separate blocker.
> - **Usage stats required yet another app** — each with its own subscription and ads.
> - **Text-only launchers were too minimal.** I couldn't tell apart Google Authenticator and Microsoft Authenticator when they were just text. Too simple became its own kind of inconvenient.
>
> So I built what I actually wanted: **Focus Launcher** — an Android launcher that combines a minimal (but not *too* minimal) home screen, conditional app blocking (Wi-Fi + time-based rules), and built-in usage stats. All in one app, no ads, no account required.
>
> A few things that make it different:
>
> - **Block rules with conditions**: "Block X only on home Wi-Fi" or "Block Y between 9pm–7am"
> - **Grayscale mode for app icons**: reduces visual stimulation without removing icons entirely
> - **Usage stats built into the launcher**: see your screen time and add blocks right from there
> - **No ads, no data collection**: your data stays on your device
>
> It's currently in pre-registration on Google Play. I'm a solo developer based in Tokyo and built this for myself first — happy to answer any questions about the approach or the tech behind it.
>
> 🔗 [Google Play (pre-registration)](https://play.google.com/store/apps/details?id=dev.kuma.focuslauncher)
> 🌐 [Website](https://kuma.dev/focus-launcher/)

---

### ■ r/androidapps 向け（機能重視）

> **Title:** [DEV] Focus Launcher — minimal launcher with Wi-Fi/time-based app blocking and built-in usage stats
>
> ---
>
> Hey r/androidapps! I'm a solo Android developer and I've been working on a launcher that sits between "extreme minimalism" and a full-featured launcher.
>
> **The problem I was solving:** I used several apps together — a minimal launcher, a separate app blocker, and a screen time tracker — each with its own subscription. I wanted one app that did all three.
>
> **What Focus Launcher does:**
>
> - **Minimal home screen** with app icons (not text-only — I found pure text launchers frustrating when apps have similar names)
> - **Conditional block rules**: block apps based on Wi-Fi network, time of day, or both. Example: "Block Instagram only when connected to home Wi-Fi"
> - **Friction levels**: choose between full block, 5-second wait, require a reason, or soft warning
> - **Grayscale icons**: reduces visual stimulation without going full text-only
> - **Built-in usage stats**: check screen time and manage blocks from the same screen
> - **No ads, no account, no data collection**
>
> **Tech details for those interested:**
> - Kotlin + Jetpack Compose
> - Accessibility Service for app blocking (transparent about this — used only for launch detection)
> - Min API 33 (Android 13+)
> - All data stored locally on device
>
> Currently in pre-registration on Google Play, launching next week. Free during beta.
>
> 🔗 [Google Play (pre-registration)](https://play.google.com/store/apps/details?id=dev.kuma.focuslauncher)
> 🌐 [Website](https://kuma.dev/focus-launcher/)
>
> Would love to hear your thoughts — especially if you've used other minimalist launchers and hit similar frustrations.

---

### ■ r/SideProject 向け（開発ストーリー）

> **Title:** I built an Android launcher to cure my own phone addiction — launching next week
>
> ---
>
> Hey! I'm a solo developer in Tokyo, and I just finished building Focus Launcher — an Android launcher designed for digital detox.
>
> **Why I built it:** I was addicted to my phone. Tried minimalist launchers, app blockers, screen time trackers — but they all felt incomplete. Conditional blocking ("block X only on home Wi-Fi") required multiple apps. Usage stats meant yet another subscription. Text-only launchers made similar apps indistinguishable.
>
> So I combined everything into one launcher.
>
> **Key features:**
> - Minimal home screen (icons, not text-only)
> - Block rules with Wi-Fi and time conditions
> - Multiple friction levels (full block / 5s wait / require reason / soft warning)
> - Built-in usage stats
> - No ads, free during beta
>
> **Stack:** Kotlin, Jetpack Compose, Room, Hilt. Accessibility Service for block detection (only used for app launch detection, nothing else).
>
> Pre-registration is live on Google Play, launching next week. Would love feedback from fellow builders!
>
> 🔗 [Google Play](https://play.google.com/store/apps/details?id=dev.kuma.focuslauncher)
> 🌐 [Website](https://kuma.dev/focus-launcher/)

---

## 3. Product Hunt ローンチ素材

### Tagline（60文字以内）

**推奨:**

> A minimal Android launcher with smart app blocking

**代替案:**
- `Reclaim your attention with conditional app blocking`
- `Block apps by Wi-Fi, time, or both — right from your launcher`

---

### Description（260文字以内）

> Focus Launcher is an Android launcher for people who want to use their phone less. It combines a minimal home screen, conditional app blocking (by Wi-Fi network, time of day, or both), and built-in usage stats — all in one app. No ads, no account, no data collection. Your data stays on your device.

---

### First Comment（ローンチ日にMaker自身が最初のコメントとして投稿）

> Hey Product Hunt! 👋
>
> I'm Kuma, a solo developer based in Tokyo. I built Focus Launcher because I was genuinely addicted to my phone — spending entire days scrolling without realizing it.
>
> I tried combining minimalist launchers, app blockers, and screen time trackers, but each had limitations. The biggest gap: no single app let me set conditional rules like "block Instagram only when I'm on my home Wi-Fi."
>
> Focus Launcher brings it all together:
>
> 🏠 **Minimal home screen** — icons without the noise (no badges, no grid clutter)
> 🚫 **Smart blocking** — Wi-Fi-based, time-based, or both
> 📊 **Usage stats** — built right into the launcher
> 🔒 **Privacy-first** — no ads, no account, all data on-device
>
> It's free during beta and I'd love your honest feedback. Happy to answer any questions!

---

## 4. タイムライン

| 日付 | やること |
|------|---------|
| 今日（4/6） | Reddit + Product Huntアカウント作成 |
| 4/6–4/8 | Redditで他の投稿にコメント・参加。PH「Coming Soon」ページ作成 |
| 4/9 | r/SideProject に投稿（テスト） |
| 4/10 | フィードバックを反映して文面調整 |
| 4/10–11 | r/digitalminimalism, r/nosurf に投稿 |
| リリース日 | r/androidapps に投稿 + Product Hunt ローンチ（水曜推奨） |

---

## 5. Tips

- **Redditでは質問で終わる**。「Would love to hear your thoughts」のような一文があると、コメントがつきやすい
- **批判にはオープンに対応する**。「Accessibility Serviceを使うのはプライバシー的にどうなの？」という質問は確実に来る。LP のポリシーセクションの内容を使って丁寧に説明する
- **Product Huntでは画像が命**。スクリーンショットは既にあるので、それに加えて30秒程度のデモGIFがあると理想的
- **両方とも「自分のために作った」ストーリーを軸にする**。宣伝ではなく、同じ問題を抱えている人への共有というトーン

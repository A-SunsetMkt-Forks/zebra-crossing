# TLDR 網路安全清單

### 🤔 誰適合使用這份指南

- 你每天都上网——为了工作，刷社交媒体，使用网上银行等等。
- 你覺得你需要更注重保護自己的網絡安全和隱私，但你不面臨立刻的危險（如果你認為你現在就面臨危險，請尋找一對一的專家咨詢）。
- 你認為自己對科技有一定的熟悉程度。例如，在你自己的手機或電腦上修改設定你覺得沒有難度。

### 🌱 應該怎樣使用這份指南

- 安全建議按難度從低到高排列。建議從第一級別開始往難度高的進發。
- 從我自身經驗來講，我建議每一步都以級別一、級別二和級別三的順序進行。我也是這樣走過來的，而我認為我對科技的掌握程度只是中等水平。
- 基於場景的安全建議假定你已經閱讀了級別一到三的所有內容。
- 這份指南不斷更新。歡迎發起pull要求，或者把這份指南保存到你自己的Github頁面上。

### 🕒 最後一次更新時間

- 2019年11月27日， 基於2019年10月23日的英語原文。

---

## 🧐 理論和科學

### 🎯 威脅模型分析

- 你正在面臨哪種威脅？一些比較常見的威脅：公司間諜，警察/政府干預，網絡暴力等。
- 你需要保護哪些文件？常見的例子包括機密文件，私人圖片等。
- 我們每一個人都面臨一定的風險（不然的話我們也不會給我們的電腦和手機設置密碼），但我們需要瞭解清楚自己的風險，以免疏忽或者造成多疑恐慌。
- 如需瞭解更多信息，可以閱讀[這篇介紹（英文）](https://ssd.eff.org/en/module/introduction-threat-modeling)。

### 🔗 最薄弱的環節/短板

- 記住，最薄弱的環節往往才是最重要的！舉個例子，如果你獲取忘記密碼的方式是你的電子郵箱，那麼黑客要做的只是黑進你的郵箱。

### 🔡 不同加密程度

1. 不加密：任何入侵帳號的第三方都可以閱讀數據。
2. 一般加密：第三方無法閱讀加密了的數據。但你所使用的平台（如Google和Facebook）仍然擁有閱讀數據的權限，它們有可能會根據法院或政府要求把你的屬於與執法人員共享。
3. 點對點加密：數據只可以被發送方和接收方閱讀。這意味著就算是平台公司也沒有閱讀數據的權限。如果執法人員要求查看數據，服務商也沒有辦法提供任何信息。

### 🧩 元數據

- 是指關於你的數據的數據，比如你給什麼號碼打了電話，通話持續了多久（但不包括通話內容）。有了足夠的元數據，黑客可以拼湊出一副相對完整的關於你的信息畫像，比如你是誰，你認識哪些人，你的下一趟旅程去哪裡等等。目前，法律針對元數據的規定存在較多灰色地帶。

---

## 💦 第一級安全建議

### ✅ 行動清單

#### 電子郵件

- 如果你正在使用網頁版郵件服務，請確認你使用的鏈接含有`https://` 。如果沒有，請更換電郵服務商。      
- 請為你的電郵開啓二步驗證（如[Gmail](https://support.google.com/accounts/answer/185839?hl=en), [Protonmail](https://protonmail.com/support/knowledge-base/two-factor-authentication/)的設置）。需要注意的是，你應該使用驗證軟件進行二步驗證（如[Authy](https://authy.com/), [Google Authenticator](https://support.google.com/accounts/answer/1066447?hl=en)），短信驗證已經不再安全。
- 開啓二步驗證後，瞭解你的電郵是否支持備份碼（這是當你遺失你的設備時使用的驗證碼）。你可以在這裡瞭解如果在[Gmail進行設置](https://support.google.com/accounts/answer/1187538?hl=en)。

#### 強密碼

- 所有少於10位的密碼都是弱密碼，你可以通過使用”-“連字符號來設計由無關聯的單詞組成的長串密碼(比如strong-password-has-many-words)。
- 再三確認你重要賬號的密保問題（電郵，銀行，Facebook等）的答案不會輕易被你的朋友或者通過網上搜索有關你的資料猜到。
- 為你的各項賬號設置不一樣的密碼，因為密碼洩漏的事件經常發生。為了使你能記住不同賬號的不同密碼，你可以使用密碼管家 （[Lifehacker不同管家的測評](https://lifehacker.com/5529133/five-best-password-managers)）來儲存、自動填充及生成密碼。切記為你的重要賬號（電郵，社交媒體，銀行，雲儲存）設置唯一的不同的密碼。
- 為你的手機設置不容易被猜到的解鎖密碼。
- 如果你正在使用iPhone，關閉USB Accessories（Settings > Face ID & Passcode > Allow Access When Locked）。

#### 加密你的設備

- 加密你的手機儲存文件：[Android](http://www.networkworld.com/article/2689371/opensource-subnet/how-to-encrypt-an-android-device-in-5-steps.html)，[蘋果](https://ssd.eff.org/en/module/how-encrypt-your-iphone)（很多手機現在已經默認加密，但你不妨再次確認）。
- 加密你的手提電腦及桌面電腦的硬盤：[Windows](https://uit.stanford.edu/service/encryption/wholedisk/bitlocker), [Windows 如果沒有 BitLocker](https://veracrypt.codeplex.com/), [Mac OSX](https://support.apple.com/en-us/HT204837).
- 確保你的備份文件也是安全的！加密你的備份硬盤，同時確保你的在線備份儲存支持端對端加密。
- 謹記加密只有在你的設備關閉時才完全有效。

#### 其他

- 為你的電話卡設置密碼： [iPhone](https://support.apple.com/en-hk/HT201529), [Android](https://www.digitalcitizen.life/how-change-or-remove-sim-pin-android-2-steps). 搜索你電話服務商的網站，瞭解它們的初始密碼是什麼（初始密碼會根據運營商改變）。
- 取消對那些不使用二步驗證的軟件的授權 (比如[Gmail的設置](https://www.lifewire.com/revoke-an-application-password-for-gmail-1171889)).
- 關閉[Google日曆中自動接收日程邀請](https://calendar.google.com/calendar/r/settings)的设定（[瞭解為什麼](https://www.forbes.com/sites/daveywinder/2019/06/11/new-security-warning-issued-for-googles-1-5-billion-gmail-and-calendar-users/#3605ff0565e5)）。
- 開啓Facebook的[異常登錄警告](https://www.facebook.com/settings?tab=security)。
- [在Microsoft Office軟件中關閉macros](https://support.office.com/en-us/article/enable-or-disable-macros-in-office-files-12b036fd-d140-4e74-b45e-16fed1a7e5c6)

### 💪🏽 養成良好習慣

#### 電子郵件

- 謹防釣魚郵件：盡可能確認郵件發件人的地址以及郵件中所有鏈接的指向地址。
- 不要打開不必要的郵件附件。如果允許的話，用在線文件系統打開/預覽文件，或者讓你的同事使用文件共享服務來傳輸文件（Dropbox, Google Drive, SpiderOak, Tresorit），這些服務會比較難破解。
- 你可以把可疑文件上傳到 [VirusTotal](http://www.virustotal.com) 進行檢測（要注意的是上傳到VirusTotal 的文檔能被安全研究者閱讀，所以不要上傳敏感信息）。

#### 更新以下這些

- 當你收到提示要更新你的操作系統（手機或電腦），馬上進行更新。
- 同樣的，及時更新手機和電腦上的軟件。
- 偶爾查看你的路由器的固體軟件以及其他與互聯網連接的設備是否需要更新。

#### 其他

- 每一兩年更改你的重要密碼（如電郵，電腦登陸，密碼管家登陸密碼）。
- 在你捐獻或者送出你的設備前清除設備上的所有資料：[手機](http://lifehacker.com/5808280/what-should-i-do-with-my-phone-before-i-sell-it)，[電腦](http://lifehacker.com/5835369/how-do-i-securely-wipe-a-computer-before-donating-it-to-charity)。
- 不要在公共充電站為你的手機充電，它們有可能在盜取你手機中的數據。你可以選擇為你的移動電池充電。

---

**👍 太棒了！現在你已經掌握了關於安全的基本信息。 
👍 嘗試挑戰下一個級別？**  

---

## 💦💦 第二級安全建議

### ✅ 行動清單

#### 增強你的隱私保護

- 查看你經常使用的社交網絡的隱私設定：誰可以查看你的內容，誰可以評論你的內容，以及誰可能看到你的定位。
- 安裝這些瀏覽器擴展軟件來保護你的隱私，並保證它們在隱私瀏覽狀態下也是開啓的：
  - 廣告攔截（如 [uBlock Origin](https://github.com/gorhill/uBlock/), [Ghostery](https://www.ghostery.com/)）。
  - 跟蹤攔截 （[Privacy Badger](https://www.eff.org/privacybadger)）。
  - [HTTPS Everywhere](https://www.eff.org/https-everywhere)。
- 如果你擁有智能音響，關閉它的錄音功能：[Google Home](https://myaccount.google.com/activitycontrols/audio) 和 [Amazon Alexa](https://twitter.com/geminiimatt/status/1125611726773334017) 的關閉指南。

#### 其他

- 給你的設備設置可以讓你遠程跟蹤，清除和加密設備的第三方應用（如 [Prey](https://www.preyproject.com), [Lookout Security](https://www.lookout.com/)）。
- 查閱你主要的電子郵件和社交媒體賬號都綁定了哪些應用（比如哪些服務能夠連接你的Facebook，它們可以讀取你的哪些數據，以及它們是否可以為你發佈信息）。
- 查閱你電腦的瀏覽器都由哪些擴展應用，刪除那些你在一段時間內沒有使用過或者不記得安裝過的應用。
- 下載 [Stethoscope](https://ragtag.org/stethoscope) 並在你的電腦上運行，它可以幫助實現你的基本安全設置（比如加密，防火牆，屏幕鎖等）。

### 💪🏾 養成良好習慣

#### 增強的你隱私保護

- 少在網上發佈個人信息，特別是那些可以被用於驗證，跟蹤你或者實現釣魚的信息（地址，手機號碼，生日等）。
- 為你的手提電腦和手機購買防窺屏，它可以保護你的屏幕不被窺探（比如[3M](https://www.3m.com/3M/en_US/company-us/all-3m-products/~/All-3M-Products/Privacy-Screen-Protectors/Privacy-Products/Black-Privacy/)的這個產品）。
- 如果你擁有域名，開啓WHOIS隱私服務並持續使用它，這個服務的花費是值得的。但要注意的是WHOIS有歷史查詢工具，如果你曾經提供過你的真實地址，你很難完全清除那些記錄。

#### 其他

- 在使用公共網絡（如咖啡廳無線網絡）時使用付費VPN。免費的VPN不是一個好的選擇應為維護人員沒有足夠的動機保護你或者你的數據。[Wirecutter](https://thewirecutter.com/reviews/best-vpn-service/) 和 [Freedom of the Press](https://freedom.press/training/choosing-a-vpn/)提供了一些選擇VPN的建議。
- 每隔一段時間查看你的手機上安裝了哪些軟件，刪除那些你不再使用的軟件。
- 如果你需要給某人發送一個密碼，把它分成兩個部分用不同的途經發送（如電子郵件加語音童話）。
- 給你手提電腦的攝像貼上貼紙，或者其他可以遮擋攝像頭的配件。
- 不要用Google、Twitter、或者Facebook帳號登陸其他網站，每個網站和服務應該有自己的獨立的帳號。

---

**🎉 恭喜！你对网络安全的掌握已经到一定程度了！**

---

## 💦💦💦 第三級安全建議

### ✅ 行動清單

#### 為敏感文件上鎖

- 列出你不想被其他人接觸到的文件（如私人照片，護照文件等）。
- 用 [Cryptomator](https://cryptomator.org/) 或 [Veracrypt](https://www.veracrypt.fr/en/Home.html) 建立加密，密碼保護的空間來保護這些文件。
- 在你的電腦和手機上到進行這樣的設置。
- 把文件移動到這些空間裡面。保證敏感文件不再存在於你手機或其他舊的文件夾中。

#### 看看你的旧密码

- 把你的在線賬號的密碼都存儲在密碼管家中。如果你正確安裝了瀏覽器擴展，它會自動在你的登陸過程中把相關的賬號信息都抓取。
- 借助你的密碼管家的分析工具，看看哪些賬號使用了弱密碼，更新那些你認為含有任何個人信息或者你不想遺失的網絡賬號的密碼。

### 💪🏾 養成良好習慣

- 使用[Signal](https://whispersystems.org/)。這是一款支持端對端加密的手機聊天軟件，一般被認為是安全的聊天軟件。除了Signal以外，很少有對安全聊天軟件的共識，人們通常會感性地選擇自己認為最安全的軟件。
- 在打語音或視頻通話時，使用端對端加密的軟件（比如Signal, Jitsi, Wire）。
- 買一部難破解的手提電話，這種電話通常比較昂貴。一般來說，蘋果手機以及使用Google版本Android系統的安卓手機相對安全。

---

**😲 哇，你把最難的網絡安全步驟都走完了，好樣的。**

---

## 💦❗️ 基於特定情境的安全建議

### 🛫 當你需要跨境

- 關閉你的設備，因為：
  - 存儲和硬盤僅僅在關閉狀態下才是加密的，睡眠模式下並非處於加密狀態。
  - 這能保證你的移動設備在開啓時需要密碼才可能登陸，在一些地區你的密碼受言論自由等法律的保護。
- 在你的設備上存儲盡可能少的信息。如果你的設備被扣留了，其他人無法獲取你沒有存儲的信息。
- 謹慎選擇你在設備上貼的貼紙，海關人員可能會認為這些貼紙代表可疑信息和行動。
- 把你的航班信息和事件告訴你的朋友。如果你在指定時間沒有出現的話讓他們聯繫律師及有關機構。
- 如果你面臨的是高風險的情況（以下這些措施有可能會引起懷疑，讓你的情況更糟）：
  - 另外建立一個相冊，郵件地址，和社交媒體賬號，這些賬號里都是沒有可疑的內容。
  - “忘記” 你的密碼：為你的設備和賬號上密碼鎖，只有你信賴的朋友有另一半密碼。
  - 登出你所有的重要賬號（或者直接把你的設備放在家中）。
- 如果想瞭解更多信息，看以下這兩篇有關如何在美國邊境要求律師協助的文章：Wired's [Guide to Getting Past Customs With Your Digital Privacy Intact](https://www.wired.com/2017/02/guide-getting-past-customs-digital-privacy-intact/) 和 [BoingBoing's addendum](http://boingboing.net/2017/02/12/how-to-cross-a-us-or-other-b.html) 。

---

### 😭 有人拿走了我的手機/電腦！

- 遠程清除你手機上的所有信息：[Android](https://support.google.com/accounts/answer/6160491?hl=en), [iOS](https://support.apple.com/kb/PH2701?locale=en_US)的教程。
- 用其他設備登出你所有的重要賬號。
- 如果這發生在跨過邊境：要求對方提供扣留收據（僅在某些國家有效，如[加拿大](https://bccla.org/wp-content/uploads/2018/10/Electronic-Devices-Privacy-Handbook-BCCLA_2.0.pdf)）。
- 獲取新的電話卡。
- 如果你重新獲得你的設備，恢復出廠設置。使用反病毒和反間諜軟件確保你的設備沒有可疑軟件。

---

### 👾 我覺得我的電腦被入侵了！

- 下載一個能在你的數據被發送到其他設備時提示你的軟件，如 [Little Snitch for Mac](https://www.obdev.at/products/littlesnitch/index.html).
- 蘋果電腦上運行 “活動監視器“（Activity Monitor）或者Windows系統上的 ”進程瀏覽“ （Process Explorer），查看有那些進程正在運行。搜索那些看起來可以的名字。
- 登陸重要的網絡賬號，查看是有其他可疑登陸，詳細教程在這裡閱讀：[Motherboard:  How to Tell if Your Account Has Been Hacked](https://motherboard.vice.com/en_us/article/bjeznz/how-do-you-know-when-youve-been-hacked-gmail-facebook)。
- 使用一部閒置的智能手機運行[Haven](https://guardianproject.github.io/haven/) ，這個軟件可以幫助你偵測入室行為。

---

### 🍆 性短信及無共識的照片分享

- 查看 [The Motherboard Guide to Sexting Securely](https://motherboard.vice.com/en_us/article/mb3nd4/how-to-sext-securely-safely-what-apps-to-use-sexting).

---

### ✊🏾 如果你要參與遊行

#### 如果出現緊急狀況

- 前把求助信息和收件人放在草稿箱，收件人應該是你信賴的並且不再遊行現場的朋友或者是法律熱線。在你被捕或者有緊急情況時及時發出。
- 隨身攜帶你手機的後備電池。
- 如果你使用指紋或者面部解鎖，你被捕後要馬上關閉你的手機。在某些國家和地區，[執法人員可以強制你提供你的指紋但不能強制你提供密碼](https://www.theatlantic.com/technology/archive/2016/05/iphone-fingerprint-search-warrant/480861/)。事實上，最好在你參與遊行之前就把面部識別功能關閉。
- 如果你參與的是高風險示威活動：把你的設備留在家中，或者使用一次性手機。

#### 分享少之又少的信息

- 存儲盡可能少的個人信息或者對你不利的信息，你永遠不知道你的設備會落在誰的手上。
- 如果你的聊天軟件支持閱後即焚，請開啓這個設置。
- 如果你需要分享照片，用[這些軟件](https://www.maketecheasier.com/best-apps-remove-exif-data-from-images/)清除所有元數據。
- 關閉定位歷史：
- - iPhone: Settings > Privacy > Location Services > System Services > Significant Locations
  - Android: Settings > Google > Google Account > Data & personalization > Location History > Manage setting > Your account & all your devices > turn off Use Location History
  - Google 地圖: Settings > Maps history > Web & App Activity
- 刪除過去的定位歷史：
  - iPhone: Settings > Privacy > Location Services > System Services > Significant Locations > Clear History
  - [Android](https://support.google.com/accounts/answer/3118687?hl=en#delete)
  - [Google 地圖](https://support.google.com/maps/answer/3137804?hl=en)

#### 其他

- 再三確認你的聊天軟件的隱私設置。
- 關閉信息預覽功能：
  - iOS: Settings > Notifications > Show Previews: When Unlocked
  - Android: Settings > Apps & notifications > Notifications > On lock screen: Hide sensitive content
- 記得使用如Signal和Whatsapp等端對端加密軟件進行語音通話。
- 更多關於[在美國](https://ssd.eff.org/en/module/attending-protests-united-states)和[其他地方](https://ssd.eff.org/en/module/attending-protests-international)遊行的信息可以看EFF網站（英文）。

---

### 📰 我是報道敏感議題的記者

以下是一些所有記者都要考慮實踐的基本安全設置。如果你報道的是特別敏感的議題或地區（如在美國報道「吹哨人」故事或做與中國相關的報道），你和你的團隊需要按需向專家咨詢。

#### 時刻做好以下準備

- 通過跟蹤軟件遠程清除你設備上的內容（如蘋果上的 [Find My](https://www.apple.com/icloud/find-my/) ，Android [Find My Device](https://support.google.com/accounts/answer/6160491?hl=en)， [Prey](https://www.preyproject.com), [Lookout Security](https://www.lookout.com/)）。
- 成為釣魚郵件的接收者（記者本來就比其他人收到更多的郵件）。

#### 保護自己

- 如果你正在旅途中，閱讀上述`當你需要跨境`情境的安全建議。
- 如果你要報道一場示威運動，閱讀上述`如果你要參與遊行`情境的安全建議，自行判定你需要作出哪些安全措施以及哪些記者權利適用於你。
- 果你在辦公室上網，使用VPN。網管通常可以看到你來自哪裡，舉個例子，他們可以看到你來自紐約時報的網絡。

#### 保護你的信源

- 用 [Signal](https://www.signal.org/) 或 [Jitsi](https://jitsi.org/) 進行端對端加密的視頻和音頻通話。
- 如果你的聊天軟件支持閱後即焚功能，開啓這個功能。如果沒有開啓，記得定期清空聊天記錄和歷史。
- 讓你的機構設置 [SecureDrop](https://securedrop.org/)。如果沒有設置或無法設置的話，鼓勵人們使用OnionShare](https://onionshare.org/)或 [Firefox Send](https://send.firefox.com/)。
- 模糊處理照片和視頻中的人臉 (如Android [ObscuraCam](https://guardianproject.info/apps/obscuracam/), Youtube [教程](https://technology.witness.org/2016/02/how-to-use-youtubes-new-blurring-feature-to-protect-identities/))。
- 用[這些軟件](https://www.maketecheasier.com/best-apps-remove-exif-data-from-images/)刪除多媒體的元數據。
- 閱讀Ted Han 和 Quinn Norton的 [Protecting Your Sources When Releasing Sensitive Documents](https://source.opennews.org/articles/how-protect-your-sources-when-releasing-sensitive-/).
- 閱讀Martin Shelton的 [Opening Secure Channels for Confidential Tips](https://source.opennews.org/articles/opening-secure-channels-confidential-tips/).

#### 保護你的數據

- 確保你正在使用的郵件和存儲空間服務商的所有人不是你正在報道的國家或者機構，也不存在與這些國家和機構的任何聯繫。
- 最好把你所有與你工作相關的內容移到端對端加密平台，比如電子郵件[Protonmail]([https://protonmail.com/](https://protonmail.com/) 或者 [Tutanota](https://tutanota.com/), 雲儲存 [Tresorit](https://tresorit.com/) 或 [SpiderOak](https://spideroak.com/)。注意[法院能夠強制谷歌交出你的所有數據](https://medium.com/@tinfoilpress/newsrooms-lets-talk-about-g-suite-1672a36eb235)。
- 盡可能把所有敏感數據存放在帶密碼的雲盤或者移動設備上。有關如何加密敏感文件的教程可以看上文`為敏感文件上鎖`。
- 不要忘記從你的電腦上永久刪除敏感文件，可以選擇使用 [Eraser for Windows](https://eraser.heidi.ie/) 或 [File Shredder for Mac](https://apps.apple.com/us/app/fileshredder/id418094085?mt=12)。

#### 更多信息

- 如果你處於非常規的國家，地區或面臨不一樣的情境，閱讀Grégoire Pouget of Nothing2Hide's 的這篇指南： [Digital Security for Journalists Requires an Adaptable Toolkit](https://gijn.org/2019/07/16/digital-security-for-journalists-requires-an-adaptable-toolkit/)。
- 如果你運營一個新聞編輯團隊，閱讀 Ontheline Newsrooms 的 [Measures for Newsrooms and Journalists to Address Online Harassment](https://newsrooms-ontheline.ipi.media/).

---

### 🕵🏼‍♂️ 人肉搜索/起底和網絡暴力

根據你的攻擊者，人肉搜索/起底和網絡暴力可以是非常具體和複雜，它可以包含你的工作等與你相關的所有信息。雖然我們提供了以下這些一般建議，但我們強烈建議你判定你的情況有沒有升級到需要與專家進行一對一咨詢。

#### 找一個你信任的朋友

- 不要自己把自己困起來，獨自面對這些情況。
  - 最基本的，找一個你信任的朋友作你的支撐，並分析情況有多糟糕。
  - 同時，我們建議你找一個你信任的朋友幫你調查，記錄，舉報和屏蔽騷擾者。你可以閱讀 Take Back The Tech's [Hey Friend!](https://www.takebackthetech.net/know-more/heyfriend) 這篇指南。有時候，交出你的手機和社交媒體帳號或許對你更有用，因為你的創傷不會總是被刺激。
- 另外，你可以向你所身處的網絡社群尋去幫助。閱讀PEN America的這篇文章：[Deploying Your Supportive Cyber Communities](https://onlineharassmentfieldmanual.pen.org/cyber-safety/deploying-your-supportive-cyber-communities/).
- 如果沒有人能馬上幫助你，Heartmob提供了一份[支援機構的清單](https://iheartmob.org/resources/supportive_organizations)，其中一些提供24小時服務。

#### 跟蹤任何更新，收集清單

- 設置 [Talkwalker](https://www.talkwalker.com/alerts) 和 [Google Alerts](https://www.google.com/alerts)追蹤你的名字和暱稱。
- 用你認為最簡單的軟件清楚記錄每一起網絡暴力（日期，時間，描述，截屏）。

#### 從互聯網上移除你的個人信息

- 给[PrivacyDuck](https://www.privacyduck.com/) 付費，清除你在網上的信息。如果你是運動家，你可以聯繫[Equity Labs](https://medium.com/@EqualityLabs/anti-doxing-guide-for-activists-facing-attacks-from-the-alt-right-ec6c290f543c)，獲取折扣價。
- 给[Reputation.com](https://www.reputation.com/) 付費， 從付費網站上移除你的信息，並後續跟蹤這些網站，確保信息保持移除。
- 你也可以用 [PrivacyDuck](https://www.privacyduck.com/resources/) 和 [Motherboard](https://motherboard.vice.com/en_us/article/ne9b3z/how-to-get-off-data-broker-and-people-search-sites-pipl-spokeo) 的免費資源幫助你移除相關信息。

#### Obscure your personal information

- 使用 [Burner](http://www.burnerapp.com/)獲取一次性號碼來打電話或發短信。
- 用[Traveling Mailbox](https://travelingmailbox.com/) 隱藏你的真實郵編。
- 刪除所有老舊網絡帳號。用[Justdelete.me](http://justdelete.me) 幫助你實現這個過程。
- 檢閱你的社交媒體帳號，刪除所有過多個人信息的帖子，比如那些涉及你的住址，你去哪裡，和誰去等信息。
- 如果你是Twitter用戶：
  - 求助於你的社區，建立一個[屏蔽清單](https://help.twitter.com/en/using-twitter/advanced-twitter-block-options)，屏蔽那些為人熟知的攻擊者。
  - 用[Semiphemeral](https://micahflee.com/2019/06/semiphemeral-automatically-delete-your-old-tweets-except-for-the-ones-you-want-to-keep/) 刪除你不想要的推文（需要使用命令列介面）。

#### 忽視/回應/舉報/屏蔽對你網絡暴力的攻擊者

- 基於你對網絡暴力事件的記錄，以及你朋友的支持，確定你想要採取的應對策略（這些策略並非惟一的）：
  - 忽視：如果得不到任何注意，有時施暴者會自然而然地離開。
  - 降級：有時你可以使用冷靜的語言在事件變得更壞前降溫。
  - 舉報：向平台或者有關的執法部門舉報實施網絡暴力的人。
  - 在社交媒體靜音（mute）你的攻擊者：讓你自己可以有個清淨。
  - 在社交媒體封鎖/屏蔽（block）你的攻擊者：你的攻擊者將無法看到你的帖子。但注意，你的攻擊者可以知道你封鎖/屏蔽了它們，並認為這是在升級事件。
  - 公開事件：有可能帶來危險，但有時候公開譴責他們的行為並獲取公眾支持能使他們停止暴力。

#### 更多信息

- Feminist Frequency: [Speak Up & Stay Safe(r)](https://onlinesafety.feministfrequency.com/en/).
- TrollBusters: [What to Do? Where to Go? Infographic](https://yoursosteam.wordpress.com/what-to-do-infographic/).
- Equity Labs: [Anti-Doxing Guide for Activists Facing Attacks from the Alt-Right](https://medium.com/@EqualityLabs/anti-doxing-guide-for-activists-facing-attacks-from-the-alt-right-ec6c290f543c).
- HeartMob/Hollaback: [Technical Safety Guide](https://iheartmob.org/resources/tech).
- Crash Override (RIP): [So You've Been Doxed](http://www.crashoverridenetwork.com/soyouvebeendoxed.html), [Preventing Doxing](http://www.crashoverridenetwork.com/preventingdoxing.html).

---

### 👤 我不想給在線約會/交友/組織提供我的真實手機號碼

有些軟件需要用你的手機號碼註冊（如Signal和Whatsapp），你可以通過以下這些渠道獲得第二個手機號碼：

- [Twilio](https://www.burnerapp.com/) (1 USD/月, 設置過程相對複雜，可以閱讀[這裡](https://medium.com/@geminiimatt/creating-an-online-persona-deb4cd8c7f46) 以及 [這個指南](https://source.opennews.org/articles/shields-using-signal-without-your-phone-number/))
- [Burner](https://www.burnerapp.com/) (5 USD/月, 但支持短期預付)
- [Google Voice](https://voice.google.com/about) (免費，但僅在美國有效)
- 手機運營商：買一個預付卡，費用不同

但注意：

- 如果你失去或者不再訂閱你的第二個手機號碼，其他人可以購買這個號碼並盜用你的身份。
- 絕大部分的公司會把你的信息交給相關部門，如果後者有提供正確的請求文件。

#### 要做到完全匿名，使用假名建立一個無法被追蹤的網絡身份

- 如果你是公眾人物，藝術家或者運動活躍人士，你可以考慮用一個假名或者集體身份，閱讀[Tactical Tech manual](https://gendersec.tacticaltech.org/wiki/index.php/Complete_manual#Creating_and_managing_identities_online) 瞭解更多細節。
- 完全安全匿名，使用這個指南：  [creating untraceable online accounts and protecting your real identity](https://medium.com/@geminiimatt/creating-an-online-persona-deb4cd8c7f46).

---

## 💦❓ 其他建議

這部分內容提供相對萬用的安全建議，適用於不面臨以上幾種情境的普通用戶。

#### 電子郵件

- 設置 [Protonmail](https://protonmail.com/) 或 [Tutanota](https://tutanota.com/) 進行端對端加密郵件。
- 瞭解你的風險，使用PGP郵件（[近期有發現PGP郵件的安全漏洞](https://www.eff.org/deeplinks/2018/05/not-so-pretty-what-you-need-know-about-e-fail-and-pgp-flaw-0)，說明這一選項不再是完全安全）。

#### 設備權限

- 購買 [YubiKey](http://www.amazon.com/Yubico-Y-072-YubiKey-NEO/dp/B00LX8KZZ8/ref=sr_1_1?ie=UTF8&qid=1421839152&sr=8-1&keywords=yubikey+NEO) USB key 來進行二步驗證。
- 用含有字母和數字的密碼來解鎖你的手機。
- [Generating Diceware passwords](http://world.std.com/~reinhold/diceware.html).

#### 文件存儲和共享

- 用端對端加密的雲儲存設備（Dropbox並不是其中之一）：[Tresorit](https://tresorit.com/), [SpiderOak](https://spideroak.com/).
- 使用加密的移動硬盤和USB，[Apricorn](https://www.apricorn.com/)等公司有提供這些硬件。
- 如果你需要匿名發送文件，使用特殊的文件共享服務，如 [OnionShare](https://onionshare.org/)等。
- 使用 [CryptPad](https://cryptpad.fr) （開源，端對端加密）而非谷歌文件和微軟辦公室。

#### 聊天軟件

- WhatsApp 設置：
  - 要100%實現端對端加密，關閉聊天記錄備份 (Settings > Chats > Chat backup) 並刪除你之前的備份 ( [iOS](https://www.wikihow.com/Delete-Backups-on-WhatsApp-on-iPhone-or-iPad), [Android](https://faq.whatsapp.com/en/android/30030306)).
  - 在Whatsapp上開啓安全通知 (Settings > Account > Security)
  - 設置一個密碼，防止你的帳號在你不知情的情況下被移動(Settings > Account > Two-Step Verification)
- 如果你是經常使用Signal的記者，閱讀Martin Sheldon's [Locking Down Signal](https://medium.com/@mshelton/locking-down-signal-d71678f653d3) 指南進一步加強你的安全措施，或者[這篇針對Whatsapp](https://medium.com/@mshelton/upgrading-whatsapp-security-386c8ce496d3)的指南。

#### 其他

- 確保你的設備上有盡可能少的信息，數據，或照片。
- 不要使用智能电视或者智能音箱。
- 用[DuckDuckGo](http://duckduckgo.com/)匿名搜索。
- 如果你或者你的機構深度使用Google Suite，考慮Google的[Advance Protection program](https://www.wired.com/story/google-advanced-protection/)。
- 把你的信用卡，護照，設備等放在法拉第籠（Faraday Bag）里，它可以屏蔽任何信號傳輸。 ([Micah Lee 的指南](https://micahflee.com/2015/11/some-thoughts-on-faraday-bags-and-operational-security/).)
- 為你自己的Wordpress網站增強保護： [Cloudflare](https://www.cloudflare.com) + [iThemes Security](https://wordpress.org/plugins/better-wp-security/).
- 使用更安全的操作系統： [Tails](https://ssd.eff.org/en/module/keeping-your-data-safe) (可以通過ＵＳＢ盤使用) 或者 [Qubes OS](https://www.qubes-os.org/).
- Android用戶可以通過[F-Droid](https://f-droid.org)下載軟件，[F-Droid](https://f-droid.org)是一個開源的注重安全的應用軟件市場。
- 對於美國居民，凍結你的信用信息，防止黑客獲取敏感數據。閱讀更多信息： Security Checklist's [Freeze Your Credit](https://securitycheckli.st/)。

---

**🏆 你閱讀了整份文檔！太棒了！**

---

## 🧠 來源

我們咨詢了許多專家，並總結了自己的經驗來建立這份清單（你可以在這裡查看我們的[所有信息來源](https://github.com/hongkonggong/tldr-digital-security/blob/master/SourcesConsulted.md)）。如果你還是沒有獲得你希望獲得信息，我們建議你閱讀以下這些文章：

- [The Motherboard Guide to Not Getting Hacked](https://motherboard.vice.com/en_us/article/d3devm/motherboard-guide-to-not-getting-hacked-online-safety-guide)
- [The Electronic Frontier Foundation's Surveillance Self-Defense](https://ssd.eff.org/)
- [Holistic digital security training curriculum for women human rights defenders](https://cyber-women.com/en/)
- [Matt Mitchell 的 Twitter](https://twitter.com/geminiimatt/)
- [Rory Peck Trust's Digital Security guide for freelance journalists](https://rorypecktrust.org/freelance-resources/digital-security/)

你可以閱讀 Martin Shelton整理的指南： [Current Digital Security Resources](https://medium.com/@mshelton/current-digital-security-resources-5c88ba40ce5c)。

---

## 📝 授權

本著作係採用[創用 CC 姓名標示-非商業性-相同方式分享 4.0 國際 授權條款](https://creativecommons.org/licenses/by-nc-sa/4.0/)授權.

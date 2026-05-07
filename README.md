# 📇 Page Maker - Multi-ID A4 Generator Bot

A powerful Telegram bot designed to arrange multiple ID cards (front & back pairs) onto a single A4 page for professional printing. Fully optimized for memory-constrained environments and high-security data privacy.

## 🚀 Key Features

### 1. Professional A4 Layouts
- **Auto-Pairing**: Upload front and back images, and the bot automatically pairs them.
- **5-Pair Capacity**: Generates a standard A4 sheet with up to 5 ID pairs (10 images total).
- **Multiple Formats**: Export your results as **PDF**, **JPG**, **PNG**, or **TIFF**.

### 2. Precise Sizing & Presets
- **Ready-to-Print**: Defaults to the standard **85.5 x 54 mm** ID size.
- **Preset Buttons**: One-click selection for common sizes (Standard ID, Size 1, Size 2).
- **Private Presets**: Save your favorite custom sizes as personal presets with a nickname. Only you can see them!
- **Custom Manual Entry**: Type your own dimensions (e.g., `1000 * 600 px` or `8.5 * 5.5 cm`).
- **Layout Control**: Adjust side gaps, vertical gap levels (1-4), and top margins to fit any sticker paper.

### 3. Interactive Admin Dashboard (`/admin`)
- **User Management**: View active users and block/unblock IDs with a single click.
- **Dynamic Presets**: Manage default size choices (Add/Delete) directly from the Telegram UI.
- **Rich Broadcast**: Send messages or media to all users instantly by replying to any post with `/broadcast`.

### 4. Privacy & Optimization
- **Auto-Purge**: All uploaded source images and generated output files are **deleted physically** from the server as soon as the job is finished.
- **Memory Efficiency**: Hardened Sharp configuration for running on shared hosting (CPanel/Back4App).
- **Reliability**: Internal tracking prevents duplicate processing of the same message or button click.

---

## 📖 User Manual

### How to Print a Page
1. **Send Images**: Upload your ID images as "Photos" or "Documents".
2. **Label Them**: 
   - Reply to an image with `front` or `back`.
   - OR send images with `front` or `back` in the caption.
3. **Check Status**: Use `/status` to see how many pairs are ready.
4. **Print**: Click the **📄 Print** button on your keyboard.
5. **Orientation**: Choose **Normal** or **Flip + Reverse** (for double-sided printing alignment).

### Configuring Settings
1. Type `/settings` or click **⚙️ Settings**.
2. **Set Size**: Choose a preset or enter dimensions manually.
3. **Margins/Gaps**: Click the buttons to cycle through pre-set gap and margin levels.
4. **Format**: Toggle between PDF, JPG, etc.
5. **Restore**: Use **Restore Defaults** to jump back to the standard 85.5x54mm layout.

### Admin Guide (For Owners)
- **Dashboard**: Use `/admin` for a button-driven control panel.
- **Blocking**: In the "Users" menu, click **🚫 Block** to blacklist an ID.
- **Presets**: In the "Presets" menu, delete old ones or see the format to add new ones.
- **Adding a Preset**: Use `/addpreset <Name> <W> <H> <Unit> <GapChoice>`
  - *Example*: `/addpreset IDCard 85.5 54 mm small`

---

## 🇪🇹 የአጠቃቀም መመሪያ (በአማርኛ)

**እንኳን ወደ Page Maker Bot በሰላም መጡ!** ይህ ቦት መታወቂያዎችን በአንድ የ A4 ወረቀት ላይ በአግባሁ አቀናጅቶ ለማተም ይረዳዎታል።

### እንዴት መጠቀም ይቻላል?
1. **ፎቶዎችን ይላኩ**፦ የታተሚውን መታወቂያ ፎቶ ይላኩ።
2. **ምልክት ያድርጉ**፦
   - ለፊተኛው ገጽ፦ ፎቶውን ከላኩ በኋላ `front` ብለው ይጻፉ (ወይም በፎቶው መግለጫ/caption ላይ `front` ይበሉ)።
   - ለጀርባው ገጽ፦ ፎቶውን ከላኩ በኋላ `back` ብለው ይጻፉ።
3. **ሁኔታውን ይመልከቱ**፦ `/status` የሚለውን በመጫን ስንት መታወቂያዎች እንደተዘጋጁ ማየት ይችላሉ።
4. **ለማተም (Print)**፦ **📄 Print** የሚለውን ቁልፍ ይጫኑ። ቦቱ በጥቂት ሰከንዶች ውስጥ የተዘጋጀውን ፋይል ይልክልዎታል።

### ጠቃሚ መረጃዎች
- **የግል መጠን (Private Presets)**፦ የራስዎን የተለየ መጠን በስም መዝግበው ማስቀመጥ ይችላሉ። ይህ መጠን ለእርስዎ ብቻ የሚታይ ነው።
- **ማስተካከያ (Settings)**፦ የመታወቂያውን መጠን ለመቀየር `/settings` የሚለውን ይጫኑ።
- **ደህንነት**፦ ቦቱ ስራውን እንደጨረሰ የላኩትን ፎቶዎች ወዲያውኑ ከሰርቨሩ ላይ ያጠፋል።

---

## 🛠️ Installation & Deployment

### Local Setup
1. Clone the repository.
2. Run `npm install`.
3. Create a `.env` file with your `BOT_TOKEN`.
4. Run `npm start`.

### Deployment Docs
- See [DEPLOYMENT.md](file:///d:/ALL projects/all Nid/Page maker/orderidbot/DEPLOYMENT.md) for general VPS setup.
- See [BACK4APP-DEPLOYMENT.md](file:///d:/ALL projects/all Nid/Page maker/orderidbot/BACK4APP-DEPLOYMENT.md) for serverless hosting.
- See [CPANEL-MEMORY-FIX.md](file:///d:/ALL projects/all Nid/Page maker/orderidbot/CPANEL-MEMORY-FIX.md) for shared hosting memory limits.

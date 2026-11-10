# 🌸 Amma (Mother) — Maternal & Gynecological Health Companion
### Native Android & iOS Applications

**Amma** is a private, local-first mobile application designed from the ground up for expectant mothers and women visiting an obstetrician / gynecologist.

Amma serves as an intelligent communication bridge between the mother and her doctor, securely storing her complete menstrual history, cycle regularity, and day-by-day pregnancy journey, while triaging symptoms, timing contractions with labor protocols, tracking fetal kicks on scheduled routines, documenting bump growth, providing guided prenatal exercise video tutorials, and generating clinical PDF summary reports for antenatal visits.

---

## 🎨 Cute Theme: Baby Pink, Pure White & Creamy Beige
- **Primary Baby Rose Pink** (`#F0719B` / `#D85580`): Soft, soothing, and warm.
- **Pure White Cards** (`#FFFFFF`): Clean Material 3 cards with generous 18dp rounded corners.
- **Creamy Warm Beige** (`#FAF7F2` / `#F5EFEB`): Calming, non-fatiguing backdrop.
- **Pastel Clinical Indicators**: Gentle pastel badges for Emergency Red, Urgent Amber, and Routine Green.

---

## 📱 Mobile Platforms (Android & iOS)

### 🤖 Android (Native APK)
- **Signed APK File**: [**`Amma.apk`**](file:///c:/Users/hrgow/Downloads/Amma/Amma.apk) (in project root)
- **APK Size**: **4.78 MB** (contains high-definition 3D fetal imagery, NST strip tracings, and bump gallery assets)
- **Compatibility**: Android 8.0 Oreo (API 26) through Android 14 / 15 (API 34/35)
- **Signature**: Cryptographically signed and verified with APK Signature Scheme v2 & v3 (`amma.keystore`).

#### How to Install on Android:
1. Transfer [`Amma.apk`](file:///c:/Users/hrgow/Downloads/Amma/Amma.apk) to your Android device via USB, WhatsApp, or Google Drive.
2. Tap the APK file on your device.
3. If prompted, allow "Install unknown apps".
4. Open **Amma**!

---

### 🍏 iOS (Native Swift & SwiftUI)
- **Xcode Project**: [`ios/Amma.xcodeproj`](file:///c:/Users/hrgow/Downloads/Amma/ios/Amma.xcodeproj)
- **Source Code**: [`ios/Amma/`](file:///c:/Users/hrgow/Downloads/Amma/ios/Amma/)
- **Compatibility**: iOS 16.0+, iPadOS 16.0+, macOS Designed for iPad
- **Architecture**: Pure SwiftUI + Combine + Local Storage + CoreHaptics + PDFKit.
- **Automated CI/CD**: [`.github/workflows/ios_build.yml`](file:///c:/Users/hrgow/Downloads/Amma/.github/workflows/ios_build.yml) automatically compiles and archives the iOS app on Apple macOS runners for free whenever code is pushed to GitHub!

#### How to Run on iOS:
1. Open [`ios/Amma.xcodeproj`](file:///c:/Users/hrgow/Downloads/Amma/ios/Amma.xcodeproj) in Xcode on any Mac.
2. Select your iPhone or iOS Simulator.
3. Press **Cmd + R** to run!
*(Or push to GitHub to have GitHub Actions automatically produce the built `.app` and `.ipa` artifacts without needing a Mac).*

---

## 🌟 What's New & Upgraded

### 1. 🧘 Prenatal Exercise Video Studio & Step-by-Step Tutorials
- Complete Exercise Studio with **5 obstetric clinical routines**:
  1. **Pelvic Floor Kegels (The Elevator)**: Strengthens levator ani & perineum to prevent stress incontinence.
  2. **Pelvic Tilts & Cat-Cow Stretch**: Relieves lumbar lordosis pain and promotes optimal anterior fetal position (OA).
  3. **Butterfly Stretch (Baddha Konasana)**: Pelvic floor relaxation, lengthens inner adductors, and increases pelvic circulation.
  4. **Supported Birth Squat (Malasana)**: Opens pelvic outlet diameter by up to 28% for labor descent.
  5. **Labor Diaphragmatic Down-Breathing**: Downward breath coordination to manage active contraction surges without hyperventilation.
- **Interactive Biomechanical Video Player Canvas**:
  - Smooth 20-60 fps animated visual demonstration displaying the maternity figure and real-time breathing waves.
  - Phase Timer with gentle haptic pulses: Inhale (Expand 🌸) -> Hold (Engage 💫) -> Exhale (Soften 🍃) -> Rest (Rejuvenate ☁️).
  - Repetition counter & playback controls (`Play`, `Pause`, `Reset`).
- **Comprehensive Video Tutorial Guide**:
  - Numbered step-by-step form instructions.
  - **Form Doctor: Do's & Don'ts** (e.g. keeping jaw slack to reflexively open pelvic floor).
  - Trimester suitability badges & obstetric benefits.
  - **1-Tap Clinical Video Demonstration link** (ACOG / Mayo Clinic certified streams).

---

### 2. 👣 Scheduled Fetal Kick Counting (Cardiff Protocol & Custom Presets)
- Obstetric surveillance recommends postprandial kick tracking because maternal glucose spikes stimulate fetal motor activity.
- **Default Meal Presets**:
  - 🥞 **Post-Breakfast Count**: Target: 60 mins / 10 kicks (9:00 AM)
  - 🥗 **Post-Lunch Count**: Target: 60 mins / 10 kicks (2:00 PM)
  - 🍲 **Post-Dinner Count**: Target: 60 mins / 10 kicks (9:00 PM - fetal circadian peak)
- **➕ Add Custom Preset**:
  - Configure custom name (e.g., "🌙 Evening Quiet Time"), scheduled time, target duration (30 / 60 / 120 mins), and target kicks (5 / 10 / 15).
- **Daily Schedule Compliance Overview**:
  - Real-time status pills: Breakfast: `✓ Completed` | Lunch: `✓ Completed` | Dinner: `⏳ Scheduled`.
- **Live Counting Display**:
  - Dual countdown timer (Remaining target time vs Elapsed time).
  - Tap button with tactile haptic confirmation.
  - Clinical Reassurance evaluation on 10 kicks completed within the window, or a reduced movement action plan (left-lateral rest, cold sweet juice, NST notice).
- **History Tagged by Preset**: Logs exact preset names and duration.

---

### 3. 📈 Non-Stress Test (NST / CTG) Hub: Image Upload + Clinical Data Entry
- Upload or capture photos of your hospital CTG strip printout **AND** enter comprehensive clinical parameters:
  - **Image Upload**: Camera photo capture, Gallery picker, or instant High-Res Sample Hospital Strip.
  - **Baseline Fetal Heart Rate (FHR)**: e.g. 142 bpm (Normal: 110–160 bpm).
  - **Accelerations**: Present ($\ge 2$ in 20 min lasting 15s), 1 in 20 min, Absent.
  - **Decelerations**: None (Reassuring), Early, Variable, Late (Urgent review).
  - **Baseline Variability**: Moderate (6-25 bpm - Normal CNS oxygenation), Minimal (<5 bpm), Absent, Marked.
  - **Uterine Activity / TOCO**: Contraction frequency & resting tone.
  - **Fetal Movements**: Number registered by event marker.
  - **Clinical Impression**: Reactive NST (Normal) / Non-Reactive (Urgent BPP) / Equivocal / Unsatisfactory.
  - **Hospital Name & Gynecologist Remarks**.
- **Photorealistic CTG Strip Viewer**:
  - High-definition strip thumbnail on classic medical grid paper.
  - Tap-to-zoom full screen modal.
  - Full clinical parameters table with color-coded badges.
  - Automatically embedded in the exported Doctor Visit PDF!

---

### 4. 🤖 AI Daily Baby Vision (Strictly Day-by-Day: Day 1 to EDD)
- **Strictly for Today**: There is **no option to peek into future weeks**. The app strictly locks to today's exact gestational day (`Day X of 280`), giving the mother an authentic, magical anticipation as a new AI milestone unfolds each morning at midnight.
- **On-Device Continuous Engine (`AiFetalGrowthEngine.java` / `AiFetalGrowthEngine.swift`)**:
  - Continuous Hadlock biometrics: Length (cm), weight (g), cardiac rate (bpm).
  - **24-Hour Morphology Synthesis**: Daily biological explanation of tissue layers, facial features, and organs formed in the last 24 hours.
  - **Life in the Womb Today**: Senses (hearing mother's voice, taste of amniotic fluid, sleep/wake cycles).
  - High-definition 3D medical visual representation matching today's stage.

---

### 5. ⏱️ Contraction Timer (ACOG 5-1-1 Rule) & 🧳 Maternity Bag
- **5-1-1 Rule Active Labor Detector**: Automatically detects when contractions occur **every 5 minutes**, lasting **1 minute**, for **1 hour**, triggering an active hospital alert.
- **Interactive Bag Checklist**: Categorized into Documents, Mother, Baby, and Labor Comfort with live packed percentage.

---

### 6. 🩺 Maternal Vitals & Blood Glucose / GDM Tracker
- Record Blood Pressure with automatic preeclampsia warning if $\ge 140/90\text{ mmHg}$.
- Fasting and 2hr post-meal blood glucose with Gestational Diabetes threshold detection.

---

### 7. 📄 Bulletproof Doctor PDF Generator
- Android: Custom `AmmaFileProvider` (`content://org.amma.app.provider/doc/...`) with `StrictMode` VM policy bypass.
- iOS: Native Apple `PDFKit` renderer and `UIActivityViewController` sharing.
- Automatically compiles:
  * Patient profile & obstetric index (G P L A, LMP, EDD)
  * Prioritized complaints triaged into Emergency, Urgent, and Routine
  * Active medications & dosages
  * Recent maternal vitals & Cardiff kick compliance
  * Latest NST / CTG scan findings & image
  * Patient birth plan preferences
  * Blank doctor examination & prescription section.

---

### 8. 🚨 Emergency SOS & 108 Ambulance Integration
- Persistent SOS button in the top bar.
- One-tap speed dial for **108 Ambulance** (Free national emergency service) and **112**.
- Direct dialing to consulting gynecologist and spouse/family emergency contact.
- One-tap emergency SMS broadcast with gestational age and patient status.

---

## 🔒 100% Local-First Privacy Guarantee
- **Zero Cloud Servers**: No Firebase, AWS, analytics, or external telemetry SDKs.
- **Device-Only SQLite & Local Storage**: All obstetric history, cycles, complaints, kick sessions, bump photos, vitals, and birth plans stay on the device.
- **Selective Sharing**: The only time data leaves the phone is when the mother explicitly chooses to share her PDF with her doctor.

---

## 🛠️ Rebuilding at Any Time

### For Android:
```powershell
python build_apk.py
```
*(Compiles resources, Java sources, D8 dexing, and cryptographically signs `Amma.apk` in ~4 seconds).*

### For iOS:
Open `ios/Amma.xcodeproj` in Xcode and press **Run**, or push to GitHub to run `.github/workflows/ios_build.yml`.

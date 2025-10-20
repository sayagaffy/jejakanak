**JejakAnak - Dummy Web Prototype Master Plan**

**Executive Summary**

Sebelum memulai development aplikasi Flutter final, kita akan membangun **dummy web application** sebagai high-fidelity interactive prototype. Dummy web app ini akan meniru fitur dan user interface dari aplikasi real menggunakan front-end code dan realistic placeholder data. Tujuan utama adalah **memvalidasi requirements dan design** dengan team dan stakeholders secara early, memastikan semua orang memiliki pemahaman yang clear tentang functionality sebelum heavy development dimulai.

**Manfaat Utama**:

- ![ref1] **Validate Requirements**: Confirm semua fitur yang direncanakan benar-benar dibutuhkan
- ![ref1] **Test UX Flow**: Identifikasi friction points dalam user journey
- ![ref1] **Stakeholder Alignment**: Psikolog, educator, dan parent tester dapat memberikan feedback konkret
- ![ref1] **Reduce Development Risk**: Catch issues sebelum invest banyak resource di coding
- ![ref1] **Accelerate Development**: Blueprint yang jelas untuk developer (reference design)

**Timeline**: 2-3 weeks (Week 1-3 dari project roadmap)

**Deliverables**:

1. Clickable web prototype dengan semua key screens
1. Realistic dummy data (30-50 activities, 3-5 sample children with logs)
1. Validation report dari psikolog team, Uwa Farah team, dan parent testers
1. Refined requirements dan design ready untuk development![ref2]
1. **Objectives & Success Criteria**
1. **Primary Objectives**

**Requirement Validation**:

- Confirm ALL functional requirements dari masterplan implemented correctly
- Identify missing features atau edge cases yang belum terpikirkan
- Validate 4E framework implementation (apakah UI-nya jelas untuk parents)
- Ensure prenatal to teen coverage makes sense dalam praktik

**UI/UX Validation**:

- Test navigation flow (apakah intuitive?)
- Validate information architecture (apakah mudah find things?)
- Test onboarding experience (apakah clear untuk first-time users?)
- Ensure activity logging process tidak tedious (friction-free)
- Validate dashboard insights (apakah helpful atau confusing?)

**Stakeholder Buy-In**:

- Psikolog team confirms educational value dan developmental appropriateness
- Uwa Farah team confirms content structure works for their workflow (admin panel)
- Parent testers confirm app solves real problems dan would use regularly
- Tech team confident tentang feasibility

**Design Refinement**:

- Identify UI improvements (layout, colors, typography, iconography)
- Discover missing screens atau modals
- Refine copy/messaging (apakah relatable untuk target audience?)
- Optimize for mobile mental model (even though prototype is web)
2. **Success Criteria**

Prototype dianggap sukses jika:

- ![ref1] All key user flows dapat dilalui dari start to finish
- ![ref1] Psikolog team: "Yes, ini approach-nya educationally sound"
- ![ref1] Uwa Farah team: "Yes, kami understand how to input content"
- ![ref1] Parent testers (5 people): Rata-rata rating 4/5 atau higher untuk usability
- ![ref1] Zero critical confusions (no one says "I don't understand what this app does")
- ![ref1] Tech team: "We're confident we can build this"
3. **Out of Scope (What Prototype Won't Do)**
- ![ref3] **No Real Backend**: Tidak ada database, API, atau server logic. Semua data static/mock
- ![ref3] **No Real Authentication**: Login form exists tapi tidak actual validation (any input diterima)
- ![ref3] **No Actual Photo Upload**: Photo upload UI exists tapi tidak store anywhere (simulate dengan placeholder)
- ![ref3] **No Push Notifications**: Cannot test notification delivery
- ![ref3] **No Real Gamification Calculations**: XP, badges shown tapi tidak calculated dynamically
- ![ref3] **No Performance Testing**: Prototype tidak need to be fast, just functional
- ![ref3] **No Security**: Prototype tidak have secure authentication or HTTPS (local/staging only)![ref4]
2. **Prototype Scope: Key Screens & Flows**
1. **Screen Inventory (Priority Order)**

**MUST HAVE** (Core flows - 15 screens):

1. **Splash Screen**: Logo + tagline
1. **Welcome/Onboarding**: 3 slide carousel (intro, features, benefits)
1. **Sign Up/Login**: Single screen with tabs
1. **Profile Setup**: Parent name, photo upload (mock)
1. **Add Child - Step 1**: Name, status (expecting/born), date picker
1. **Add Child - Step 2**: Photo, gender, notes
1. **Home Dashboard**: Main screen after login
- Child selector (if multiple)
- Recommended activities section
- Scheduled activities
- Quick stats
- Recent memories
8. **Activity Library**: Browse/search view
- Filter bar (age, category, duration)
- Activity cards (grid or list)
9. **Activity Detail**: Full activity information
- Hero image
- Description, materials, steps
- Educational value
- Schedule/Mark as Done buttons
10. **Schedule Activity Modal**: Date/time picker, reminder options
10. **Log Activity - Step 1**: Photo upload interface (mockup)
10. **Log Activity - Step 2**: Notes textarea
10. **Log Activity - Step 3**: 4E feedback toggles
10. **Child Timeline**: Chronological list of logged activities
10. **Child Dashboard (Insights)**: Stats, charts, talent indicators

**SHOULD HAVE** (Important but can be simplified - 8 screens):

16. **Settings**: Notification preferences, account settings
16. **Edit Profile**: Parent and child profile editing
16. **Activity Schedule List**: Calendar view of scheduled activities
16. **Recommendations Explained**: Modal showing why activity was recommended
16. **Badge Showcase**: Grid of earned and locked badges
16. **Challenge Page**: Active and past challenges
16. **Play Spot Detail**: Map view + spot info (simplified)
16. **Help/FAQ**: Static content page

**NICE TO HAVE** (If time permits - 5 screens):

24. **Admin Panel - Dashboard**: Stats for content team
24. **Admin Panel - Create Activity**: Template-based form
24. **Admin Panel - Review Queue**: Pending submissions
24. **Activity Variations Display**: Other parents' contributions
24. **Recipe Exchange Tab**: User-submitted recipes

**TOTAL**: 15-28 screens (depending on time)

2. **User Flow Maps**

**Flow A: First-Time User Onboarding**

Splash (2s auto-advance)Splash (2s auto-advance)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.005.png)

↓↓

WWelcome Screenelcome Screen

├─├─ Slide 1: "Dokumentasikan perjalanan si kecil" Slide 1: "Dokumentasikan perjalanan si kecil"

├─├─ Slide 2: "Aktivit Slide 2: "Aktivitas edukatif teras edukatif ter-kurasi"-kurasi"

└─└─ Slide 3: "T Slide 3: "Temukan bakat anak Anda"emukan bakat anak Anda"

↓↓

`  `[Get Started] button  [Get Started] button

↓↓

Sign Up ScreenSign Up Screen

├─├─ Email + Password fields Email + Password fields

├─├─ OR Social login butt OR Social login buttons (Google, Apple - mockup)ons (Google, Apple - mockup)

└─└─ [Create Account] button [Create Account] button

↓↓

Profile SetupProfile Setup

├─├─ "What's your name?" "What's your name?"

├─├─ Upload photo (placeholder image) Upload photo (placeholder image)

└─└─ [Next] [Next]

↓↓

Add Child - Step 1Add Child - Step 1

├─├─ "T "Tell us about your child"ell us about your child"

├─├─ Name input Name input

`  `├─ Status radio: ![ref5] Expecting (EDD picker) / ![ref5] Born (birth date picker)

└─└─ [Next] [Next]

↓↓

Add Child - Step 2Add Child - Step 2

├─├─ Photo upload (mockup) Photo upload (mockup)

├─├─ Gender dropdown (optional) Gender dropdown (optional)

├─├─ Notes textarea (optional) Notes textarea (optional)

└─└─ [Complete] [Complete]

↓↓

Personalization ModalPersonalization Modal

├─├─ "Help us personalize" "Help us personalize"

├─├─ Notification preferences checkboxes Notification preferences checkboxes

└─└─ [Finish] [Finish]

↓↓

Home Dashboard (with tooltip tour overlay - skippable)Home Dashboard (with tooltip tour overlay - skippable)

**Flow B: Browse & Schedule Activity**

Home DashboardHome Dashboard![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.007.png)

↓↓

Scroll to "Recommended for [Child]" sectionScroll to "Recommended for [Child]" section

↓↓

TTap activity cardap activity card

↓↓

Activity Detail PageActivity Detail Page

├─├─ Swipe through images Swipe through images

├─├─ Read description, materials, steps Read description, materials, steps

├─├─ Expand "Parent T Expand "Parent Tips"ips"

├─├─ See "What They'll Learn" See "What They'll Learn"

└─└─ Action buttons at bott Action buttons at bottomom

↓↓

TTap [Schedule] buttonap [Schedule] button

↓↓

Schedule ModalSchedule Modal

├─├─ Date picker (calendar widget) Date picker (calendar widget)

├─├─ T Time picker (optional)ime picker (optional)

├─├─ Reminder dropdown (15min/1hr/1day before) Reminder dropdown (15min/1hr/1day before) ├─├─ Notes input (optional) Notes input (optional)

└─└─ [Confirm] [Confirm]

↓↓

Toast: "Activity scheduled! ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.008.png)"

↓↓

Return to DashboardReturn to Dashboard

└─└─ New card in "Scheduled Activities" section New card in "Scheduled Activities" section

**Flow C: Log Activity (Core Value Loop)**

Home Dashboard OR Activity DetailHome Dashboard OR Activity Detail![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.009.png)

↓↓

TTap [Mark as Done] buttonap [Mark as Done] button

↓↓

Log Activity Screen - Step 1: PhotosLog Activity Screen - Step 1: Photos

├─├─ [T [Take Photo] button (simulated witake Photo] button (simulated with file picker)h file picker)

├─├─ [Choose from Gallery] button (file picker) [Choose from Gallery] button (file picker)

├─├─ Show selected thumbnails (max 10) Show selected thumbnails (max 10)

├─├─ T Tap thumbnail ap thumbnail →→ add caption modal add caption modal

└─└─ [Next] or [Skip] [Next] or [Skip]

↓↓

Log Activity Screen - Step 2: NotesLog Activity Screen - Step 2: Notes

├─├─ "How did it go?" "How did it go?"

├─├─ T Textarea (placeholder prompts)extarea (placeholder prompts)

├─├─ Character count (0/500) Character count (0/500)

└─└─ [Next] or [Skip] [Next] or [Skip]

↓↓

Log Activity Screen - Step 3: 4E FeedbackLog Activity Screen - Step 3: 4E Feedback

`  `├─ ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.010.png) Enjoy: ![ref5] Yes / ![ref5] Neutral / ![ref5] No

`  `├─ ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.011.png) Easy: ![ref5] Too Easy / ![ref5] Just Right / ![ref5] Challenging   ├─ ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.012.png) Excellent: ![ref5] Yes / ![ref5] Okay / ![ref5] Struggled

`  `└─ ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.013.png) Earn: ![ref5] Yes / ![ref5] No

↓↓

`  `[Save Activity] button  [Save Activity] button

↓↓

Success AnimationSuccess Animation

├─├─ Confetti ef Confetti effect (CSS animation)fect (CSS animation)

├─├─ "+10 XP" badge animation "+10 XP" badge animation

├─├─ Check if badge unlocked  Check if badge unlocked →→ Show badge modal Show badge modal

└─└─ [V [View Tiew Timeline] or [Back Home]imeline] or [Back Home]

↓↓

TTimeline Updatedimeline Updated

└─└─ New entry card appear New entry card appears at tops at top

**Flow D: View Insights**

Home DashboardHome Dashboard![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.014.png)

↓↓

TTap on child stats card or [Vap on child stats card or [View Insights] buttoniew Insights] button

↓↓

Child Dashboard (Insights Page)Child Dashboard (Insights Page)

├─├─ Header: Child photo + name + age Header: Child photo + name + age

├─├─ Activity Breakdown Chart (pie chart - static image for prototype) Activity Breakdown Chart (pie chart - static image for prototype)   ├─ Favorite Activities section (cards with "![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.015.png) Loved" count)

├─├─ T Talent Indicators sectionalent Indicators section

││ └─└─ Insight cards: Insight cards:

`  `│       "![ref6] Rina shows creative talent!"

││       "Based on 8 activities where she excelled"       "Based on 8 activities where she excelled"

││       [T       [Tap to see details modal]ap to see details modal]

├─├─ Areas to Explore Areas to Explore

││ └─└─ "Haven't tried Science yet!" "Haven't tried Science yet!"

││ └─└─ Carousel of 3 Science activity cards Carousel of 3 Science activity cards

└─└─ [V [View Full Tiew Full Timeline] buttonimeline] button

↓↓

TTimeline Vimeline Viewiew

├─├─ V Vertical scrollertical scroll

├─├─ Month/year headers Month/year headers

├─├─ Activity log cards (date, photo, tit Activity log cards (date, photo, title, category)le, category)

└─└─ T Tap card ap card →→ Log detail modal Log detail modal

**Flow E: Admin - Create Activity (Simplified)**

Admin Login Page (separate URL: /admin)Admin Login Page (separate URL: /admin)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.017.png)

├─├─ Email + Password Email + Password

└─└─ [Login] (any input accepted in prototype) [Login] (any input accepted in prototype)

↓↓

Admin DashboardAdmin Dashboard

├─├─ Quick stats cards Quick stats cards

├─├─ Recent activity feed Recent activity feed

└─└─ [Create New Activity] CT [Create New Activity] CTAA

↓↓

TTemplate Selector Modalemplate Selector Modal

`  `├─ ![ref6] Art & Craft

`  `├─ ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.018.png) Science

`  `├─  ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.019.png) Physical

`  `├─ ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.020.png) Cooking

└─└─ ... (8 options) ... (8 options)

↓↓

Create Activity Form (WCreate Activity Form (Wizard)izard)

├─├─ Step 1: Basic Info (title, age, categories, dif Step 1: Basic Info (title, age, categories, difficultyficulty, duration), duration) ├─├─ Step 2: Materials (list bui Step 2: Materials (list builder)lder)

├─├─ Step 3: Instructions (steps with im Step 3: Instructions (steps with image upload mockup)age upload mockup)

├─├─ Step 4: Educational V Step 4: Educational Value (checklists, parent tips textarea)alue (checklists, parent tips textarea) └─└─ Step 5: Media & Preview Step 5: Media & Preview

├─├─ Upload main image (file picker) Upload main image (file picker)

├─├─ [Preview Activity] button  [Preview Activity] button →→ Opens mobile view modal Opens mobile view modal └─└─ [Save as Draft] / [Submit for Review] / [Publish] [Save as Draft] / [Submit for Review] / [Publish]

↓↓

Success MessageSuccess Message

`  `└─ "Activity created! ![ref7]"

↓↓

Return to Admin Dashboard (new activity in list)Return to Admin Dashboard (new activity in list)![ref4]

**3. Dummy Data Strategy**

1. **Realistic Data Principles**

**Why Realistic Data Matters**:

- Testers can understand context (lorem ipsum is distracting)
- Reveals content strategy issues (e.g., text too long breaks layout)
- Allows meaningful feedback ("This activity sounds fun!" vs "Lorem ipsum dolor sit")
- Demonstrates app's value proposition convincingly

**Data Realism Guidelines**:

- ![ref1] Use actual Indonesian names, places, contexts
- ![ref1] Age-appropriate activity titles and descriptions
- ![ref1] Realistic photos (use free stock photos: Unsplash, Pexels)
- ![ref1] Plausible timestamps (recent dates, not 1970)
- ![ref1] Varied data (different categories, difficulties, durations)
- ![ref3] No real personal data (use obviously fake emails like [test@jejakanak.app)](mailto:test@jejakanak.app)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.022.png)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.023.png)
- ![ref3] No child faces in photos (privacy, use illustrations or partial shots)
2. **Activity Library Data (50 Activities Minimum)**

**Category Distribution**:

- Art & Creativity: 8 activities
- Science & Discovery: 6 activities
- Physical & Outdoor: 8 activities
- Literacy & Language: 6 activities
- Music & Rhythm: 4 activities
- Cooking & Nutrition: 6 activities
- Social & Emotional: 6 activities
- Cognitive & Logic: 6 activities

**Age Distribution**:

- Prenatal (0 months): 3 activities
- 0-12 months: 5 activities
- 1-3 years: 10 activities
- 3-5 years: 12 activities
- 6-8 years: 10 activities
- 9-11 years: 6 activities
- 12-15 years: 4 activities

**Sample Activities** (Examples for prototype):

json![ref8]

{{

"id""id":: "act-001""act-001",,

"title""title":: "Membuat Kolase dari Daun Kering""Membuat Kolase dari Daun Kering",,

"slug""slug":: "kolase-daun-kering""kolase-daun-kering",,

"description""description":: "Ajak si kecil mengumpulkan daun kering dan membuat karya seni kolase yang indah. Aktivit"Ajak si kecil mengumpulkan daun kering dan membuat karya seni kolase yang indah. Aktivitas ini melatih kreativitas ini melatih kreativit "ageMinMonths""ageMinMonths":: 3636,,

"ageMaxMonths""ageMaxMonths":: 8484,,

"categories""categories":: [["Art & Creativity""Art & Creativity",, "Outdoor""Outdoor"]],,

"dif"difficulty"ficulty":: "easy""easy",,

"durationMinutes""durationMinutes":: 3030,,

"locationT"locationType"ype":: "both""both",,

"materials""materials":: [[

{{"name""name":: "Daun kering""Daun kering",, "quantity""quantity":: "10-15 lembar""10-15 lembar",, "isCommon""isCommon":: truetrue}},,

{{"name""name":: "Lem putih""Lem putih",, "quantity""quantity":: "1 botol""1 botol",, "isCommon""isCommon":: truetrue}},,

{{"name""name":: "Kertas karton""Kertas karton",, "quantity""quantity":: "1 lembar""1 lembar",, "isCommon""isCommon":: truetrue}},,

{{"name""name":: "Spidol warna""Spidol warna",, "quantity""quantity":: "Set""Set",, "isCommon""isCommon":: truetrue}}

]],,

"steps""steps":: [[

{{

"order""order":: 11,,

"instruction""instruction":: "Ajak anak berjalan-jalan di taman atau halaman untuk mengumpulkan daun kering. Bi"Ajak anak berjalan-jalan di taman atau halaman untuk mengumpulkan daun kering. Biarkan mereka memilih daun dengan bentuk daarkan mereka memilih daun dengan bentuk da "imageUrl""imageUrl":: "/images/activit"/images/activities/leaf-collage-step1.jpg"ies/leaf-collage-step1.jpg"

}},,

{{

"order""order":: 22,,

"instruction""instruction":: "Di rumah, tunjukkan cara mengoleskan lem di balik daun dengan jari atau kuas kecil.""Di rumah, tunjukkan cara mengoleskan lem di balik daun dengan jari atau kuas kecil.",,

"imageUrl""imageUrl":: "/images/activit"/images/activities/leaf-collage-step2.jpg"ies/leaf-collage-step2.jpg"

}},, {{

"order""order":: 33,,

"instruction""instruction":: "Bantu anak menempelkan daun di kertas karton untuk membentuk gambar (misal:"Bantu anak menempelkan daun di kertas karton untuk membentuk gambar (misal: pohon, bunga, kupu-kupu, atau desain abstrak)." pohon, bunga, kupu-kupu, atau desain abstrak)." "imageUrl""imageUrl":: nullnull

}},,

{{

"order""order":: 44,,

"instruction""instruction":: "Setelah selesai, tambahkan detail dengan spidol warna. Biarkan karya mengering lalu pajang di dinding!""Setelah selesai, tambahkan detail dengan spidol warna. Biarkan karya mengering lalu pajang di dinding!",,

"imageUrl""imageUrl":: nullnull

}}

]],,

"educationalV"educationalValues"alues":: [["Creativity""Creativity",, "Fine Motor Skills""Fine Motor Skills",, "Nature Appreciation""Nature Appreciation",, "Art Expression""Art Expression"]],,

"parentT"parentTips"ips":: "Biarkan anak bereksplorasi dengan bentuk dan warna"Biarkan anak bereksplorasi dengan bentuk dan warna tanpa terlalu banyak instruksi. T tanpa terlalu banyak instruksi. Tidak perlu 'sempurna' - proses lebih penting dari idak perlu 'sempurna' - proses lebih penting dari "conversationStarters""conversationStarters":: [[

"Daun mana yang paling kamu suka? Kenapa?""Daun mana yang paling kamu suka? Kenapa?",,

"Kalau daun ini bisa bicara, kira-kira dia cerita apa?""Kalau daun ini bisa bicara, kira-kira dia cerita apa?",,

"Apa yang kamu rasakan saat pegang daun ke"Apa yang kamu rasakan saat pegang daun kering?"ring?"

"Apa yang kamu rasakan saat pegang daun ke"Apa yang kamu rasakan saat pegang daun kering?"ring?"![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.025.png)

]],,

"safetyNotes""safetyNotes":: "Pastikan daun yang dikumpulkan bersih dan tidak beracun. Hindari daun dengan duri atau getah. A"Pastikan daun yang dikumpulkan bersih dan tidak beracun. Hindari daun dengan duri atau getah. Awasi penggunaan lem."wasi penggunaan lem." "mainImageUrl""mainImageUrl":: "/images/activit"/images/activities/leaf-collage-main.jpg"ies/leaf-collage-main.jpg",,

"additionalImages""additionalImages":: [[

"/images/activit"/images/activities/leaf-collage-2.jpg"ies/leaf-collage-2.jpg",,

"/images/activit"/images/activities/leaf-collage-3.jpg"ies/leaf-collage-3.jpg"

]],,

"videoUrl""videoUrl":: nullnull,,

"popularityScore""popularityScore":: 8585,,

"viewCount""viewCount":: 342342,,

"completionCount""completionCount":: 127127,,

"averageRating""averageRating":: 4.74.7,,

"publishedAt""publishedAt":: "2025-09-15T08:00:00Z""2025-09-15T08:00:00Z"

}}

**More Examples** (Titles Only for Speed):

1. "Eksperimen Gunung Berapi Mini" (Science, 5-10 years)
1. "Yoga untuk Bumil: Trimester 2" (Prenatal)
1. "Sensory Play: Kotak Harta Karun" (0-2 years)
1. "Membuat Smoothie Buah Bersama" (Cooking, 3-7 years)
1. "Berburu Bentuk di Sekitar Rumah" (Outdoor, 2-5 years)
1. "Cerita Bergambar Buatan Sendiri" (Literacy, 6-10 years)
1. "Lagu & Gerakan: 'Kepala Pundak Lutut Kaki'" (Music, 1-4 years)
1. "Puzzle DIY dari Gambar Keluarga" (Cognitive, 4-8 years)
1. "Berkebun Mini: Menanam Kacang Hijau" (Science/Outdoor, 5-10 years)
1. "Napas dalam untuk Bumil" (Prenatal) ... (40 more activities covering all categories and ages)
3. **User & Child Profile Data (5 Sample Parents)**

**Parent 1: Siti Rahmawati**

- Email: <siti.test@jejakanak.app>![ref9]![ref10]
- Level: 3 (Active Parent)
- XP: 550
- Current Streak: 5 days
- Badges: Early Bird, Memory Keeper, Art Explorer
- Children:
  - **Rina** (4 years old, born 2020-03-15)
    - 18 activities logged
    - Favorite categories: Art (8), Music (4), Outdoor (3)
    - Insights: "Shows creative talent", "Loves hands-on activities"

**Parent 2: Budi Santoso**

- Email: <budi.test@jejakanak.app>![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.028.png)![ref11]
- Level: 4 (Super Parent)
- XP: 1,245
- Current Streak: 12 days
- Badges: Early Bird, Memory Keeper, Well-Rounded, Week Warrior, Super Parent
- Children:
  - **Arya** (7 years old, born 2018-01-22)
    - 35 activities logged
    - Favorite categories: Science (12), Outdoor (10), Cognitive (8)
    - Insights: "Curious about how things work", "Ready for advanced challenges"
  - **Sari** (4 years old, born 2021-06-10)
    - 15 activities logged
    - Favorite categories: Cooking (6), Art (5), Social (4)
    - Insights: "Enjoys social interaction", "Budding chef!"

**Parent 3: Dewi Lestari (Bumil)**

- Email: <dewi.test@jejakanak.app>![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.030.png)![ref11]
- Level: 1 (Newbie Parent)
- XP: 45
- Current Streak: 0 days
- Badges: Early Bird
- Children:
  - **Baby Lestari** (Expecting, EDD: 2026-02-14)
    - 3 prenatal activities logged
    - Notes: "Feeling prepared and excited!"

**Parent 4: Rudi Hartono**

- Email: <rudi.test@jejakanak.app>![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.031.png)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.032.png)
- Level: 2 (Engaged Parent)
- XP: 280
- Current Streak: 3 days
- Badges: Early Bird, Memory Keeper
- Children:
  - **Kevin** (10 years old, born 2015-08-05)
    - 12 activities logged
    - Favorite categories: Physical (5), Science (4), Outdoor (3)
    - Insights: "Loves active play", "Try team sports?"

**Parent 5: Ani Wijaya**

- Email: <ani.test@jejakanak.app>![ref9]![ref10]
- Level: 3 (Active Parent)
- XP: 620
- Current Streak: 0 days (streak broken yesterday)
- Badges: Early Bird, Memory Keeper, Art Explorer, Storyteller (10 detailed notes)
- Children:
  - **Luna** (5 years old, born 2020-11-30)
    - 22 activities logged
    - Favorite categories: Literacy (9), Art (7), Music (4)
    - Insights: "Loves stories and books", "Strong language development"
4. **Activity Logs (Sample Data for Timelines)**

**For Rina (Siti's daughter) - Recent 5 Logs**:

json![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.033.png)

[[

{{

"id""id":: "log-001""log-001",,

"activityT"activityTitle"itle":: "Membuat Kolase dari Daun Kering""Membuat Kolase dari Daun Kering",,

"completedAt""completedAt":: "2025-10-18T15:30:00Z""2025-10-18T15:30:00Z",,

"photos""photos":: [[

"/images/logs/rina-collage1.jpg""/images/logs/rina-collage1.jpg",,

"/images/logs/rina-collage2.jpg""/images/logs/rina-collage2.jpg"

]],,

"notes": "Rina sangat excited mengumpulkan daun! Dia bikin gambar kupu-kupu dari daun oak. Warnanya cantik banget - emas dan coklat. Dia bilan "feedback4E""feedback4E":: {{

"enjoy""enjoy":: truetrue,,

"easy""easy":: truetrue,,

"excellent""excellent":: truetrue,,

"earn""earn":: truetrue

}},,

"isFavorite""isFavorite":: truetrue

}},, {{

"id""id":: "log-002""log-002",,

"activityT"activityTitle"itle":: "Lagu & Gerakan: 'Kepala Pundak Lutut Kaki'""Lagu & Gerakan: 'Kepala Pundak Lutut Kaki'",,

"completedAt""completedAt":: "2025-10-16T10:00:00Z""2025-10-16T10:00:00Z",,

"photos""photos":: [["/images/logs/rina-song.jpg""/images/logs/rina-song.jpg"]],,

"notes": "Rina udah hafal lagunya! Sekarang dia yang lead, Ibu yang ikut ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.034.png) Gerakan kakinya udah koordinasi banget.", "feedback4E""feedback4E":: {{

"enjoy""enjoy":: truetrue,,

"easy""easy":: falsefalse,,

"excellent""excellent":: truetrue,,

"earn""earn":: falsefalse

}},,

"isFavorite""isFavorite":: falsefalse

}},, {{

"id""id":: "log-003""log-003",,

"activityT"activityTitle"itle":: "Berburu Bentuk di Sekitar Rumah""Berburu Bentuk di Sekitar Rumah",,

"completedAt""completedAt":: "2025-10-14T16:45:00Z""2025-10-14T16:45:00Z",,

"photos""photos":: [[]],,

"notes""notes":: "Rina nemuin banyak bentuk lingkaran (jam dinding, pi"Rina nemuin banyak bentuk lingkaran (jam dinding, piring) dan persegi (jendela, bantal). Aktivitas ini simple tring) dan persegi (jendela, bantal). Aktivitas ini simple tapi efektif!"api efektif!" "feedback4E""feedback4E":: {{

"enjoy""enjoy":: falsefalse,,

"easy""easy":: truetrue,,

"excellent""excellent":: falsefalse,,

"earn""earn":: falsefalse

}},,

"isFavorite""isFavorite":: falsefalse

"isFavorite""isFavorite":: falsefalse![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.035.png)

}},, {{

"id""id":: "log-004""log-004",,

"activityT"activityTitle"itle":: "Sensory Play: Kotak Harta Karun""Sensory Play: Kotak Harta Karun",,

"completedAt""completedAt":: "2025-10-12T14:20:00Z""2025-10-12T14:20:00Z",,

"photos""photos":: [["/images/logs/rina-sensory"/images/logs/rina-sensory.jpg".jpg"]],,

"notes""notes":: "Bikin sensory bin pakai beras dan mainan kecil. Rina main 45 m"Bikin sensory bin pakai beras dan mainan kecil. Rina main 45 menit nonstop! Focused banget."enit nonstop! Focused banget.",, "feedback4E""feedback4E":: {{

"enjoy""enjoy":: truetrue,,

"easy""easy":: truetrue,,

"excellent""excellent":: falsefalse,,

"earn""earn":: falsefalse

}},,

"isFavorite""isFavorite":: falsefalse

}},, {{

"id""id":: "log-005""log-005",,

"activityT"activityTitle"itle":: "Membuat Smoothie Buah Bersama""Membuat Smoothie Buah Bersama",,

"completedAt""completedAt":: "2025-10-10T09:00:00Z""2025-10-10T09:00:00Z",,

"photos""photos":: [["/images/logs/rina-smoothi"/images/logs/rina-smoothie1.jpg"e1.jpg",, "/images/logs/rina-smoothi"/images/logs/rina-smoothie2.jpg"e2.jpg"]],,

"notes": "Rina suka banget masukin buah ke blender! Smoothie pisang-strawberry jadi favorit. Bonus: dia mau minum buah "feedback4E""feedback4E":: {{

"enjoy""enjoy":: truetrue,,

"easy""easy":: truetrue,,

"excellent""excellent":: falsefalse,,

"earn""earn":: truetrue

}},,

"isFavorite""isFavorite":: truetrue

}}

]]

(Similar log data for other children - total ~80 logs across 5 parents)

5. **Gamification Data**

**Badges (Pre-defined in System)**:

javascript![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.036.png)

constconst BADGESBADGES == [[

{{

typetype:: "early\_bird""early\_bird",,

namename:: "Early Bird""Early Bird",,

descriptiondescription:: "Logged your first 5 activities""Logged your first 5 activities",,

icon: "![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.037.png)",

unlockedByunlockedBy:: [["siti""siti",, "budi""budi",, "dewi""dewi",, "rudi""rudi",, "ani""ani"]] *// all have this// all have this* }},,

{{

typetype:: "memory\_keeper""memory\_keeper",,

namename:: "Memory Keeper""Memory Keeper",, descriptiondescription:: "Uploaded 20 photos""Uploaded 20 photos",, icon: "![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.038.png)",

unlockedByunlockedBy:: [["siti""siti",, "budi""budi",, "ani""ani"]]

}},, {{

typetype:: "art\_explorer""art\_explorer",,

namename:: "Art Explorer""Art Explorer",,

descriptiondescription:: "Completed 10 Art activiti"Completed 10 Art activities"es",, icon: "![ref6]",

unlockedByunlockedBy:: [["siti""siti",, "ani""ani"]]

}},, {{

typetype:: "week\_warrior""week\_warrior",,

namename:: "W"Week Week Warrior"arrior",, descriptiondescription:: "7-day activity streak""7-day activity streak",, icon: " ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.039.png) ",

unlockedByunlockedBy:: [["budi""budi"]]

}},, {{

typetype:: "super\_parent""super\_parent",,

namename:: "Super Parent""Super Parent",,

descriptiondescription:: "Logged 50 activities""Logged 50 activities",, icon: " ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.040.png) ",

unlockedByunlockedBy:: [["budi""budi"]]

}},, {{

typetype:: "well\_rounded""well\_rounded",,

namename:: "W"Well-Rounded"ell-Rounded",, descriptiondescription:: "T"Tried all 8 categories"ried all 8 categories",, icon: "![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.041.png)",

unlockedByunlockedBy:: [["budi""budi"]]

}},, {{

typetype:: "storyteller""storyteller"

typetype:: "storyteller""storyteller",,![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.042.png)

namename:: "Storyteller""Storyteller",,

descriptiondescription:: "W"Wrote 10 detailed notes (50+ characters)"rote 10 detailed notes (50+ characters)",, icon: "![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.043.png)",

unlockedByunlockedBy:: [["ani""ani"]]

}},,

*// ... (15 mor// ... (15 more badges, most locked for all users)e badges, most locked for all users)*

]];;

**Current Challenge** (Active):

json![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.044.png)

{{

"id""id":: "challenge-oct-2025""challenge-oct-2025",,

"title""title":: "October Outdoor Adventure""October Outdoor Adventure",,

"description""description":: "Complete 5 outdoor activit"Complete 5 outdoor activities this month and earn the Outdoor Explorer badge!"ies this month and earn the Outdoor Explorer badge!",, "startDate""startDate":: "2025-10-01""2025-10-01",,

"endDate""endDate":: "2025-10-31""2025-10-31",,

"goalCount""goalCount":: 55,,

"category""category":: "Outdoor""Outdoor",,

"participants""participants":: [[

{{"userId""userId":: "siti""siti",, "progress""progress":: 33,, "completed""completed":: falsefalse}},,

{{"userId""userId":: "budi""budi",, "progress""progress":: 55,, "completed""completed":: truetrue}},, *// completed!// completed!*

{{"userId""userId":: "rudi""rudi",, "progress""progress":: 22,, "completed""completed":: falsefalse}}

]]

}}

6. **Community Data (If Included)**

**Play Spots** (3 examples):

json![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.045.png)

[[

{{

"id""id":: "spot-001""spot-001",,

"name""name":: "T"Taman Spathodea, BSD"aman Spathodea, BSD",,

"type""type":: "playground""playground",,

"address""address":: "Jl. Pahlawan Seribu, BSD City"Jl. Pahlawan Seribu, BSD City, T, Tangerang Selatan"angerang Selatan",,

"latitude""latitude":: -6.3018-6.3018,,

"longitude""longitude":: 106.6519106.6519,,

"ageSuitabilityMi"ageSuitabilityMin"n":: 11,,

"ageSuitabilityMax""ageSuitabilityMax":: 1212,,

"facilities""facilities":: [["parking""parking",, "restroom""restroom",, "food\_stall""food\_stall",, "shade""shade"]],,

"photos""photos":: [["/images/playspots/spathodea.jpg""/images/playspots/spathodea.jpg"]],,

"notes""notes":: "Great for toddlers! Ada ayuna"Great for toddlers! Ada ayunan, perosotan, dan area pasirn, perosotan, dan area pasir. Pagi hari best time (sepi & sejuk).". Pagi hari best time (sepi & sejuk).",, "upvotes""upvotes":: 1515,,

"activityCount""activityCount":: 88

}},, {{

"id""id":: "spot-002""spot-002",,

"name""name":: "Kidzania Jakarta""Kidzania Jakarta",,

"type""type":: "indoor\_play""indoor\_play",,

"address""address":: "Pacific Place Mall, Jakarta""Pacific Place Mall, Jakarta",,

"latitude""latitude":: -6.2252-6.2252,,

"longitude""longitude":: 106.8093106.8093,,

"ageSuitabilityMi"ageSuitabilityMin"n":: 44,,

"ageSuitabilityMax""ageSuitabilityMax":: 1414,,

"facilities""facilities":: [["parking""parking",, "restroom""restroom",, "food\_court""food\_court",, "AC""AC"]],,

"notes""notes":: "Role-play activities untuk anak. Lum"Role-play activities untuk anak. Lumayan pricey tapi worth it. Book online untuk avoid queue."ayan pricey tapi worth it. Book online untuk avoid queue.",, "upvotes""upvotes":: 2323,,

"activityCount""activityCount":: 1212

}},, {{

"id""id":: "spot-003""spot-003",,

"name""name":: "Perpustakaan Cikini""Perpustakaan Cikini",,

"type""type":: "library""library",,

"address""address":: "Jl. Cikini Raya, Jakarta Pusat""Jl. Cikini Raya, Jakarta Pusat",,

"ageSuitabilityMi"ageSuitabilityMin"n":: 33,,

"ageSuitabilityMax""ageSuitabilityMax":: 1515,,

"facilities""facilities":: [["parking""parking",, "restroom""restroom",, "wheelchair\_accessible""wheelchair\_accessible"]],,

"notes""notes":: "Koleksi buku anak bagus. Ada story telling session setiap Sabtu pagi jam 10. Free!""Koleksi buku anak bagus. Ada story telling session setiap Sabtu pagi jam 10. Free!",, "upvotes""upvotes":: 99,,

"activityCount""activityCount":: 44

}}

]]

**Activity Variations** (2 examples):

json![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.046.png)

[[

{{

"parentActivityT"parentActivityTitle"itle":: "Membuat Kolase dari Daun Kering""Membuat Kolase dari Daun Kering",,

"submittedBy""submittedBy":: "ani""ani",,

"variationT"variationTitle"itle":: "Luna's Underwater Scene Collage""Luna's Underwater Scene Collage",,

"variationNotes""variationNotes":: "Kami pakai daun kering untuk bikin pemandangan bawah laut! Daun oak jadi ubur"Kami pakai daun kering untuk bikin pemandangan bawah laut! Daun oak jadi ubur-ubur-ubur, daun maple jadi ikan. Luna add glitt, daun maple jadi ikan. Luna add glitt "photoUrl""photoUrl":: "/images/variations/l"/images/variations/luna-underwateruna-underwater.jpg".jpg",,

"helpfulCount""helpfulCount":: 55

}},, {{

"parentActivityT"parentActivityTitle"itle":: "Membuat Smoothie Buah Bersama""Membuat Smoothie Buah Bersama",,

"submittedBy""submittedBy":: "siti""siti",,

"variationT"variationTitle"itle":: "Green Monster Smoothie (Rina's Fave)""Green Monster Smoothie (Rina's Fave)",,

"variationNotes": "Tambah bayam + yogurt + madu. Rina surprisingly suka! Dia sebut 'jus monster hijau' ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.047.png) Healthy & yummy "photoUrl""photoUrl":: "/images/variations/green-smoothie.j"/images/variations/green-smoothie.jpg"pg",,

"helpfulCount""helpfulCount":: 1212

}}

]]![ref12]

4. **Technology Stack untuk Prototype**
1. **Evaluation Criteria**

Prototype tech stack harus:

- ![ref1] **Fast to develop** (2-3 weeks deadline)
- ![ref1] **Easy to iterate** (quick changes based on feedback)
- ![ref1] **Realistic feel** (interactive, not just static mockup)
- ![ref1] **Accessible** (anyone can open and test, no complex setup)
- ![ref1] **Disposable** (tidak perlu production-quality code, akan di-rewrite di Flutter)
2. **Recommended Stack**

**Option A: React + TailwindCSS** (Recommended) **Pros**:

- Component-based (easy to reuse elements)
- TailwindCSS untuk rapid styling (utility classes)
- React hooks untuk simple state management
- Banyak UI libraries gratis (Headless UI, Radix UI)
- Hot reload (instant preview)
- Team familiar (you know Vue, React similar)

**Cons**:

- Slight learning curve jika belum pernah React (but similar to Vue)
- Need Node.js setup

**Tech Details**:

- **Framework**: React 18 (via Vite for fast dev server)
- **Styling**: TailwindCSS + Headless UI (for modals, dropdowns)
- **Routing**: React Router (for multi-page navigation)
- **State**: React Context atau useState (simple, no Redux needed)
- **Icons**: Lucide React atau Heroicons
- **Charts**: Recharts (for dashboard pie chart)
- **Animations**: Framer Motion (for page transitions, confetti)
- **Date Picker**: React DatePicker

**Setup Time**: ~1 hour (create-react-app atau Vite)![ref13]

**Option B: Vue 3 + TailwindCSS** (Alternative if Prefer Vue) **Pros**:

- You're already familiar with Vue!
- Component-based
- TailwindCSS sama aja
- Composition API powerful

**Cons**:

- Slightly less library options vs React

**Tech Details**: Similar to React but with Vue ecosystem![ref2]

**Option C: Plain HTML + Bootstrap + Vanilla JS** (Fastest but Less Elegant) **Pros**:

- Zero setup (just open index.html in browser)
- No build process
- Anyone can edit (even non-developers)

**Cons**:

- Code becomes messy quickly (hard to maintain)
- Less interactive feel (more work for dynamic behavior)
- No component reusability

**When to Use**: Only if extreme time constraint (1 week instead of 2-3)![ref2]

**RECOMMENDATION**: **React + TailwindCSS** (Option A)

**Why**: Sweet spot antara speed dan quality. Component reusability saves time. Tailwind makes styling fast. React's ecosystem rich (easy find copy-paste components).

3. **Project Structure (React)**

jejakanak-prototype/jejakanak-prototype/![ref8]

├──├── public/ public/

││ ├──├── index.html index.html

││ ├──├── images/ images/

││ ││ ├──├── activiti activities/      # Activity photoses/      # Activity photos

││ ││ ├──├── logs/            # User log photos logs/            # User log photos

││ ││ ├──├── playspots/       # Play spot phot playspots/       # Play spot photosos

││ ││ ├──├── avatars/         # Child avatars avatars/         # Child avatars

││ ││ └──└── badges/          # Badge icons badges/          # Badge icons

││ └──└── data/ data/

││ ├──├── activiti activities.json  # All 50 activitieses.json  # All 50 activities

││ ├──├── users.json       # 5 sample parents users.json       # 5 sample parents

││ ├──├── children.json    # Child profil children.json    # Child profileses

││ ├──├── logs.json        # Activity l logs.json        # Activity logsogs

││ ├──├── badges.json      # Badge definitions badges.json      # Badge definitions

││ ├──├── challenges.json  # Active challenges challenges.json  # Active challenges

││ └──└── playspots.json   # Play spot data playspots.json   # Play spot data

├──├── src/ src/

││ ├──├── components/ components/

││ ││ ├──├── ActivityCard.jsx ActivityCard.jsx

││ ││ ├──├── ActivityDetail.j ActivityDetail.jsxsx

││ ││ ├──├── ChildCard.jsx ChildCard.jsx

││ ││ ├──├── LogCard.jsx LogCard.jsx

││ ││ ├──├── BadgeIcon.jsx BadgeIcon.jsx

││ ││ ├──├── Modal.jsx Modal.jsx

││ ││ ├──├── Navbar Navbar.jsx.jsx

││ ││ ├──├── BottomNav BottomNav.jsx.jsx

││ ││ └──└── ... (20-30 components) ... (20-30 components)

││ ├──├── pages/ pages/

││ ││ ├──├── Splash.jsx Splash.jsx

││ ││ ├──├── W Welcome.jsxelcome.jsx

││ ││ ├──├── SignUp.jsx SignUp.jsx

││ ││ ├──├── OnboardingAddChild.jsx OnboardingAddChild.jsx

││ ││ ├──├── Home.jsx Home.jsx

││ ││ ├──├── ActivityLi ActivityLibrarybrary.jsx.jsx

││ ││ ├──├── ActivityDetailP ActivityDetailPage.jsxage.jsx

││ ││ ├──├── LogActivity LogActivity.jsx.jsx

││ ││ ├──├── ChildT ChildTimeline.jsximeline.jsx

││ ││ ├──├── ChildDashboard.jsx ChildDashboard.jsx

││ ││ ├──├── Settings.jsx Settings.jsx

││ ││ └──└── ... (15-20 pages) ... (15-20 pages)

││ ├──├── context/ context/

││ ││ └──└── AppContext.jsx  # Global stat AppContext.jsx  # Global state (current usere (current user, child), child) ││ ├──├── hooks/ hooks/

││ ││ └──└── useLocalStorage.jsx  # Persist logged in user useLocalStorage.jsx  # Persist logged in user

││ ├──├── utils/ utils/

││ ├──├── utils/ utils/![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.050.png)

││ ││ ├──├── calculateAge.js calculateAge.js

││ ││ ├──├── filterActiviti filterActivities.jses.js

││ ││ └──└── formatDate.js formatDate.js

││ ├──├── App.jsx              # Root component with R App.jsx              # Root component with Routerouter ││ ├──├── index.css            # T index.css            # Tailwind importsailwind imports

││ └──└── main.jsx             # Entry point main.jsx             # Entry point

├──├── package.json package.json

├──├── tailwind.config.js tailwind.config.js

├──├── vite.config.js vite.config.js

└──└── README.md README.md

4. **Data Management Strategy**

**Static JSON Files**: All dummy data stored in  /public/data/ as JSON **Why JSON Files**:

- No database needed (zero setup)
- Easy to edit (just open file, change data)
- Fast to load (fetch() from public folder)
- Version controllable (git tracks changes)

**Data Flow**:

javascript![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.051.png)

*// In component// In component*

useEfuseEffectfect(((()) =>=> {{ fetchfetch(('/data/activit'/data/activities.json'ies.json')) ..thenthen((resres =>=> res res..jsonjson(()))) ..thenthen((datadata =>=> setActivitiessetActivities((datadata))));; }},, [[]]));;

**State Management**:

- **Global State** (Context API): Current logged-in user, selected child
- **Local State** (useState): Page-specific data (form inputs, filters)
- **Persistence** (localStorage): Remember logged-in user across sessions (simulate auth)

**Example Context**:

javascript![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.052.png)

constconst AppContextAppContext == createContextcreateContext(());;

exportexport functionfunction AppProviderAppProvider(({{ children  children }})) {{

constconst [[currentUsercurrentUser,, setCurrentUser setCurrentUser]] == useStateuseState(((()) =>=> {{

*// Load fr// Load from localStorage if existsom localStorage if exists*

constconst saved  saved == localStoragelocalStorage..getItemgetItem(('currentUser''currentUser'));; returnreturn saved  saved ?? JSONJSON..parseparse((savedsaved)) :: nullnull;;

}}));;

constconst [[selectedChildselectedChild,, setSelectedChild setSelectedChild]] == useStateuseState((nullnull));;

constconst loginlogin == ((emailemail)) =>=> {{

*// Simulate logi// Simulate login - find user in datan - find user in data*

fetchfetch(('/data/users.json''/data/users.json'))

..thenthen((resres =>=> res res..jsonjson(())))

..thenthen((usersusers =>=> {{

constconst user  user == users users..findfind((uu =>=> u u..emailemail ====== email email));; setCurrentUsersetCurrentUser((useruser));;

localStoragelocalStorage..setItemsetItem(('currentUser''currentUser',, JSONJSON..stringifystringify((useruser))));; }}));;

}};;

returnreturn ((

<<AppContextAppContext..ProviderProvider value value=={{{{       currentUser      currentUser,,

`      `selectedChild      selectedChild,,

`      `setSelectedChild      setSelectedChild,,

`      `login      login

}}}}>>

{{childrenchildren}} <<//AppContextAppContext..ProviderProvider>>

));;

}}

5. **Simulating Interactivity**

**Login/Signup**:

- Any email input → Accepts
- Password field → Ignored (no validation)
- On submit → Find user in users.json by email (or create mock user)
- Store in context + localStorage

**Adding Child**:

- Form inputs → Store in local state
- On submit → Add to  currentUser.children array in memory (not persisted)
- Navigate to home with new child

**Logging Activity**:

- Photo upload → File picker, store File objects in state, display thumbnails
- On save → Create log object, push to  selectedChild.logs array in memory
- Show success animation, update timeline

**Scheduling**:

- Date picker → Store selected date in state
- On confirm → Add to  scheduledActivities array in memory
- Display in "Upcoming" section

**Gamification**:

- XP/Badges → Pre-calculated in dummy data
- On log activity → Show "+10 XP" animation (not actually calculated)
- If new badge unlocked (pre-defined) → Show badge modal

**Recommendations**:

- Algorithm → Simplified (show predefined list for each child)
- "Recommended" activities → Pre-selected in data based on child's past logs

**Charts**:

- Dashboard pie chart → Static image or use Recharts with dummy percentages
- Data doesn't update dynamically (just for show)

**Filters/Search**:

- Activity library filters → Client-side filtering of activities.json
- Real-time search → Filter array by title match

**Admin Panel**:

- Create activity form → All fields functional
- On submit → Show success message, mock add to library (not persisted)
- Template selector → Pre-fill form with template data![ref4]
5. **Development Process (Week-by-Week)**

**Week 1: Foundation & Core Flows**

**Day 1-2: Setup & Data Preparation**

` `Initialize React + Vite project![ref14]

` `Install dependencies (Tailwind, React Router, etc.)![ref15]

` `Configure Tailwind (colors, fonts matching brand)![ref16]

` `Create project structure (folders, base components)![ref17]

` `Prepare all dummy data JSON files (use GPT to generate if needed)![ref18]

` `Gather images:![ref14]

- Download 50+ free stock photos (Unsplash: kids, activities, parenting)
- Create placeholder avatars (Boring Avatars generator)
- Badge icons (emoji or simple SVGs)

**Day 3-4: User Authentication & Onboarding**

` `Build Splash screen (auto-advance after 2s)![ref19]

` `Build Welcome screen (3-slide carousel)![ref20]

` `Build SignUp/Login page![ref21]

` `Implement Context for global state![ref22]

` `Build Add Child flow (Step 1 & 2)![ref23]

` `Build Personalization modal![ref19]

` `Test full onboarding flow (Splash → Welcome → Sign Up → Add Child → Home)![ref20]

**Day 5-7: Home Dashboard & Activity Library**

` `Build Home Dashboard:![ref20]

- Child selector (if multiple)
- Recommended activities section (cards)
- Scheduled activities section
- Quick stats cards
- Recent memories section

` `Build Activity Library page:![ref16]

- Grid of activity cards
- Filter bar (category, age, duration dropdowns)
- Search input (real-time filter)

` `Build ActivityCard component (reusable)  Build Activity Detail page:![ref20]![ref21]

- Image carousel
- Full content display (materials, steps, tips)
- Schedule button (opens modal)
- Mark as Done button

` `Build Schedule modal (date/time pickers, reminder dropdown)![ref16]

` `Test flow: Home → Browse → Activity Detail → Schedule → Back to Home![ref17]![ref4]

**Week 2: Core Value Loop & Insights**

**Day 8-10: Activity Logging**

` `Build Log Activity page (multi-step wizard):![ref14]

- Step 1: Photo upload UI (file picker, thumbnails)
- Step 2: Notes textarea
- Step 3: 4E feedback (visual toggles)
- Navigation: Back/Next buttons, progress indicator

` `Build success animation (confetti + XP badge)![ref19]

` `Build badge unlock modal (if applicable)![ref20]

` `Implement adding log to child's timeline (in-memory)![ref21]

` `Test flow: Activity Detail → Log → Success → Timeline updated![ref22]

**Day 11-12: Timeline & Insights Dashboard**

` `Build Child Timeline page:![ref20]

- Vertical scroll
- Month/year headers
- Log cards (date, photo, title, excerpt)
- Tap card → Expand detail modal

` `Build Child Dashboard (Insights) page:![ref15]

- Header with child info
- Activity breakdown chart (pie chart - Recharts or static image)
- Favorite activities carousel
- Talent indicators section (insight cards)
- Areas to explore section (recommended categories)

` `Implement basic "insights" logic (count categories, detect favorites)![ref21]

` `Test flow: Home → Child Dashboard → View insights → Explore recommended activities![ref22]

**Day 13-14: Polish Core Features**

` `Build Settings page (notification preferences, account info)![ref19]

` `Build Edit Profile pages (parent, child)![ref20]

` `Implement bottom navigation (Home, Library, Add/Log, Timeline, Profile)  Add page transitions (smooth animations)![ref21]![ref22]

` `Add loading states (skeletons, spinners)![ref23]

` `Add empty states ("No activities logged yet" with CTA)![ref19]

` `Bug fixes and responsive tweaks (test on mobile size)![ref20]![ref24]

**Week 3: Secondary Features & Admin Panel**

**Day 15-16: Gamification Elements**

` `Build Badges page (grid of earned + locked badges)![ref22]

` `Build Challenge page (active challenge with progress bar)![ref23]

` `Add XP/level display to Home (user avatar with level badge)  Add streak indicator to dashboard ("![ref19] ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.064.png) 5-day streak!")![ref20]

` `Test badge animations and challenge progress![ref21]

**Day 17-18: Community Features (If Time Permits)**

` `Build Play Spots page:![ref20]

- Map view (embedded Google Maps iframe or static map image with pins)
- List view (spot cards with distance, upvotes)

` `Build Play Spot Detail modal![ref18]

` `Build Activity Variations section (on activity detail page)![ref14]

- Carousel of user variations
- "Helpful" button

` `Test community flows![ref22]

**Day 19-20: Admin Panel**

` `Build Admin Login page (separate URL:  /admin )  Build Admin Dashboard:![ref19]![ref15]

- Stats cards
- Recent activity feed
- Create Activity CTA

` `Build Create Activity page:![ref19]

- Template selector modal
- Multi-step form wizard (5 steps)
- Preview modal (mobile view simulation)

` `Build Activity Library management table (list with edit/delete)![ref18]

` `Test admin flows: Login → Dashboard → Create Activity → Preview → Save![ref14]

**Day 21: Final Polish & Testing**

` `Cross-browser testing (Chrome, Safari, Firefox)![ref16]

` `Mobile responsive testing (iPhone, Android sizes)![ref17]

` `Fix any layout bugs![ref18]

` `Add tooltips/help text where needed![ref14]

` `Proofread all copy (check for typos)![ref15]

` `Create a "demo account" with rich data for testers![ref16]

` `Deploy prototype to Vercel/Netlify (free hosting)![ref17]

- Get shareable URL: [https://jejakanak-prototype.vercel.app](https://jejakanak-prototype.vercel.app/)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.065.png)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.066.png)![ref13]
6. **User Testing Protocol**
1. **Participant Recruitment**

**Target Participants**:

**Group A: Psikolog/Educator Team (2-3 people)**

- Uwa Farah (lead validator)
- 1-2 child development experts
- Focus: Educational value, developmental appropriateness, safety

**Group B: Content Team (2-3 people)**

- Uwa Farah's content creators
- Focus: Admin panel usability, content input workflow

**Group C: Parent Testers (5-7 people)**

- Mix of demographics:
  - 2 first-time parents (young children 0-3)
  - 2 experienced parents (children 4-8)
  - 1 parent with multiple kids
  - 1 expectant mother (pregnant)
  - 1 parent with older child (9-15)
- Mix of tech-savviness (not all early adopters)
- All from target market (urban Indonesia)

**Recruitment**:

- Internal network (friends, colleagues)
- Parenting Facebook groups (post invitation)
- Incentive: Early access to app + "Founding Member" badge when launches
2. **Testing Sessions**

**Format**: Individual 1-hour sessions (remote via Zoom or in-person) **Session Structure**:

**Part 1: Introduction (5 min)**

- Explain purpose: "Testing prototype app, not testing you"
- Emphasize: "Think aloud - say what you're thinking"
- Clarify: "This is dummy, some things won't work perfectly"
- Get consent (record session for note-taking)

**Part 2: Guided Tasks (40 min)**

Facilitate (but don't help), observe, take notes:

**Task 1: Onboarding (10 min)**

- "Imagine you just downloaded JejakAnak. Explore and sign up."
- Observe:
  - Do they understand value proposition from welcome screen?
  - Any confusion in sign up flow?
  - Add child process smooth?
  - Do they understand prenatal option?

**Task 2: Browse Activities (10 min)**

- "You want to find a fun art activity for your 4-year-old. Show me how you'd do that."
- Observe:
  - Can they find library easily?
  - Do they use filters or scroll?
  - Is activity detail page clear?
  - Do they understand materials/steps?

**Task 3: Schedule Activity (5 min)**

- "You found an activity you like. Schedule it for this weekend."
- Observe:
  - Can they find schedule button?
  - Is scheduling process intuitive?
  - Do they set reminder?

**Task 4: Log Activity (10 min)**

- "Pretend you just did this activity with your child. Log it."
- Observe:
  - Photo upload: confusing?
  - Notes: do they write something meaningful?
  - 4E feedback: do they understand each dimension?
  - Any friction?

**Task 5: Explore Insights (5 min)**

- "Check your child's progress and insights."
- Observe:
  - Can they find dashboard?
  - Do they understand insights?
  - Is chart readable?
  - Do recommendations make sense?

**Part 3: Open Exploration (10 min)**

- "Explore the app freely. Click around."
- See what they naturally gravitate to
- Note: What do they click? What do they ignore?

**Part 4: Feedback Discussion (5 min)**

- Structured questions:
  - "What did you like most?"
  - "What was confusing or frustrating?"
  - "Would you use this app? Why or why not?"
  - "What's missing?"
  - "On a scale 1-5, how likely to recommend?"
- Open-ended: "Any other thoughts?"
3. **Psikolog Team Validation (Separate Session)**

**Format**: 2-hour workshop **Focus Areas**:

1. **Educational Alignment (45 min)**
- Review sample activities (10-15 activities)
- Questions:
  - Are age ranges appropriate?
  - Is educational value clearly articulated?
  - Any safety concerns?
  - Are conversation starters effective?
  - Anything developmentally inappropriate?
2. **4E Framework Validation (30 min)**
- Show 4E feedback UI
- Questions:
  - Is this framework sound for talent discovery?
  - Are the 4 dimensions clear to parents?
  - Any concerns about misinterpretation?
  - Suggestions for improvement?
3. **Insights Review (30 min)**
- Show sample insights ("Rina shows creative talent")
- Questions:
  - Are these insights helpful or misleading?
  - Risk of labeling children too early?
  - How to phrase insights sensitively?
  - What insights are most valuable for parents?
4. **Overall App Assessment (15 min)**
- Would you recommend this to parents?
- Any red flags from child development perspective?
- Suggestions for improvement?
4. **Content Team Validation (Admin Panel Focus)**

**Format**: 1.5-hour hands-on session

**Tasks**:

**Task 1: Create Activity (45 min)**

- "Create a new art activity for 3-5 year olds using the admin panel."
- Observe:
  - Template helpful or restrictive?
  - Any confusing fields?
  - Validation errors helpful?
  - Preview function useful?

**Task 2: Bulk Import (15 min)**

- "You have 10 activities in a spreadsheet. How would you add them?"
- Show bulk import feature
- Get feedback on format and process

**Task 3: Review Content (15 min)**

- Show review queue with pending recipes/variations
- "Approve or reject these 3 submissions."
- Observe decision-making process

**Discussion (15 min)**:

- Is this workflow efficient for your needs?
- What would make content creation easier?
- Any features missing?
5. **Data Collection & Analysis**

**During Sessions**:

- Screen recording (with permission)
- Observer notes (what worked, what didn't)
- Quotes (especially pain points or delights)
- Task completion: Yes/No + Time taken

**After Sessions**:

- Compile notes in shared doc (Notion or Google Doc)
- Categorize feedback:
  - **Critical**: Must fix before development (e.g., "Totally confused by 4E")
  - **High**: Should fix (e.g., "Schedule button hard to find")
  - **Medium**: Nice to have (e.g., "Would love dark mode")
  - **Low**: Future consideration (e.g., "Calendar view would be cool")

**Metrics to Track**:

- Task success rate (% who completed without help)
- Average time per task
- Number of errors/wrong clicks
- SUS Score (System Usability Scale - optional survey)
- NPS (Net Promoter Score): "Likelihood to recommend (0-10)"

**Synthesis**:

- Identify patterns (if 3+ people have same issue → critical)
- Prioritize fixes for iteration
- Create action items with owners![ref24]

**7. Iteration & Refinement**

1. **Feedback Synthesis Meeting (Day 22)**

**Attendees**: Full team (product lead, tech lead, designer, Uwa Farah) **Agenda**:

1. **Share key findings** (30 min):
- Facilitator presents summary of user testing
- Highlight critical issues, repeated feedback, positive reactions
- Show video clips of key moments (confusion, delight)
2. **Prioritization exercise** (30 min):
- Group feedback into Must-Fix / Should-Fix / Nice-to-Have
- Estimate effort for each fix (1hr / half-day / 1 day)
- Decide: What changes before development? What defers to later?
3. **Assign action items** (15 min):
- Who fixes what?
- Deadline: 2-3 days for changes
4. **Re-validation plan** (15 min):
- Do we need another round of testing?
- Or just stakeholder sign-off after fixes?
2. **Common Issues & Solutions (Hypothetical)**

**Issue 1: "4E Feedback is confusing"**

- **Finding**: 3/5 parents unsure what "Earn" means
- **Solution**: Change wording to "Create" or add tooltip explanation
- **Effort**: 1 hour (update copy + add tooltip)

**Issue 2: "Too many steps to log activity"**

- **Finding**: Parents feel 3-step wizard is long
- **Solution**: Make photo upload optional, allow skip all steps except save
- **Effort**: 2 hours (adjust validation)

**Issue 3: "Can't find scheduled activities"**

- **Finding**: Users look for calendar icon but there's only a list
- **Solution**: Add calendar icon to navbar, more prominent "Upcoming" section
- **Effort**: 3 hours (new icon, reorder dashboard)

**Issue 4: "Admin form too long"**

- **Finding**: Uwa Farah team overwhelmed by 5-step wizard
- **Solution**: Collapse optional sections, make wizard progress clearer
- **Effort**: 4 hours (UI refactor)

**Issue 5: "Love the gamification!"**

- **Finding**: All parents excited about badges and streaks
- **Solution**: No change needed, validate this works! Maybe add more badges.
- **Effort**: 0 hours (keep as is)
3. **Iteration Sprint (Day 23-25)**

**Day 23-24**: Implement high-priority fixes

- Focus on critical usability issues
- Update copy where confusing
- Adjust layouts for clarity

**Day 25**: Final polish

- One more round of internal testing
- Fix any new bugs introduced
- Update documentation (if any screens changed significantly)
4. **Final Approval (Day 26)**

**Approval Meeting** (1 hour):

- Present updated prototype to stakeholders
- Walkthrough changes made based on feedback
- Get sign-off from:
  - Uwa Farah (content perspective)
  - Psikolog team (educational validation)
  - Product owner (requirements met)
  - Tech lead (feasible to implement)

**Deliverables**:

- ![ref1] Approved prototype (locked version)
- ![ref1] Validation report (summary of findings + changes made)
- ![ref1] Design spec exported from prototype (screenshots + annotations for developers)
- ![ref1] Dummy data files (ready to use as seed data in real app)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.067.png)

**8. Handoff to Development**

1. **Documentation Package**

**For Developers**:

1. **Prototype Access**:
- Live URL: [https://jejakanak-prototype.vercel.app](https://jejakanak-prototype.vercel.app/)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.068.png)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.069.png)
- Source code: GitHub repo (if open to team)
- Login credentials: [demo@jejakanak.app /](mailto:demo@jejakanak.app) password123![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.070.png)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.071.png)
2. **Screen Specifications**:
- Figma file (if exists) with final designs
- OR: Exported screenshots from prototype with annotations
- Spacing, colors, fonts documented (design system)
3. **User Flows**:
- Flow diagrams (from Section 2.2 of this doc)
- Critical paths highlighted
4. **Data Models**:
- JSON schema for each entity (activity, user, child, log)
- Relationships documented
- Sample data files (activities.json, users.json, etc.)
5. **Functional Requirements**:
- Feature list with detailed descriptions
- Edge cases identified during testing
- Known limitations of prototype (to be built properly in app)
6. **Testing Insights**:
- Validation report summary
- What worked well (keep as is)
- What was confusing (pay extra attention)
2. **Development Kickoff Meeting**

**Before Sprint 1** (Week 4 Day 1): **Agenda** (1.5 hours):

1. **Prototype Walkthrough** (30 min):
- Product lead demos prototype live
- Highlights key features and flows
- Explains why certain design decisions were made
2. **Technical Architecture Overview** (30 min):
- Tech lead presents high-level architecture (Flutter + NestJS + Postgres)
- Discusses how prototype maps to real implementation
- Identifies technical challenges
3. **Sprint 1 Planning** (30 min):
- Review Sprint 1 backlog (from masterplan)
- Assign tasks to developers (or AI coding sessions)
- Set Sprint 1 goal: "Working auth + child profile + basic activity browse"

**Outputs**:

- ![ref1] Development team understands requirements
- ![ref1] Sprint 1 tasks estimated and assigned
- ![ref1] Any blocking questions answered
3. **Prototype as Living Reference**

**Throughout Development**:

- Prototype stays deployed (URL bookmarked by all)
- Developers refer to prototype when unclear about UX
- QA testers use prototype as reference ("Does real app match prototype?")
- Product owner uses prototype to answer stakeholder questions

**Sunset Plan**:

- Prototype remains live until V1.0 launches
- After launch, archive prototype (keep GitHub repo for reference)![ref13]
9. **Success Metrics for Prototype Phase**
1. **Process Metrics**
- ![ref1] **Timeline Met**: Prototype completed in 2-3 weeks
- ![ref1] **Budget**: No cost (free tools + free hosting)
- ![ref1] **Coverage**: All 15 must-have screens built
- ![ref1] **Testing**: 5+ parent testers + psikolog team + content team validated
2. **Quality Metrics**
- ![ref1] **Usability**: Average task success rate > 80%
- ![ref1] **Satisfaction**: Average user rating > 4/5
- ![ref1] **NPS**: Average Net Promoter Score > 40 (good)
- ![ref1] **Clarity**: Zero critical confusions in testing
- ![ref1] **Approval**: All stakeholders sign off
3. **Outcome Metrics**
- ![ref1] **Requirements Refined**: 10+ adjustments made based on feedback
- ![ref1] **Risk Reduced**: Major UX issues caught early (not during development)
- ![ref1] **Alignment**: Team confident in what to build
- ![ref1] **Accelerated Development**: Developers have clear blueprint![ref4]
10. **Risks & Mitigation**
1. **Prototype-Specific Risks**

**Risk: Prototype takes longer than 3 weeks**

- **Mitigation**: Timebox strictly, cut nice-to-have screens if needed
- **Contingency**: Launch with 12 screens instead of 28, focus on core flows

**Risk: User testing reveals fundamental flaws (concept doesn't resonate)**

- **Mitigation**: Test early with 1-2 parents before building all screens
- **Contingency**: Pivot concept, rebuild prototype with new approach (adds 1-2 weeks)

**Risk: Psikolog team rejects educational approach**

- **Mitigation**: Involve them early in ideation, not just validation
- **Contingency**: Revise 4E framework or activity structure, iterate prototype

**Risk: Technical implementation is way harder than prototype suggests**

- **Mitigation**: Tech lead reviews prototype feasibility during build
- **Contingency**: Simplify certain features (e.g., less dynamic recommendations)

**Risk: Stakeholder disagreement on changes after testing**

- **Mitigation**: Clear decision-making framework (data-driven, product owner final say)
- **Contingency**: Escalate to senior leadership if deadlock
2. **Resource Risks**

**Risk: Designer unavailable (delays visual design)**

- **Mitigation**: Use pre-made Tailwind UI components, focus on functionality over aesthetics
- **Contingency**: Developer does basic design, iterate visuals later

**Risk: Not enough realistic photos for dummy data**

- **Mitigation**: Use Unsplash API (free high-quality photos)
- **Contingency**: Use illustrations or simple colored placeholders![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.072.png)
11. **Post-Prototype Action Items**
1. **Immediate Next Steps (After Approval)**

**Week 4 (Development Start)**:

1. **Archive Prototype** (1 hour):
- Tag version in GitHub:  v1.0-validated
- Export all screens as PDF (documentation)
- Update README with findings summary
2. **Extract Reusable Assets** (2 hours):
- Export color palette (Tailwind config → Flutter theme)
- Document typography scale (font sizes, weights)
- Save icon set (export SVGs)
- Collect dummy data files (use as seed data)
3. **Create Developer Handoff Doc** (3 hours):
- Screen-by-screen specifications
- Interaction notes ("On tap X, show modal Y")
- Copy all final text/copy (for consistency)
- List of edge cases discovered
4. **Setup Development Environment** (Per Masterplan):
- Initialize Flutter project
- Initialize NestJS backend
- Setup database schema
- Configure CI/CD pipeline
2. **Ongoing Prototype Maintenance**

**During Development (Week 4-16)**:

- Keep prototype live for reference
- If major design changes during dev, optionally update prototype (low priority)
- Use prototype for demos to investors/partners if needed

**After V1.0 Launch**:

- Archive prototype (no longer maintained)
- Keep GitHub repo as historical reference
- Document lessons learned in team wiki![ref2]

**12. Budget & Resources**

1. **Cost Breakdown**

**Development Costs**:

- Developer time: 2-3 weeks × 1 developer = **~120-180 hours**
  - If outsourced: Rp 150,000/hr × 150hr = Rp 22,500,000 (~$1,500 USD)
  - If internal: Opportunity cost only
- Designer time (if separate): ~20 hours for mockups
  - If outsourced: Rp 200,000/hr × 20hr = Rp 4,000,000 (~$270 USD)

**Infrastructure Costs**:

- Hosting (Vercel/Netlify): **Free** (for prototype scale)
- Domain (optional): Rp 150,000/year (~$10 USD)
- Stock photos: **Free** (Unsplash, Pexels)
- Design tools: **Free** (Figma free tier)

**Testing Costs**:

- User incentives: Rp 100,000/tester × 10 testers = Rp 1,000,000 (~$65 USD)
  - Or: Early access badge (no cash cost)

**Total Estimated Cost**: **Rp 0 - 27,500,000** (~$0-1,800 USD)

- Minimum (DIY, no outsourcing): Rp 0
- Maximum (outsource dev + design): Rp 27,500,000

**RECOMMENDATION**: Keep costs minimal (DIY), invest budget in actual app development instead

2. **Team Allocation**

**Required Roles**:

1. **Developer/Builder** (1 person, full-time 2-3 weeks):
- Skills: React/Vue, basic design sense
- Responsibilities: Build all screens, implement interactions, deploy
- Ideal candidate: You (familiar with Vue, can learn React quickly)
2. **Content Preparer** (1 person, part-time ~20 hours):
- Skills: Writing, child development knowledge
- Responsibilities: Create 50 activity descriptions, write copy
- Ideal candidate: Uwa Farah or team member
3. **Design Consultant** (1 person, part-time ~10 hours):
- Skills: UI/UX design
- Responsibilities: Create color scheme, suggest layouts, review screens
- Ideal candidate: Freelance designer or use AI tools (v0.dev, Galileo AI)
- **Alternative**: Skip this role, use Tailwind UI templates
4. **Validator/Tester** (1 person, part-time ~10 hours):
- Skills: QA mindset, attention to detail
- Responsibilities: Test all flows, document bugs, coordinate user testing
- Ideal candidate: Product owner or tech lead

**Optional**:

- **Copywriter**: For polished marketing copy (welcome screen, etc.)
- **Photographer**: For custom photos (or use stock)

**Minimum Team**: Just 1-2 people can build entire prototype (developer + content preparer)![ref25]

**13. Alternative: Low-Code Prototype Options**

1. **If Time is Extremely Constrained (1 Week Only)**

**Option: Figma Interactive Prototype Pros**:

- No coding (pure design tool)
- Very fast (1 week achievable)
- Professional-looking
- Easy to iterate (just edit design)

**Cons**:

- Less realistic (no real data handling)
- Limited interactivity (only link hotspots)
- Harder to simulate complex flows (multi-step forms)

**When to Use**: If team has no developers available and need validation ASAP

**How**:

1. Design all screens in Figma (use UI kits for speed)
1. Add interactive links (tap button → go to next screen)
1. Create multiple "paths" for different scenarios
1. Present mode = prototype
1. Share link with testers

**Effort**: ~40 hours (1 week)![ref25]

**Option: No-Code Builders (Bubble, Webflow, Softr) Pros**:

- Visual builder (drag-and-drop)
- Can handle data (better than Figma)
- Faster than code (for simple apps)

**Cons**:

- Learning curve (need to learn the tool)
- Limitations (complex interactions harder)
- Not free (most require subscription)
- Vendor lock-in (can't export code easily)

**When to Use**: If team wants semi-functional prototype with basic data handling but no coding **Recommendation**: **Not recommended** for JejakAnak prototype

- Why: Mobile app UX hard to replicate in no-code builders
- Learning new tool takes time (defeats speed purpose)
- Code-based prototype more flexible for iterations![ref24]
2. **Hybrid Approach (Recommended for Time Savings)**

**Strategy**: Design in Figma, Build Core Flows in Code **Week 1**: Design all screens in Figma (fast, visual)

- Day 1-3: Design 20 screens
- Day 4-5: Interactive prototype in Figma (clickable)
- Day 5: Present to team for early feedback

**Week 2**: Build critical flows in code (realistic)

- Only build: Onboarding, Browse, Log Activity (3 key flows)
- Skip: Settings, Admin, secondary features
- Use Figma as reference for styling

**Week 3**: User testing + iteration

- Test both Figma (for full coverage) and code prototype (for realism)
- Iterate based on feedback

**Benefits**:

- Figma gives full picture (all screens)
- Code prototype validates core interactions (most critical)
- Saves time (not coding everything)![ref24]

**14. Deliverables Checklist**

1. **At End of Prototype Phase (Day 26)**

**Must Have**:

` `Live prototype URL (accessible by anyone)![ref26]

` `Source code in GitHub (if code-based)![ref27]

` `Dummy data files (all JSON)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.076.png)

` `User testing report (findings + recommendations)![ref28]

` `Validation sign-off (from psikolog, Uwa Farah, parents)  Screenshots of all screens (for documentation)![ref29]![ref26]

` `Handoff document (for developers)![ref27]

**Should Have**:

` `Design system documented (colors, typography, components)  User flow diagrams (visual maps)![ref28]![ref29]

` `Demo video (5-min walkthrough of prototype)![ref26]

` `Lessons learned doc (what worked, what didn't)![ref27]

**Nice to Have**:

` `Figma file (parallel to code, for designers)![ref20]

` `Analytics setup (track clicks in prototype - optional)  A/B tested variations (if time permits)![ref21]![ref22]

2. **Success Declaration**

**Prototype Phase is Successful When**:

1. ![ref1] All 5 key user flows are clickable and realistic
1. ![ref1] 80%+ of testers successfully complete tasks without help
1. ![ref1] Psikolog team: "Educational approach is sound"
1. ![ref1] Uwa Farah team: "We can work with this admin panel"
1. ![ref1] Parent testers: Average NPS > 40 ("Would recommend")
1. ![ref1] Development team: "Clear what to build, confident we can"
1. ![ref1] Stakeholders: Unanimous approval to proceed
1. ![ref1] Timeline met: Completed in 2-3 weeks

**If Not All Criteria Met**:

- Extend prototype phase by 1 week (iteration)
- OR: Launch development with known risks (document them)
- OR: Pivot concept (if fundamental issues discovered)![ref24]
15. **Appendix: Resources & Tools**
1. **Recommended Tools**

**Design & Mockup**:

- Figma (free): figma.com
- Excalidraw (wireframes): excalidraw.com
- Whimsical (user flows): whimsical.com

**Front-End Development**:

- Vite (React setup): vitejs.dev
- Tailwind CSS: tailwindcss.com
- Headless UI (components): headlessui.com
- Heroicons (icons): heroicons.com
- Framer Motion (animations): framer.com/motion

**Dummy Data & Assets**:

- Unsplash (photos): unsplash.com
- Pexels (photos): pexels.com
- Lorem Picsum (placeholder images): picsum.photos
- Faker.js (generate fake data): fakerjs.dev
- Mockaroo (CSV generator): mockaroo.com

**Hosting & Deployment**:

- Vercel (free): vercel.com
- Netlify (free): netlify.com
- GitHub Pages (free): pages.github.com

**User Testing**:

- Zoom (video calls): zoom.us
- Loom (screen recording): loom.com
- Maze (user testing platform): maze.co
- Google Forms (surveys): forms.google.com

**Project Management**:

- Notion (docs + tasks): notion.so
- Trello (simple kanban): trello.com
- Miro (whiteboard): miro.com
2. **Sample Prompts for AI Assistance**

**For Generating Dummy Data**:

Generate 10 realistic child development activitiGenerate 10 realistic child development activities for ages 3-5 yeares for ages 3-5 years in Indonesia. s in Indonesia. ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.079.png)Each activity should include:Each activity should include:

- T- Title (in Bahasa Indonesia)itle (in Bahasa Indonesia)
- Description (2-3 sentences)- Description (2-3 sentences)
- Materials needed (list)- Materials needed (list)
- 4-5 step instructions- 4-5 step instructions
- Educational value (2-3 tags like "Creativity", "Fine Mot- Educational value (2-3 tags like "Creativity", "Fine Motor")or")
- Duration estimate- Duration estimate

  Format as JSON arrayFormat as JSON array..

**For Creating React Components**:

Create a React component called ActivityCard that diCreate a React component called ActivityCard that displays:splays:![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.080.png)

- Activity image (prop: imageUrl)- Activity image (prop: imageUrl)
- T- Title (prop: tititle (prop: title)le)
- Age range badge (pr- Age range badge (prop: ageMin, ageMax)op: ageMin, ageMax)
- Duration badge (prop: duration)- Duration badge (prop: duration)
- Favorite icon (heart, prop: isFavorite)- Favorite icon (heart, prop: isFavorite)

  Use TUse Tailwind CSS for styling. Card should have hover efailwind CSS for styling. Card should have hover effect and be clickable.fect and be clickable.

**For Writing Copy**:

WWrite 3 welcome screen slides for a parenting app called JejakAnak:rite 3 welcome screen slides for a parenting app called JejakAnak:![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.081.png)

- Slide 1: Introduce the app (document child's journey)- Slide 1: Introduce the app (document child's journey)
- Slide 2: Key feature (curated educational activities)- Slide 2: Key feature (curated educational activities)
- Slide 3: V- Slide 3: Value (discover child's talents)alue (discover child's talents)

  TTone: Wone: Warm, supportive, aspirational. Keep each to 2 sentences max.arm, supportive, aspirational. Keep each to 2 sentences max. TTararget audience: Indonesian parents (use Bahasa Indonesia)get audience: Indonesian parents (use Bahasa Indonesia)..

3. **Useful Code Snippets**

**Basic React Router Setup**:

jsx

importimport {{ BrowserRouterBrowserRouter,, RoutesRoutes,, RouteRoute }} fromfrom 'react-router'react-router-dom'-dom';; ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.082.png)importimport SplashSplash fromfrom './pages/Splash''./pages/Splash';;

importimport WWelcomeelcome fromfrom './pages/W'./pages/Welcome'elcome';;

importimport HomeHome fromfrom './pages/Home''./pages/Home';;

*// ... other pages// ... other pages*

functionfunction AppApp(()) {{

returnreturn ((

<<BrowserRouterBrowserRouter>>

<<RoutesRoutes>>

<<RouteRoute pathpath==""//"" elementelement=={{<<SplashSplash />/>}} />/>

<<RouteRoute pathpath==""/welcome/welcome"" elementelement=={{<<WWelcomeelcome />/>}} />/> <<RouteRoute pathpath==""/signup/signup"" elementelement=={{<<SignUpSignUp />/>}} />/>

<<RouteRoute pathpath==""/home/home"" elementelement=={{<<HomeHome />/>}} />/>

<<RouteRoute pathpath==""/library/library"" elementelement=={{<<ActivityLibraryActivityLibrary />/>}} />/> <<RouteRoute pathpath==""/activity/:/activity/:idid"" elementelement=={{<<ActivityDetailActivityDetail />/>}} />/> <<RouteRoute pathpath==""/log/log"" elementelement=={{<<LogActivityLogActivity />/>}} />/>

<<RouteRoute pathpath==""/timeli/timelinene"" elementelement=={{<<TTimelineimeline />/>}} />/> <<RouteRoute pathpath==""/insights/insights"" elementelement=={{<<ChildDashboardChildDashboard />/>}} />/> {{*/\* ... mor/\* ... more re routes \*/outes \*/*}}

</</RoutesRoutes>>

</</BrowserRouterBrowserRouter>>

));;

}}

**Loading JSON Data**:

constconst [[activitiesactivities,, setActivities setActivities]] == useStateuseState(([[]]));; constconst [[loadingloading,, setLoading setLoading]] == useStateuseState((truetrue));;

useEfuseEffectfect(((()) =>=> {{

fetchfetch(('/data/activit'/data/activities.json'ies.json'))

..thenthen((resres =>=> res res..jsonjson(())))

..thenthen((datadata =>=> {{

setActivitiessetActivities((datadata));;

setLoadingsetLoading((falsefalse));;

}}))

..catchcatch((errerr =>=> {{

consoleconsole..errorerror(('Failed to load activi'Failed to load activities:'ties:',, err err));; setLoadingsetLoading((falsefalse));;

}}));;

}},, [[]]));;

ifif ((loadingloading)) returnreturn <<divdiv>>Loading...Loading...</</divdiv>>;;

**Simple Filter Logic**:

constconst [[filtersfilters,, setFilters setFilters]] == useStateuseState(({{![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.083.png)

categorycategory:: 'all''all',,

ageMinageMin:: 00,,

ageMaxageMax:: 180180,,

searchsearch:: ''''

}}));;

constconst filteredActivities  filteredActivities == activities activities..filterfilter((activityactivity =>=> {{

*// Category fil// Category filterter*

ifif ((filtersfilters..categorycategory !==!== 'all''all' &&&& !!activityactivity..categoriescategories..includesincludes((filtersfilters..categorycategory)))) {{

returnreturn falsefalse;;

}}

*// Age filt// Age filter (child's age within activity range)er (child's age within activity range)* constconst childAge  childAge == selectedChild selectedChild..ageMonthsageMonths;; ifif ((childAge childAge << activity activity..ageMinMonthsageMinMonths ||||

`      `childAge       childAge >> activity activity..ageMaxMonthsageMaxMonths)) {{

returnreturn falsefalse;;

}}

*// Sear// Search filterch filter*

ifif ((filtersfilters..searchsearch &&&& !!activityactivity..titletitle..toLowerCasetoLowerCase(())..includesincludes((filtersfilters..searchsearch..toLowerCasetoLowerCase(()))))) {{

returnreturn falsefalse;;

}}

returnreturn truetrue;; }}));;

**Confetti Animation (Simple CSS)**:

*// Using r// Using react-confetti libraryeact-confetti library ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.084.png)*importimport ConfettiConfetti fromfrom 'react-confetti''react-confetti';; importimport {{ useState  useState }} fromfrom 'react''react';;

functionfunction SuccessScreenSuccessScreen(()) {{

constconst [[showConfettishowConfetti,, setShowConfetti setShowConfetti]] == useStateuseState((truetrue));;

useEfuseEffectfect(((()) =>=> {{

*// Stop confetti// Stop confetti after 5 seconds after 5 seconds*

constconst timer  timer == setTsetTimeoutimeout(((()) =>=> setShowConfettisetShowConfetti((falsefalse)),, 50005000));; returnreturn (()) =>=> clearTclearTimeoutimeout((timertimer));;

}},, [[]]));;

returnreturn ((

<<divdiv>>

{{showConfetti showConfetti &&&& <<ConfettiConfetti />/>}} <h1>Activity Logged! ![ref7]</h1> <<pp>>+10 XP earned+10 XP earned</</pp>>

</</divdiv>>

));;

}}![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.085.png)

16. **Conclusion**

This Dummy Prototype Master Plan provides a comprehensive roadmap for building a high-fidelity, interactive web prototype of JejakAnak in 2-3 weeks. By investing this time upfront, the team will:

1. **Validate Requirements**: Ensure all features are actually needed and well-designed
1. **Test UX**: Identify and fix usability issues before expensive development
1. **Align Stakeholders**: Get everyone on the same page (psikolog, educators, parents, tech team)
1. **Accelerate Development**: Provide clear blueprint for Flutter developers
1. **Reduce Risk**: Catch major problems early when they're cheap to fix

**Key Success Factors**:


- ![ref1] Realistic dummy data (not lorem ipsum)
- ![ref1] Interactive flows (clickable, not just static mockups)
- ![ref1] Actual user testing (5-10 people, structured sessions)
- ![ref1] Stakeholder validation (psikolog sign-off critical)
- ![ref1] Clear handoff (documentation for developers)

**Expected Outcomes**:

- Validated prototype (approved by all stakeholders)
- Refined requirements (10+ improvements from feedback)
- Confident team (clear vision, ready to build)
- Faster development (fewer surprises, less rework)

**Next Steps**:

1. Review this plan with team (30 min)
1. Assign prototype builder (1 developer)
1. Start Week 1 on Monday (setup + data prep)
1. Ship prototype by end of Week 3
1. Start development Week 4 with validated design

**Remember**: The prototype is disposable. Its value is in the learning, not the code. Don't over-engineer it. Build just enough to test hypotheses and validate decisions. Then throw it away and build the real thing properly in Flutter.

**Let's build something parents will love!** ![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.086.png)![](Aspose.Words.e6fa97ae-601e-49ce-8aec-7f7a4576c76d.087.png)

**Document Version**: 1.0

**Created**: October 20, 2025

**Owner**: JejakAnak Product Team **Status**: Ready for Execution

**Timeline**: Week 1-3 of Project Roadmap![ref12]

**END OF DUMMY PROTOTYPE MASTER PLAN**

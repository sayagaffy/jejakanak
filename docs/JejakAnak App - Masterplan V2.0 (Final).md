**JejakAnak App - Comprehensive Masterplan V2.0**

**Executive Summary**

**JejakAnak** adalah platform mobile yang membantu orangtua mendokumentasikan dan mengoptimalkan perjalanan tumbuh kembang anak dari masa kehamilan hingga remaja (prenatal - 15 tahun). Aplikasi ini menggabungkan curated educational content, activity logging, talent discovery melalui 4E framework (Enjoy, Easy, Excellent, Earn), gamification, dan community features untuk menciptakan ecosystem parenting yang engaging dan insightful.

**Filosofi Nama**: "Jejak Anak" melambangkan rekam jejak setiap langkah perjalanan anak, dimulai bahkan sebelum lahir, membentuk narasi lengkap tumbuh kembang yang dapat dilihat kembali di masa depan.

**Value Proposition**:

- **Untuk Orangtua**: Guidance terstruktur, dokumentasi memories, insights tentang minat/bakat anak
- **Untuk Anak**: Pengalaman edukatif yang terpersonalisasi dan terdokumentasi
- **Untuk Educator (Content Team)**: Platform untuk mendistribusikan konten edukatif berkualitas![ref1]

**1. Vision & Objectives**

1. **Vision Statement**

"Menjadi companion terpercaya orangtua Indonesia dalam membesarkan anak yang berkembang optimal sesuai potensinya, dengan mendokumentasikan setiap momen berharga dari kandungan hingga remaja."

2. **Primary Objectives**
1. **Documentation Excellence**: Menyediakan platform intuitif untuk mencatat milestone, aktivitas, dan memories anak dalam satu tempat
1. **Educational Guidance**: Menawarkan library aktivitas edukatif terstruktur, age-appropriate, dan ter-kurasi oleh ahli
1. **Talent Discovery**: Membantu orangtua mengidentifikasi minat dan bakat anak melalui 4E framework dan pattern recognition
1. **Parent Empowerment**: Memberikan insights actionable untuk mendukung perkembangan anak
1. **Community Building**: Memfasilitasi knowledge sharing antar orangtua (recipe exchange, play spots, tips)
1. **Long-term Engagement**: Menciptakan habit logging melalui gamification dan personalized recommendations
3. **Success Metrics (12 Months Post-Launch)**

**User Acquisition**:

- 50,000 registered users
- 25,000 monthly active users (MAU)
- 10,000+ children profiles created

**Engagement**:

- Average 3 activities logged per user per week
- 60% user retention rate (D30)
- 40% weekly active users (WAU/MAU ratio)

**Content**:

- 300+ curated activities across all age groups
- 20+ new activities added monthly
- 80% activity completion rate (users who start activity logging finish it)

**Community**:

- 500+ user-contributed content (recipes, tips, play spots)
- 5,000+ activity variations shared

**Quality**:

- Net Promoter Score (NPS) > 50
- 4.5+ rating on Play Store & App Store
- <2% churn rate monthly![ref2]
2. **Target Users**
1. **Primary Users: Parents & Guardians**

**Demographics**:

- Age: 25-45 years old
- Income: Middle to upper-middle class (able to afford smartphones and activities)
- Location: Urban/suburban Indonesia (initially Jakarta, Surabaya, Bandung, Medan, Bali)
- Tech-savvy: Comfortable using mobile apps

**Psychographics**:

- **Engaged Parents**: Actively involved in child's development
- **Education-conscious**: Value early childhood education
- **Community-oriented**: Seek support from fellow parents
- **Documentation enthusiasts**: Love capturing moments (Instagram generation)

**User Personas**:

**Persona 1: "Rina the First-Time Mom"**

- Age: 28, pregnant with first child
- Works: Marketing professional
- Pain points: Overwhelmed with parenting information, unsure how to prepare
- Needs: Structured guidance, prenatal activities, community support
- Goals: Be a prepared parent, document pregnancy journey

**Persona 2: "Budi the Active Dad"**

- Age: 35, has 2 kids (4 and 7 years old)
- Works: Entrepreneur, flexible schedule
- Pain points: Runs out of activity ideas, wants quality time with kids
- Needs: Diverse activity suggestions, track progress
- Goals: Bond with kids, discover their talents early

**Persona 3: "Siti the Organized Mom"**

- Age: 32, has 1 child (5 years old)
- Works: Part-time consultant
- Pain points: Forgets to document moments, wants systematic tracking
- Needs: Easy logging, insights on child development
- Goals: Be intentional with child's education, preserve memories
2. **Secondary Users: Educators & Content Creators**

**Uwa Farah's Content Team**:

- Child development experts, psychologists, early childhood educators
- Role: Create and curate educational activities
- Needs: Easy-to-use content management tools with guidance
- Pain points: Not tech-savvy, need structured templates

**Future Consideration**: External educators, parenting coaches who might contribute content

3. **Tertiary Users: Children (Indirect)**

**Age Range**: Prenatal to 15 years

- **Prenatal (0 months)**: Future child, activities for expectant mothers
- **Newborn (0-12 months)**: Sensory stimulation, bonding activities
- **Toddler (1-3 years)**: Motor skills, early exploration
- **Preschool (3-5 years)**: Creativity, pre-literacy
- **Early Elementary (6-8 years)**: Academic readiness, hobbies
- **Middle Childhood (9-11 years)**: Skill mastery, interests
- **Pre-teen (12-15 years)**: Identity, passion projects

**Note**: In V1, children do not directly operate the app. Parent-operated interface only.![ref2]

3. **Core Features (Version 1.0)**
1. **User Management & Profiles**

**User Registration & Authentication**

- Email/password signup with email verification
- Social login: Google, Apple (OAuth 2.0)
- Password reset via email
- Secure token-based authentication (JWT)

**Parent Profile**

- Full name, profile photo
- Email, phone (optional)
- Location (city-level for content personalization)
- Notification preferences
- Privacy settings

**Child Profile Management**

- Multiple children per account (unlimited)
- Per child:
  - Name, nickname
  - Birth date OR Expected Due Date (EDD)
  - Status: "Expecting" or "Born"
  - Profile photo/avatar
  - Gender (optional)
  - Notes (special considerations, allergies, etc.)
- Auto-calculation of age in months
- Automatic content filtering by age
- Transition flow: When baby born, update status and unlock newborn content
2. **Activity Library (Content Repository)**

**Content Structure** Each activity contains:

- **Basic Info**: Title, description (150 chars), slug
- **Classification**:
  - Age range (min/max in months)
  - Categories (multi-select: Art, Science, Outdoor, Physical, Music, Literacy, Cooking, Social)
  - Difficulty (Easy, Medium, Challenging)
  - Duration (15min, 30min, 1hr, 2hr+)
  - Location (Indoor, Outdoor, Both)
- **Materials Needed**: List with quantities, common vs special items flag
- **Instructions**: Numbered steps with optional images per step
- **Educational Value**:
  - Learning outcomes (Fine Motor, Gross Motor, Creativity, Problem Solving, Language, Social Skills, etc.)
  - Parent tips (how to facilitate)
  - Conversation starters (questions to ask child)
  - Safety notes (if applicable)
- **Media**: Main image, 0-5 additional images, optional video URL (YouTube/Vimeo)
- **Metadata**: Created by, status (draft/pending/published), publish date, popularity score

**Browsing & Discovery**

- **Home View**: Personalized recommendations (see section 3.3)
- **Library View**:
  - Grid or list display
  - Filters: Age range, category, difficulty, duration, location
  - Search: By title, keywords
  - Sort: Popular, newest, A-Z, duration
- **Category Pages**: Browse by specific category
- **Activity Detail**: Full-screen view with all content

**Content Lifecycle**

- Content created by admin team via Admin Panel (see 3.9)
- Status flow: Draft → Pending Review → Published
- Continuous updates: New activities added weekly (target: 5-10/week)
- Launch target: 100+ activities across all age groups
3. **Personalized Recommendations**

**Recommendation Engine (Rule-Based for V1) Algorithm Factors**:

1. **Age-appropriate**: Filter by child's current age
1. **Category balance**: Suggest categories child hasn't tried recently
1. **Interest alignment**: Prioritize categories where child showed high "Enjoy" in 4E
1. **Skill progression**: Match difficulty to child's demonstrated capability
1. **Recency**: Avoid recently completed activities (30-day window)
1. **Popularity**: Slight boost for highly-rated activities
1. **Trending**: Highlight new content (published within 2 weeks)

**Presentation**:

- "Recommended for [Child Name]" section on home dashboard
- 5 activity cards with reasons: "Because Rina loves Art activities" or "Time to try something new!"
- Refresh daily or after each logged activity

**Future Enhancement (V2)**: Machine learning model for deeper personalization

4. **Activity Scheduling**

**Schedule Feature**

- From activity detail page: "Schedule" button
- User selects:
  - Date (calendar picker)
  - Time (optional, time picker)
  - Reminder: 15min / 1 hour / 1 day before
  - Personal notes (e.g., "Prepare materials the night before")
- Scheduled activities appear in:
  - "Upcoming Activities" section on dashboard
  - Calendar view (optional feature)
- Edit or cancel schedule anytime

**Reminders**

- Push notification at scheduled time minus reminder offset
- Notification content:
  - " ![ref3] Reminder: 'Finger Painting' activity in 1 hour!"
  - Action: Tap to open activity detail
  - Option to reschedule or mark as done
5. **Activity Logging & Journaling**

**Core Logging Flow Step 1: Initiate Log**

- From activity detail: "Mark as Done" button
- Or from scheduled activity: Quick log shortcut

**Step 2: Upload Photos**

- Camera integration: Take photo directly
- Gallery picker: Select 1-10 existing photos
- Per photo: Optional caption
- Auto-compression before upload (max 2MB per photo)
- Photos stored in cloud (S3) with CDN

**Step 3: Write Notes**

- Free-text field (max 500 characters)
- Placeholder prompts: "How did [child] enjoy this? Any highlights?"
- Optional: Voice-to-text for convenience

**Step 4: 4E Framework Feedback** Visual toggles for:

- ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.004.png) **Enjoy**: Did they love it?
  - Options: Yes / Neutral / No
- ![ref4] **Easy**: Was it challenging?
  - Options: Too Easy / Just Right / Challenging
- ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.006.png) **Excellent**: Did they excel?
  - Options: Yes / Okay / Struggled
- ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.007.png) **Earn**: Did they create/produce something?
  - Options: Yes / No

**Step 5: Additional Options**

- Mark as favorite ( ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.008.png))
- Tag location (if applicable, link to play spot)
- Add custom tags (optional)

**Step 6: Save**

- Confirmation animation with confetti
- XP points awarded (+10 base, +5 for photo, +5 for detailed notes)
- Check for badge unlocks
- Prompt: "Share your variation?" (if applicable)

**Activity Timeline (Journal View)**

- Chronological display of all logged activities for a child
- Month/year section headers
- Each entry card shows:
  - Activity title & category
  - Date completed
  - Thumbnail photo(s)
  - Short preview of notes
  - 4E badges (icons showing ratings)
- Tap card to view full log details
- Filter timeline: By category, date range, favorites
- Export timeline: PDF or shareable image (future feature)
6. **Child Dashboard & Insights**

**Dashboard Layout Header**:

- Child photo, name, age
- Current streak: " ![ref5] 5-day streak!"
- Level badge: "Level 3 - Active Parent"

**Quick Stats Cards**:

- Total activities completed
- Categories explored (e.g., "6 out of 8")
- Photos uploaded
- Favorite category (most logged)

**Activity Breakdown Chart**:

- Pie chart or bar chart
- Shows distribution across categories
- Interactive: Tap segment to filter timeline

**Talent Indicators Section**:

- AI-generated insights (rule-based V1):
  - " ![ref6] Rina shows strong creative talent!"
    - "Based on 8 Art activities where she excelled and enjoyed"
  - " ![ref7] Consider science classes for Budi"
    - "He finds Science activities easy and often excels"
- Confidence level indicator (Low/Medium/High)
- Action button: "Explore more [category] activities"

**Areas to Explore**:

- Categories with low or zero activity count
- " ![ref8] You haven't tried Music activities yet! Here are 3 to start:"
- Carousel of recommended activities

**Recent Memories**:

- Last 3-5 logged activities with photos
- Quick access to timeline

**Insights Generation Logic Triggers**:

- Recalculate after every 5 new activities logged
- Or weekly batch processing

**Pattern Detection**:

IF child has >= 10 activities in category XIF child has >= 10 activities in category X![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.013.png)

AND Enjoy rate in category X > 70%AND Enjoy rate in category X > 70%

AND Excellent rate in category X > 50%AND Excellent rate in category X > 50%

THEN generate insight: "[Child] shows talent in [category]"THEN generate insight: "[Child] shows talent in [category]" CONFIDENCE: High if >= 15 activities, Medium if 10-14CONFIDENCE: High if >= 15 activities, Medium if 10-14

IF child has 0 activities in category YIF child has 0 activities in category Y

AND child's age is appropriate for category YAND child's age is appropriate for category Y THEN generate suggestion: "TTHEN generate suggestion: "Try [category Y]"ry [category Y]"

IF child's difIF child's difficulty progression shows 80%+ "Just Right" or "Challenging"ficulty progression shows 80%+ "Just Right" or "Challenging" THEN generate insight: "Ready for advanced activities in [categories]"THEN generate insight: "Ready for advanced activities in [categories]"

7. **Gamification System**

**Experience Points (XP) & Levels XP Sources**:

- Log activity: +10 XP
- Add photo: +5 XP per photo (max +25)
- Write detailed notes (>50 chars): +5 XP
- Complete 4E feedback: +5 XP
- Try new category (first time): +20 XP
- Schedule activity in advance: +3 XP
- Share recipe/tip: +15 XP
- Help other parents (content marked helpful): +10 XP

**Level System**:

- Formula: Level = floor(sqrt(XP / 100)) + 1
- Levels:
  - Lv 1 (0-100 XP): Newbie Parent  ![ref9]
  - Lv 2 (100-400 XP): Engaged Parent  ![ref10]
  - Lv 3 (400-900 XP): Active Parent  ![ref11]
  - Lv 4 (900-1600 XP): Super Parent  ![ref12]
  - Lv 5 (1600+ XP): Legendary Parent  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.018.png)

**Level-Up Benefits**:

- Unlock special badge border color
- Notification: " ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.019.png) Level Up! You're now Level 3!"
- Social sharing: Share achievement on social media

**Achievement Badges Badge Types** (20+ total):

- **Early Bird ![ref9]**: Log first 5 activities
- **Memory Keeper**  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.020.png): Upload 20 photos
- **Storyteller ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.021.png)**: Write 10 detailed notes
- **Art Explorer**  ![ref6]: Complete 10 Art activities
- **Science Guru ![ref7]**: Complete 10 Science activities
- **Outdoor Adventurer**  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.022.png): Complete 10 Outdoor activities
- **Well-Rounded** ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.023.png): Try all 8 categories
- **Week Warrior ![ref5]** : 7-day activity streak
- **Month Master** ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.024.png): 30-day activity streak
- **Century Club**  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.025.png): Log 100 activities
- **Helpful Parent**  ![ref8] : Share 5 tips/recipes
- **Community Star**  ![ref11]: 20 contributions marked helpful
- **Early Adopter ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.026.png)**: Join during launch month
- **Consistency Champion**  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.027.png) : Log activities 4 weeks consecutively
- **Photo Pro**  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.028.png): Upload 100 photos
- **Category King/Queen**: Master one category (50 activities)
- **Talent Scout**  ![ref13]: Unlock 3 talent insights for child

**Badge Display**:

- Profile showcase page (grid of earned badges)
- Grayscale locked badges (show progress toward unlock)
- Badge detail modal: Description, earn date, rarity %
- Social sharing: "I just earned [badge]!" template

**Streaks Activity Streak**:

- Counts consecutive days with at least 1 logged activity
- Display on dashboard: " ![ref5] 7-day streak! Keep it going!"
- Notification if streak at risk: "Don't break your 10-day streak! Log an activity today."
- Streak freeze: 2 free freeze days per month (auto-applied on first miss)

**Milestone Celebrations**:

- 7 days: Badge + encouraging message
- 30 days: Badge + feature in app spotlight
- 100 days: Legendary badge + special reward (unlock premium content?)

**Monthly Challenges**

**Challenge System**:

- Admin creates challenges each month
- Examples:
  - "October Outdoor Adventure": Complete 5 outdoor activities
  - "November Creativity Month": Try 3 different Art activities
  - "December Family Time": Log 10 activities total
- User joins challenge (opt-in)
- Progress tracker: "3/5 completed"
- Rewards: Exclusive badge, bonus XP, feature in challenge leaderboard

**Challenge Display**:

- Dedicated "Challenges" tab in app
- Active challenges at top
- Past challenges (with completion status)
- No competitive leaderboards (to avoid pressure)
8. **Notification System**

**Notification Types**

1. **Scheduled Reminders**
- Trigger: X minutes before scheduled activity
- Content: " ![ref3] [Activity name] starts in [time]! Ready to begin?"
- Actions: [Open Activity] [Snooze] [Cancel]
2. **Engagement Nudges**
- Trigger: 3 days without activity logging
- Content: "Miss you!  ![ref4] [Child name] would love trying this: [Activity suggestion]"
- Frequency: Max once per week
3. **Weekly Digest**
- Trigger: Every Monday 9 AM
- Content: "Week ahead! 5 new activities added + Personalized picks for [Child]"
- Includes: Activity cards, child's stats summary
4. **Milestone Celebrations**
- Trigger: Achievement unlocked
- Content: " ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.030.png) Wow! [Child] completed 10 activities! You're amazing."
- Actions: [View Progress] [Share]
5. **Badge Earned**
- Trigger: Immediate on badge unlock
- Content: "Achievement Unlocked!  ![ref12] [Badge name]"
- Actions: [View Badge] [Share]
6. **New Content Alerts**
- Trigger: Weekly content publish
- Content: "[X] new activities perfect for [Child age]!  ![ref13]"
- Frequency: Weekly (Fridays)
7. **Streak Warnings**
- Trigger: 18 hours since last activity if streak active
- Content: " ![ref5] Keep your [X]-day streak alive! Quick activity idea: ..."
- Frequency: Max once daily
8. **Community Updates**
- Trigger: User's contribution approved
- Content: "Your recipe is live!  ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.031.png) Other parents will love it."
- OR: "5 parents found your tip helpful! +50 XP"
9. **Insight Generation**
- Trigger: New insight computed
- Content: " ![ref8] New insight about [Child]: [Insight summary]"
- Actions: [View Full Insight]
10. **Challenge Updates**
- Trigger: Progress milestones
- Content: "Halfway there! 3 more activities to complete October Challenge."

**User Controls**

- Notification preferences in settings:
  - Toggle each type on/off
  - Quiet hours (e.g., 10 PM - 7 AM)
  - Delivery channel: Push / Email / Both
- Default: All enabled except engagement nudges (opt-in)

**Implementation**

- **Push Notifications**: Firebase Cloud Messaging (FCM)
- **Email Notifications**: SendGrid or AWS SES (for digests, important alerts)
- **In-App Notifications**: Bell icon with badge count, dropdown list
9. **Admin Panel (Content Management)**

**Access & Roles Admin Roles**:

- **Super Admin**: Full access (tech team)
- **Content Manager**: Create, edit, publish content (Uwa Farah)
- **Content Creator**: Create, submit for review (Uwa Farah's team)
- **Reviewer**: Approve/reject user-generated content

**Authentication**:

- Separate login from parent app
- Role-based access control (RBAC)
- Activity logging for audit trail

**Features Dashboard Home**:

- Quick stats:
  - Total activities published
  - Pending review count
  - This week's user completions
  - Most popular activity (trending)
- Recent user activity feed (sample logs)
- Quick actions: Create Activity, Review Queue

**Create/Edit Activity**:

**Step 1: Choose Template**

- Pre-structured templates by category:
  - ![ref6] Art & Craft Activity
  - ![ref7] Science Experiment
  - ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.032.png) Physical Activity
  - ![ref10] Literacy & Reading
  - ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.033.png) Cooking & Nutrition
  - ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.034.png) Music & Rhythm
  - ![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.035.png) Outdoor Exploration
  - ![ref4] General/Custom
- Each template has pre-filled sections with placeholders

**Step 2-5: Form Wizard** (as detailed in discussion)

- Basic Info (title, age, categories, difficulty, duration, location)
- Materials & Prep
- Instructions (steps with image uploads)
- Educational Value (learning outcomes, tips, conversation starters)
- Media & Preview

**Validation System**:

- Required field checks
- Character limits enforced
- Image size/format validation
- Warning for missing recommended fields
- Preview mode: See mobile app view before publish

**Bulk Import**:

- CSV/Excel template download
- Upload file with parsed data
- Preview import with error highlights
- Bulk create as drafts
- Review individually before publishing

**Activity Library Management**:

- List view with filters (status, category, date)
- Search by title
- Bulk actions: Publish, archive, delete
- Edit existing activities
- Duplicate activity (as starting template)
- View analytics per activity (completion rate, ratings)

**Review Queue**:

- List of pending content:
  - User-submitted recipes
  - Activity variations
  - Play spots
  - Parent tips
- Per item:
  - Content preview
  - Submitter info
  - Actions: Approve, Reject, Request Changes
  - Text field for reviewer notes
- Filter by content type, date, priority

**Content Analytics**:

- Activity performance:
  - Views, completion rate, average rating
  - 4E feedback aggregates
  - Most logged activities (trending)
- User engagement:
  - Total active users
  - Activities logged per day/week
  - Category popularity distribution
- Community contributions:
  - Submissions per week
  - Approval rate
  - Top contributors

**User Management** (Super Admin only):

- View registered users
- Search by email, name
- User activity summary
- Moderate reported content
- Ban/unban users (safety)

**Challenge Management**:

- Create monthly challenges
- Set criteria (type, target, duration)
- Define rewards (badge, XP)
- View participation stats
- End challenge and distribute rewards

**Technical Implementation**

- **Platform**: Web-based (responsive design)
- **Framework**: React or Vue.js SPA
- **Backend**: Same NestJS API (admin routes)
- **Authentication**: Separate JWT for admin users
- **Hosting**: Same infrastructure, different subdomain (admin.jejakanak.com)

**Alternative Option**: Leverage Strapi CMS

- Headless CMS with admin panel out-of-the-box
- Customize content types for Activity, etc.
- Faster setup, trade-off on customization
- Decision: Evaluate during Phase 0 (prototype)
10. **Community Features (Phased Rollout)**

**Phase 1 (V1.0): Activity Variations User Flow**:

- After logging activity, optional prompt: "Try something unique? Share your variation!"
- Submit:
  - Short note (max 280 chars)
  - 1 photo (optional)
- Moderation:
  - Auto-approve if passes profanity filter
  - Manual review queue for edge cases
- Display:
  - On activity detail page, section "Other Parents' Ideas"
  - Carousel of variation cards
  - "Helpful" button (upvote)

**Safety**:

- No child face recognition enforcement (privacy)
- Report button for inappropriate content
- Admin review for flagged content

**Phase 2 (V1.5): Recipe Exchange User Flow**:

- For cooking-category activities only
- Submit full recipe:
  - Title, ingredients (structured list), steps, photo
  - Prep time, servings, dietary tags (optional)
- Moderation:
  - Uwa Farah team reviews (food safety check)
  - Approve/reject with feedback
- Display:
  - "Parent Recipes" tab on cooking activities
  - Filter by dietary preference (future)

**Incentive**:

- Badge: "Recipe Contributor" after 1st approval
- Badge: "Master Chef" after 10 approvals
- XP rewards: +15 per approved recipe

**Phase 3 (V1.5): Play Spots Database**

**User Flow**:

- When logging outdoor activity, option to "Tag Location"
- Search existing spots OR add new:
  - Name, type (playground, park, mall play area, etc.)
  - Address (Google Maps autocomplete)
  - Facilities checkboxes (parking, restroom, food, wheelchair access)
  - Age suitability estimate
  - Photo (optional)
  - Short note (max 200 chars)
- Auto-publish (lightweight moderation)

**Discovery**:

- "Play Spots Near You" section in app
- Map view with pins
- List view with distance, rating (upvote count)
- Filter: Type, age, facilities
- Each spot shows:
  - Activities logged here (count)
  - Parent notes/reviews
  - [Get Directions] button (Google Maps deep link)

**Community Curation**:

- Upvote/downvote system
- Admin can merge duplicates or remove spam

**Phase 4 (V2.0+): Parent Tips Forum Structure**:

- Categories: Activity Hacks, Nutrition, Sleep, Books, General
- User posts: Title, body (max 1000 chars), optional photo
- Tags (pre-defined)
- Engagement: Helpful button, Save/bookmark, Comments

**Moderation**:

- Pre-moderation (all posts reviewed before publish)
- Uwa Farah team can feature best posts
- Clear community guidelines

**Future**: Direct messaging, parent groups (with heavy safety considerations)![ref14]

4. **Technology Stack**
1. **Mobile Application**

**Framework**: Flutter (Dart) **Rationale**:

- Cross-platform (Android & iOS from single codebase)
- Near-native performance
- Hot reload for rapid development
- Mature ecosystem (50,000+ packages)
- Large developer community (1M+ active developers globally)
- Strong documentation and Google backing
- AI coding assistants (Claude, Codex) well-trained on Dart/Flutter

**Key Libraries**:

- **State Management**: Riverpod or Provider (proven, simple)
- **Networking**: Dio (HTTP client with interceptors)
- **Local Storage**: Hive or SharedPreferences (lightweight)
- **Image Handling**: image\_picker, cached\_network\_image, flutter\_image\_compress
- **Navigation**: go\_router (declarative routing)
- **UI Components**: Material Design 3 widgets
- **Charts**: fl\_chart (for dashboard visualizations)
- **Maps**: google\_maps\_flutter (for play spots)
- **Notifications**: firebase\_messaging (FCM)
- **Camera**: camera package
- **Analytics**: firebase\_analytics
- **Crash Reporting**: firebase\_crashlytics

**Architecture Pattern**: Clean Architecture + Feature-First Structure

lib/lib/![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.037.png)

├──├── core/ core/

││ ├──├── network/ network/

││ ├──├── storage/ storage/

││ ├──├── utils/ utils/

││ └──└── theme/ theme/

├──├── features/ features/

││ ├──├── auth/ auth/

││ ││ ├──├── data/ (repositories, models) data/ (repositories, models)

││ ││ ├──├── domain/ (entit domain/ (entities, use cases)ies, use cases)

││ ││ └──└── presentation/ (screens, widgets, providers) presentation/ (screens, widgets, providers) ││ ├──├── activiti activities/es/

││ ├──├── logging/ logging/

││ ├──├── dashboard/ dashboard/

││ └──└── ... ...

└──└── main.dart main.dart

2. **Backend Server**

**Runtime**: Node.js (v20 LTS) **Framework**: NestJS (TypeScript) **Rationale**:

- Modular architecture by design
- TypeScript for type safety and maintainability
- Built on Express (proven web server)
- Dependency injection (enterprise-grade)
- Extensive middleware ecosystem
- Well-documented, widely adopted
- AI coding assistants proficient in TypeScript

**Project Structure**:

src/src/![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.038.png)

├──├── modules/ modules/

││ ├──├── auth/ auth/

││ ├──├── users/ users/

││ ├──├── children/ children/

││ ├──├── activiti activities/es/

││ ├──├── activity-logs/ activity-logs/

││ ├──├── recommendations/ recommendations/ ││ ├──├── gamification/ gamification/

││ ├──├── notifications/ notifications/

││ ├──├── community/ community/

││ └──└── admin/ admin/

├──├── common/ common/

││ ├──├── decorators/ decorators/

││ ├──├── filters/ filters/

││ ├──├── guards/ guards/

││ ├──├── interceptors/ interceptors/

││ └──└── pipes/ pipes/

├──├── config/ config/

├──├── database/ database/

└──└── main.ts main.ts

**Key Libraries**:

- **ORM**: Prisma (modern, type-safe database access)
- **Validation**: class-validator, class-transformer
- **Authentication**: @nestjs/jwt, @nestjs/passport
- **File Upload**: multer, AWS SDK (for S3)
- **Task Scheduling**: @nestjs/schedule (for cron jobs)
- **Caching**: @nestjs/cache-manager (with Redis)
- **Logging**: winston, morgan
- **Testing**: Jest (unit & integration tests)
- **API Documentation**: @nestjs/swagger (auto-generated docs)
- **Email**: nodemailer or SendGrid SDK

**API Design**:

- RESTful principles
- Versioned endpoints:  /api/v1/...
- Consistent response format:

json![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.039.png)

{{

"success""success":: truetrue,,

"data""data":: {{ ...  ... }},,

"message""message":: "...""...",,

"timestamp""timestamp":: "2025-10-20T"2025-10-20T..."..."

}}

- Error handling: Standard HTTP codes + descriptive messages
- Rate limiting: By IP and user (prevent abuse)
- CORS enabled for mobile app
3. **Database**

**Primary Database**: PostgreSQL 15+ **Rationale**:

- ACID compliance (data integrity critical for children's data)
- Robust relational model fits our data structure
- JSONB support (flexibility for 4E feedback, nested data)
- Most popular database among developers (49% usage)
- Excellent performance and scalability
- Rich ecosystem of tools and extensions
- Proven in production at scale

**Schema Management**:

- Prisma ORM for schema definition and migrations
- Version-controlled migrations
- Seed scripts for initial data (categories, badges, etc.)

**Key Tables** (see Section 6 for full schema):

- users, children, activities, activity\_logs, scheduled\_activities
- user\_badges, challenges, child\_insights
- play\_spots, activity\_variations, parent\_recipes
- notifications, push\_tokens

**Database Hosting**:

- **Production**: AWS RDS PostgreSQL (managed service)
  - Automated backups (daily)
  - Multi-AZ deployment (high availability)
  - Read replicas (if needed for scaling)
- **Development**: Local PostgreSQL or Docker container

**Caching Layer**: Redis (optional for V1, recommended for V2)

- Cache frequently accessed data (categories, featured activities)
- Session storage (if needed)
- Rate limiting counters
- Leaderboard/stats (if real-time needed)
4. **File Storage & CDN**
4. **File Storage & CDN**

**Storage**: AWS S3

- Photo uploads stored in private buckets
- Organized by user/child ID
- Lifecycle policies: Move old photos to cheaper storage (Glacier)

**CDN**: AWS CloudFront

- Fast global delivery of images
- Signed URLs for private content (child photos)
- Caching strategy: Long TTL for activity images, shorter for user content

**Image Processing**:

- Client-side compression (Flutter)
- Optional: AWS Lambda for additional resizing/optimization on upload
5. **Cloud Infrastructure**

**Provider**: AWS (Amazon Web Services) **Rationale**:

- Market leader, most mature cloud platform
- Comprehensive service catalog
- Strong documentation and community
- Compliance certifications (important for children's data)
- Regional availability (ap-southeast-1 for Indonesia)

**Services Used**:

- **Compute**: ECS Fargate (containerized backend, serverless)
- **Database**: RDS PostgreSQL
- **Storage**: S3 + CloudFront CDN
- **Networking**: VPC, ALB (Application Load Balancer)
- **Monitoring**: CloudWatch (logs, metrics, alarms)
- **Secrets**: AWS Secrets Manager (API keys, DB passwords)
- **Email**: SES (transactional emails)

**Alternative Consideration**: Google Cloud Platform or Azure (if team has existing expertise)

6. **Push Notifications**

**Service**: Firebase Cloud Messaging (FCM) **Rationale**:

- Free
- Cross-platform (Android, iOS, Web)
- Reliable delivery
- Topic-based and targeted messaging
- Well-documented Flutter integration

**Implementation**:

- Backend sends messages via FCM Admin SDK
- Mobile app receives with firebase\_messaging package
- Token management: Store device tokens in database
- Topics for broadcast: "all\_users", "new\_content", etc.
7. **Analytics & Monitoring**

**User Analytics**: Firebase Analytics + Google Analytics 4

- Event tracking (activity\_logged, badge\_earned, etc.)
- User demographics
- Retention cohorts
- Funnel analysis

**Error Tracking**: Sentry

- Real-time error alerts
- Stack traces with context
- Release tracking
- Performance monitoring

**Application Monitoring**: AWS CloudWatch + Grafana

- Server metrics (CPU, memory, request rate)
- Custom dashboards
- Alerting (Slack/email on critical events)

**Logging**: Winston (structured JSON logs) → CloudWatch Logs

- Centralized logging
- Searchable and filterable
- Retention policy: 90 days
8. **CI/CD & DevOps**

**Version Control**: Git + GitHub **CI/CD**: GitHub Actions

- **Pipeline**:
  - On push to  dev branch: Run tests, lint, build → Deploy to staging
  - On push to  main branch: Run tests, build → Deploy to production
  - Manual approval for production deployments

**Containerization**: Docker

- Dockerfile for backend
- Docker Compose for local development (backend + PostgreSQL + Redis)

**Infrastructure as Code**: Terraform or AWS CloudFormation

- Define all AWS resources in code
- Reproducible environments (staging, production)
- Version-controlled infrastructure

**Environments**:

- **Development**: Local machines
- **Staging**: AWS environment (mirror of production, smaller scale)
- **Production**: AWS environment (auto-scaling, multi-AZ)

**Deployment Strategy**:

- Backend: Blue-green deployment via ECS (zero downtime)
- Mobile App: Phased rollout on Play Store/App Store (10% → 50% → 100%)
9. **Third-Party Integrations**

**Maps**: Google Maps API

- Geocoding for play spot addresses
- Map display in Flutter app
- Directions deep link

**Social Login**: Google Sign-In, Sign in with Apple

- OAuth 2.0 flow
- Reduced friction for user registration

**Email Service**: SendGrid or AWS SES

- Transactional emails (verification, password reset)
- Digest emails (weekly summary)

**Payment Gateway** (Future - if monetization):

- Midtrans (Indonesia-focused) or Stripe
10. **Security Considerations**

**Data Protection**:

- HTTPS everywhere (TLS 1.3)
- Encrypted database connections
- Encrypted S3 buckets (AES-256)
- Environment variables for secrets (never in code)

**Authentication & Authorization**:

- JWT with short expiry (1 hour) + refresh tokens
- Role-based access control (RBAC) for admin panel
- Password hashing: bcrypt (10 rounds)

**Input Validation**:

- All user input validated and sanitized
- Protection against: SQL injection, XSS, CSRF
- Rate limiting on API endpoints

**Privacy**:

- GDPR-compliant data handling (if targeting EU users)
- Privacy policy clearly displayed
- User data export feature (future)
- Account deletion cascade (remove all child data)
- Photos: Private by default, parent controls sharing

**Child Safety**:

- No public child profiles
- Moderation for all user-generated content with children
- Reporting mechanism for inappropriate content
- No direct messaging in V1 (to prevent misuse)![ref14]
5. **Development Roadmap**
1. **Phase 0: Foundation & Validation (Week 1-3)**

**Week 1**:

[![ref15]] Finalize requirements (this masterplan)

[![ref15]] Stakeholder alignment (team meeting)

` `Create detailed user stories (product backlog)  Design sprint kickoff![ref16]![ref17]

**Week 2-3**:

` `Figma design: All key screens (20-25 screens)![ref18]

` `Build dummy web prototype (interactive, realistic data)![ref19]

` `Uwa Farah team: Prepare 30 seed activities (across age groups)  Validation sessions:![ref20]![ref21]

- Psikolog team review (2 hrs)
- Educator team review (2 hrs)
- Parent user testing (5 parents, 1 hr each)  Iterate prototype based on feedback![ref16]

` `Final design sign-off![ref17]

**Deliverables**:

- Figma design system + mockups
- Clickable web prototype
- Validation report (feedback summary)
- Prioritized feature backlog
2. **Phase 1: MVP Alpha (Week 4-9) - 6 weeks**

**Goal**: Core value loop functional **Sprint 1 (Week 4-5): Foundation**

` `Project setup (GitHub repos, CI/CD)![ref22]

` `Backend scaffolding (NestJS modules)  Flutter app scaffolding![ref16]![ref17]

` `Database schema + migrations![ref23]

` `Auth system (registration, login, JWT)  User profile management![ref24]![ref22]

` `Child profile CRUD![ref16]

**Sprint 2 (Week 6-7): Content & Browsing**

` `Activity model + API endpoints![ref23]

` `Admin panel V0.1 (basic activity creation)  Seed 50+ activities (Uwa Farah team)![ref24]![ref22]

` `Activity library UI (browse, filter, search)  Activity detail page![ref16]![ref17]

` `AWS S3 integration (image uploads)![ref23]

**Sprint 3 (Week 8-9): Logging & Timeline**

` `Activity logging flow (photos, notes, 4E)  Timeline view (child's activity history)![ref18]![ref19]

` `Activity scheduling feature![ref20]

` `Basic dashboard (stats cards)![ref21]

` `Push notification setup (FCM)![ref25]

**Testing**:

` `Unit tests for critical backend logic  Integration tests (API endpoints)![ref19]![ref20]

` `Flutter widget tests (key screens)![ref21]

` `Manual QA (test all flows)![ref25]

**Alpha Release**:

` `Deploy to staging environment  Internal team testing (10 users)  Bug bash session![ref19]![ref20]![ref21]

` `Iterate based on feedback![ref25]

**Deliverables**:

- Functional MVP: Auth, Browse, Schedule, Log, Timeline
- 50+ activities in database
- Deployed on staging
3. **Phase 2: MVP Beta (Week 10-13) - 4 weeks**

**Goal**: Add intelligence & engagement

**Sprint 4 (Week 10-11): Recommendations & Insights**

` `Recommendation algorithm implementation  Insights generation logic (pattern detection)  Enhanced dashboard (insights section)![ref19]![ref20]![ref21]

` `"Recommended for You" section on home![ref25]

**Sprint 5 (Week 12-13): Gamification & Admin**

` `Gamification system (XP, levels, badges, streaks)  Milestone celebrations![ref18]![ref19]

` `Challenge system![ref20]

` `Admin panel enhancement:![ref21]

- Template-based activity creation
- Bulk import
- Review queue
- Analytics dashboard

**Sprint 6 (Week 13): Notifications & Polish**

` `Implement all notification types![ref23]

` `Notification preferences UI![ref24]

` `UI/UX polish (animations, transitions)  Performance optimization![ref22]![ref16]

` `Accessibility improvements![ref17]

**Testing**:

` `Full regression testing![ref24]

` `Load testing (backend performance)  Security audit (basic)![ref22]![ref16]

` `Beta user testing (20-30 parents)![ref17]

**Beta Release**:

` `Deploy to production (soft launch)![ref24]

` `Closed beta group (invite-only)![ref22]

` `Collect structured feedback (surveys)  Monitor analytics and errors![ref16]![ref17]

**Deliverables**:

- Feature-complete V1.0 (minus community features)
- 100+ activities
- Beta testing insights
4. **Phase 3: V1.0 Launch (Week 14-16) - 3 weeks**

**Goal**: Polish & public release **Week 14: QA & Fixes**

` `Address all beta feedback![ref18]

` `Fix critical bugs (P0/P1)![ref19]

` `Performance tuning (optimize slow queries)  Security hardening![ref20]![ref21]

` `Content expansion (target: 150 activities)![ref25]

**Week 15: Launch Prep**

` `App store submissions (metadata, screenshots, video)  Privacy policy & terms of service (legal review)![ref19]![ref20]

` `Help documentation & FAQ![ref21]

` `Onboarding tutorial refinement![ref25]

` `Marketing website (landing page)![ref18]

` `Social media setup (Instagram, Facebook, TikTok)![ref19]

` `Press kit (product description, images, team info)![ref20]

**Week 16: Launch Week**

` `App store approval received![ref25]

` `Final smoke testing on production![ref18]

` `Launch announcement (social media, email)  PR outreach (parenting blogs, media)![ref19]![ref20]

` `Monitor launch (support queries, crash rates)  Hotfix readiness (team on standby)![ref21]![ref25]

**Post-Launch (Weeks 17-18)**:

` `Daily monitoring (analytics, errors, support)![ref19]

` `User feedback collection (in-app, email)![ref20]

` `Prioritize V1.1 backlog![ref21]

` `Retrospective meeting (what went well, what to improve)![ref25]

**Deliverables**:

- Live on App Store & Play Store
- 150+ activities
- Marketing collateral
- Support channel active
- V1.1 roadmap defined
5. **Phase 4: V1.5 - Community Features (Week 19-24) - 6 weeks**

**Goal**: Build community & retention

**Sprint 7 (Week 19-20): Activity Variations**

` `User submission flow (photo + note)  Moderation system (review queue)![ref22]![ref16]

` `Display variations on activity page![ref17]

` `"Helpful" upvote feature![ref23]

**Sprint 8 (Week 21-22): Recipe Exchange**

` `Recipe submission form (cooking activities)  Uwa Farah team review workflow![ref22]![ref16]

` `Recipe display (dedicated tab)![ref17]

` `Dietary filters (vegetarian, halal, etc.)![ref23]

**Sprint 9 (Week 23-24): Play Spots**

` `Location tagging on activity logs![ref22]

` `Play spot creation (crowd-sourced)![ref16]

` `Google Maps integration![ref17]

` `Play spot discovery page (map + list)  Upvote/downvote system![ref23]![ref24]

**Testing & Release**:

` `Community feature testing![ref16]

` `Moderation workflow testing![ref17]

` `Deploy V1.5 to production (phased rollout)![ref23]

**Deliverables**:

- Active community features
- 500+ play spots (target by Month 6)
- User-generated content flowing
6. **Phase 5: V2.0 Planning (Month 7+)**

**Potential Features** (prioritize based on user feedback):

` `Advanced ML recommendations![ref18]

` `Child-facing interface (for older kids)![ref19]

` `Parent groups (local communities)![ref20]

` `In-app messaging (with heavy moderation)![ref21]

` `Virtual workshops/events![ref25]

` `Monetization (premium content, subscription tiers)![ref18]

` `Multi-language support (English, regional languages)![ref19]

` `School/educator partnerships![ref20]

` `Offline mode![ref21]

` `Wearable integration (smart watches for activity tracking)![ref25]![ref26]

6. **Database Schema (Detailed)**

sql![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.052.png)

*-- ==========-- ============================================================================== -- USERS & AUTHENTICA-- USERS & AUTHENTICATIONTION*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE users  users ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `email   email VVARCHARARCHAR((255255)) UNIQUEUNIQUE NOTNOT NULLNULL,,

`  `password\_hash   password\_hash VVARCHARARCHAR((255255)),, *-- nullable for OAuth users-- nullable for OAuth users*   full\_name   full\_name VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `username   username VVARCHARARCHAR((5050)) UNIQUEUNIQUE,, *-- for community featur-- for community featureses*   profile\_photo\_url   profile\_photo\_url TEXTTEXT,,

`  `location\_city   location\_city VVARCHARARCHAR((100100)),,

*-- Gamification-- Gamification*

levellevel INTEGERINTEGER DEFDEFAULAULTT 11,,

`  `experience\_points   experience\_points INTEGERINTEGER DEFDEFAULAULTT 00,,

`  `current\_streak\_days   current\_streak\_days INTEGERINTEGER DEFDEFAULAULTT 00,,   longest\_streak\_days   longest\_streak\_days INTEGERINTEGER DEFDEFAULAULTT 00,,   last\_activity\_logged\_at   last\_activity\_logged\_at TIMESTTIMESTAMPAMP,,

*-- Pr-- Prefereferencesences*

`  `notification\_preferences JSONB   notification\_preferences JSONB DEFDEFAULAULTT '{'{     "scheduled\_reminders": true,    "scheduled\_reminders": true,

`    `"weekly\_digest": true,    "weekly\_digest": true,

`    `"milestone\_celebrations": true,    "milestone\_celebrations": true,

`    `"new\_content\_alerts": true,    "new\_content\_alerts": true,

`    `"engagement\_nudges": false    "engagement\_nudges": false

`  `}'  }',,

*-- OAuth-- OAuth*

`  `google\_id   google\_id VVARCHARARCHAR((255255)) UNIQUEUNIQUE,,   apple\_id   apple\_id VVARCHARARCHAR((255255)) UNIQUEUNIQUE,,

*-- T-- Timestampsimestamps*

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   last\_login\_at   last\_login\_at TIMESTTIMESTAMPAMP,,

*-- Soft delete-- Soft delete*

`  `deleted\_at   deleted\_at TIMESTTIMESTAMPAMP,,

*-- Indexes-- Indexes*

INDEXINDEX idx\_email  idx\_email ((emailemail)),,

INDEXINDEX idx\_username  idx\_username ((usernameusername)),, INDEXINDEX idx\_created\_at  idx\_created\_at ((created\_atcreated\_at))

INDEXINDEX idx\_created\_at  idx\_created\_at ((created\_atcreated\_at))![ref27]

));;

CREACREATETE TTABLEABLE user\_badges  user\_badges ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `user\_id UUID   user\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)) ONON DELETEDELETE CASCADECASCADE,,   badge\_type   badge\_type VVARCHARARCHAR((5050)) NOTNOT NULLNULL,,

`  `earned\_at   earned\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

`  `is\_showcased   is\_showcased BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

UNIQUEUNIQUE((user\_iduser\_id,, badge\_type badge\_type)),, INDEXINDEX idx\_user\_badges  idx\_user\_badges ((user\_iduser\_id)),, INDEXINDEX idx\_badge\_type  idx\_badge\_type ((badge\_typebadge\_type))

));;

*-- ==========-- ============================================================================== -- CHILDREN & PROFILES-- CHILDREN & PROFILES*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE children  children ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `user\_id UUID   user\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)) ONON DELETEDELETE CASCADECASCADE,,   name   name VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `birth\_date   birth\_date DADATETE,, *-- nullable for pr-- nullable for prenatalenatal*

`  `expected\_due\_date   expected\_due\_date DADATETE,, *-- nullable, for pr-- nullable, for prenatalenatal*

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'born''born',, *-- 'expecting' or 'born'-- 'expecting' or 'born'*

`  `profile\_photo\_url   profile\_photo\_url TEXTTEXT,,

`  `gender   gender VVARCHARARCHAR((2020)),, *-- 'male', 'female', '-- 'male', 'female', 'other', 'prother', 'prefer\_not\_to\_say'efer\_not\_to\_say'*

`  `notes   notes TEXTTEXT,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   deleted\_at   deleted\_at TIMESTTIMESTAMPAMP,,

INDEXINDEX idx\_user\_children  idx\_user\_children ((user\_iduser\_id)),, INDEXINDEX idx\_created\_at  idx\_created\_at ((created\_atcreated\_at))

));;

*-- ==========-- ============================================================================== -- CONTENT LIBRAR-- CONTENT LIBRARYY*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE activities  activities ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,   title   title VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `slug   slug VVARCHARARCHAR((255255)) UNIQUEUNIQUE NOTNOT NULLNULL,,

`  `description   description TEXTTEXT NOTNOT NULLNULL,,

`  `description   description  ,,![ref27]

*-- Classification-- Classification*

`  `age\_min\_months   age\_min\_months INTEGERINTEGER NOTNOT NULLNULL DEFDEFAULAULTT 00,, *-- 0 for pr-- 0 for prenatalenatal*

`  `age\_max\_months   age\_max\_months INTEGERINTEGER NOTNOT NULLNULL,,

`  `categories JSONB   categories JSONB NOTNOT NULLNULL,, *-- ["Art", "Cr-- ["Art", "Creativity"]eativity"]*

`  `dif  difficulty ficulty VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'easy''easy',, *-- 'easy', 'm-- 'easy', 'medium', 'challenging'edium', 'challenging'*   estimated\_duration\_minut  estimated\_duration\_minutes es INTEGERINTEGER,,

`  `location\_type   location\_type VVARCHARARCHAR((2020)),, *-- 'indoor', 'outdoor', 'both'-- 'indoor', 'outdoor', 'both'*

*-- Content-- Content*

`  `materials JSONB  materials JSONB,, *-- [{"name": "-- [{"name": "Paper", "quantity": "5 sheets", "is\_common":Paper", "quantity": "5 sheets", "is\_common": true}] true}]*   steps JSONB  steps JSONB,, *-- [{"or-- [{"order": 1, "instruction": "...", "image\_url": "der": 1, "instruction": "...", "image\_url": "..."}]..."}]*

`  `educational\_values JSONB  educational\_values JSONB,, *-- ["Cr-- ["Creativity", "Fine Motor"]eativity", "Fine Motor"]*

`  `parent\_tips   parent\_tips TEXTTEXT,,

`  `conversation\_starters JSONB  conversation\_starters JSONB,, *-- ["What colors do you see?", "H-- ["What colors do you see?", "How does it feel?"]ow does it feel?"]*

`  `safety\_notes   safety\_notes TEXTTEXT,,

*-- Media-- Media*

`  `main\_image\_url   main\_image\_url TEXTTEXT NOTNOT NULLNULL,,

`  `additional\_images JSONB  additional\_images JSONB,, *-- ["url1", "url2"]-- ["url1", "url2"]*   video\_url   video\_url TEXTTEXT,,

*-- Metadata-- Metadata*

`  `created\_by UUID   created\_by UUID REFERENCESREFERENCES users users((idid)),,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'draft''draft',, *-- 'draft', 'pending\_r-- 'draft', 'pending\_review', 'published', 'areview', 'published', 'archived'chived'*

*-- Analytics-- Analytics*

`  `popularity\_score   popularity\_score INTEGERINTEGER DEFDEFAULAULTT 00,,   view\_count   view\_count INTEGERINTEGER DEFDEFAULAULTT 00,,

`  `completion\_count   completion\_count INTEGERINTEGER DEFDEFAULAULTT 00,,   average\_rating   average\_rating DECIMALDECIMAL((33,,22)),,

*-- T-- Timestampsimestamps*

`  `published\_at   published\_at TIMESTTIMESTAMPAMP,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

*-- Indexes-- Indexes*

INDEXINDEX idx\_slug  idx\_slug ((slugslug)),,

INDEXINDEX idx\_age\_range  idx\_age\_range ((age\_min\_monthsage\_min\_months,, age\_max\_months age\_max\_months)),, INDEXINDEX idx\_categories  idx\_categories ((categoriescategories)) USINGUSING GIN GIN,,

INDEXINDEX idx\_status  idx\_status ((statusstatus)),,

INDEXINDEX idx\_published\_at  idx\_published\_at ((published\_atpublished\_at)),,

INDEXINDEX idx\_popularity  idx\_popularity ((popularity\_score popularity\_score DESCDESC))

));;

CREATE TABLE activity\_templates (

CREACREATETE TTABLEABLE activity\_templ activity\_templates ates ((![ref27]

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `name   name VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `category   category VVARCHARARCHAR((5050)),,

`  `template\_structure JSONB   template\_structure JSONB NOTNOT NULLNULL,, *-- Pr-- Pre-defined sectionse-defined sections*   created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP ));;

*-- ==========-- ============================================================================== -- ACTIVITY LOGGING & JOURNALING-- ACTIVITY LOGGING & JOURNALING*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE activity\_logs  activity\_logs ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `child\_id UUID   child\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES children children((idid)) ONON DELETEDELETE CASCADECASCADE,,   activity\_id UUID   activity\_id UUID REFERENCESREFERENCES activities activities((idid)) ONON DELETEDELETE SETSET NULLNULL,,

`  `custom\_activity\_ti  custom\_activity\_title tle VVARCHARARCHAR((255255)),, *-- if activity\_id is nul-- if activity\_id is nulll*

`  `completed\_at   completed\_at TIMESTTIMESTAMPAMP NOTNOT NULLNULL,,

*-- Content-- Content*

`  `photos JSONB  photos JSONB,, *-- [{"url": "s3://...", "caption": "..."-- [{"url": "s3://...", "caption": "...", "or, "order": 1}]der": 1}]*   notes   notes TEXTTEXT,,

*-- 4E Feedback-- 4E Feedback*

`  `feedback\_4e JSONB  feedback\_4e JSONB,, *-- {"enjoy": true, "easy"-- {"enjoy": true, "easy": false, "excellent": true, "earn": false}: false, "excellent": true, "earn": false}*

*-- Additional-- Additional*

`  `duration\_minutes   duration\_minutes INTEGERINTEGER,,

`  `location\_name   location\_name TEXTTEXT,,

`  `location\_spot\_id UUID  location\_spot\_id UUID,, *-- FK to play\_spots (futur-- FK to play\_spots (future)e)*

`  `mood\_tags JSONB  mood\_tags JSONB,, *-- ["happy", "curious", "-- ["happy", "curious", "frustrated"]frustrated"]*   is\_favorite   is\_favorite BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

`  `shared\_as\_variation   shared\_as\_variation BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

*-- Indexes-- Indexes*

INDEXINDEX idx\_child\_logs  idx\_child\_logs ((child\_idchild\_id)),,

INDEXINDEX idx\_activity\_logs  idx\_activity\_logs ((activity\_idactivity\_id)),,

INDEXINDEX idx\_completed\_at  idx\_completed\_at ((completed\_at completed\_at DESCDESC))

));;

CREACREATETE TTABLEABLE scheduled\_activities  scheduled\_activities ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `child\_id UUID   child\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES children children((idid)) ONON DELETEDELETE CASCADECASCADE,,

`  `child\_id UUID   child\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES children children((idid)) ONON DELETEDELETE CASCADECASCADE,,![ref27]

`  `activity\_id UUID   activity\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES activities activities((idid)) ONON DELETEDELETE CASCADECASCADE,,

`  `scheduled\_for   scheduled\_for TIMESTTIMESTAMPAMP NOTNOT NULLNULL,,

`  `reminder\_before\_minutes   reminder\_before\_minutes INTEGERINTEGER DEFDEFAULAULTT 6060,,   reminder\_sent   reminder\_sent BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

`  `notes   notes TEXTTEXT,,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'pending''pending',, *-- 'pending', 'completed', '-- 'pending', 'completed', 'cancelled'cancelled'*   completed\_log\_id UUID   completed\_log\_id UUID REFERENCESREFERENCES activity\_logs activity\_logs((idid)),,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_child\_scheduled  idx\_child\_scheduled ((child\_idchild\_id)),, INDEXINDEX idx\_scheduled\_for  idx\_scheduled\_for ((scheduled\_forscheduled\_for)),, INDEXINDEX idx\_status  idx\_status ((statusstatus))

));;

*-- ==========-- ============================================================================== -- INSIGHTS & ANAL-- INSIGHTS & ANALYTICSYTICS*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE child\_insights  child\_insights ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `child\_id UUID   child\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES children children((idid)) ONON DELETEDELETE CASCADECASCADE,,

`  `insight\_type   insight\_type VVARCHARARCHAR((5050)) NOTNOT NULLNULL,, *-- 'talent\_indicator', 'category\_pr-- 'talent\_indicator', 'category\_prefereference', 'skill\_development'ence', 'skill\_development'*   category   category VVARCHARARCHAR((5050)),, *-- if category-specific-- if category-specific*

`  `message   message TEXTTEXT NOTNOT NULLNULL,,

`  `confidence\_level   confidence\_level VVARCHARARCHAR((2020)),, *-- 'low', 'medium', '-- 'low', 'medium', 'high'high'*

`  `supporting\_data JSONB  supporting\_data JSONB,, *-- {"activities\_count": 15, "enjoy\_rate": 0.93}-- {"activities\_count": 15, "enjoy\_rate": 0.93}*

`  `generated\_at   generated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   is\_viewed   is\_viewed BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_child\_insights  idx\_child\_insights ((child\_idchild\_id)),,

INDEXINDEX idx\_insight\_type  idx\_insight\_type ((insight\_typeinsight\_type)),, INDEXINDEX idx\_generated\_at  idx\_generated\_at ((generated\_at generated\_at DESCDESC))

));;

*-- ==========-- ============================================================================== -- COMMUNITY FEA-- COMMUNITY FEATURESTURES*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE play\_spots  play\_spots ((![ref27]

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `name   name VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

typetype VVARCHARARCHAR((5050)),, *-- 'playgr-- 'playground', 'park', 'indoor\_play', 'library', 'ound', 'park', 'indoor\_play', 'library', 'museum'museum'*   address   address TEXTTEXT,,

`  `latitude   latitude DECIMALDECIMAL((1010,, 88)),,

`  `longitude   longitude DECIMALDECIMAL((1111,, 88)),,

`  `age\_suitability\_mi  age\_suitability\_min n INTEGERINTEGER,,

`  `age\_suitability\_max   age\_suitability\_max INTEGERINTEGER,,

`  `facilities JSONB  facilities JSONB,, *-- ["parking", "r-- ["parking", "restrestroom", "food\_stall"]oom", "food\_stall"]*

`  `photos JSONB  photos JSONB,,   notes   notes TEXTTEXT,,

`  `created\_by UUID   created\_by UUID REFERENCESREFERENCES users users((idid)),,   upvotes   upvotes INTEGERINTEGER DEFDEFAULAULTT 00,,

`  `downvotes   downvotes INTEGERINTEGER DEFDEFAULAULTT 00,,

`  `activity\_count   activity\_count INTEGERINTEGER DEFDEFAULAULTT 00,,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'active''active',, *-- 'active', 'flagged', 'r-- 'active', 'flagged', 'removed'emoved'*

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_location  idx\_location ((latitudelatitude,, longitude longitude)),, INDEXINDEX idx\_type  idx\_type ((typetype)),,

INDEXINDEX idx\_created\_by  idx\_created\_by ((created\_bycreated\_by))

));;

CREACREATETE TTABLEABLE activity\_variations  activity\_variations ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `parent\_activity\_id UUID   parent\_activity\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES activities activities((idid)) ONON DELETEDELETE CASCADECASCADE,,   submitted\_by UUID   submitted\_by UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)),,

`  `variation\_title   variation\_title VVARCHARARCHAR((255255)),,

`  `variation\_notes   variation\_notes TEXTTEXT,, *-- max 500 chars-- max 500 chars*   photo\_url   photo\_url TEXTTEXT,,

`  `helpful\_count   helpful\_count INTEGERINTEGER DEFDEFAULAULTT 00,,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'pending''pending',, *-- 'pending', 'appr-- 'pending', 'approved', 'roved', 'rejected'ejected'*   reviewed\_by UUID  reviewed\_by UUID REFERENCESREFERENCES users users((idid)),,

`  `reviewed\_at   reviewed\_at TIMESTTIMESTAMPAMP,,

`  `review\_notes   review\_notes TEXTTEXT,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,![ref27]

INDEXINDEX idx\_parent\_activity  idx\_parent\_activity ((parent\_activity\_idparent\_activity\_id)),,

INDEXINDEX idx\_status  idx\_status ((statusstatus))

));;

CREACREATETE TTABLEABLE parent\_recipes  parent\_recipes ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `parent\_activity\_id UUID   parent\_activity\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES activities activities((idid)) ONON DELETEDELETE CASCADECASCADE,,   submitted\_by UUID   submitted\_by UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)),,

`  `recipe\_title   recipe\_title VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `ingredients JSONB  ingredients JSONB,, *-- [{"item": "Banana", "quantity": "2"-- [{"item": "Banana", "quantity": "2"}]}]*   steps JSONB  steps JSONB,,

`  `prep\_time\_minutes   prep\_time\_minutes INTEGERINTEGER,,

`  `servings   servings VVARCHARARCHAR((5050)),,

`  `dietary\_tags JSONB  dietary\_tags JSONB,, *-- ["vegetarian", "halal", "nut-fr-- ["vegetarian", "halal", "nut-free"]ee"]*

`  `photo\_url   photo\_url TEXTTEXT,,

`  `notes   notes TEXTTEXT,,

`  `helpful\_count   helpful\_count INTEGERINTEGER DEFDEFAULAULTT 00,,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'pending''pending',,

`  `reviewed\_by UUID  reviewed\_by UUID REFERENCESREFERENCES users users((idid)),,   review\_notes   review\_notes TEXTTEXT,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_parent\_activity  idx\_parent\_activity ((parent\_activity\_idparent\_activity\_id)),,

INDEXINDEX idx\_status  idx\_status ((statusstatus))

));;

CREACREATETE TTABLEABLE parent\_tips  parent\_tips ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,   submitted\_by UUID   submitted\_by UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)),,

`  `category   category VVARCHARARCHAR((5050)),, *-- 'activity\_hacks', 'nutrition', 'sleep', 'books', 'ge-- 'activity\_hacks', 'nutrition', 'sleep', 'books', 'general'neral'*   title   title VVARCHARARCHAR((100100)) NOTNOT NULLNULL,,

`  `content   content TEXTTEXT NOTNOT NULLNULL,, *-- max 1000 chars-- max 1000 chars*

`  `photo\_url   photo\_url TEXTTEXT,,

`  `tags JSONB  tags JSONB,,

`  `helpful\_count   helpful\_count INTEGERINTEGER DEFDEFAULAULTT 00,,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'pending''pending',, *-- 'pending', 'appr-- 'pending', 'approved', 'roved', 'rejected', 'featurejected', 'featured'ed'*   reviewed\_by UUID  reviewed\_by UUID REFERENCESREFERENCES users users((idid)),,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,, ![ref27]  updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_category  idx\_category ((categorycategory)),,

INDEXINDEX idx\_status  idx\_status ((statusstatus)),,

INDEXINDEX idx\_created\_at  idx\_created\_at ((created\_at created\_at DESCDESC))

));;

*-- ==========-- ============================================================================== -- NOTIFICA-- NOTIFICATIONS & ENGAGEMENTTIONS & ENGAGEMENT*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE notifications  notifications ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `user\_id UUID   user\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)) ONON DELETEDELETE CASCADECASCADE,,

typetype VVARCHARARCHAR((5050)) NOTNOT NULLNULL,, *-- 'scheduled\_r-- 'scheduled\_reminder', 'milestone', 'badge\_earned'eminder', 'milestone', 'badge\_earned', etc., etc.*   title   title VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `message   message TEXTTEXT NOTNOT NULLNULL,,

datadata JSONB JSONB,, *-- Context-specific payload-- Context-specific payload*

`  `is\_read   is\_read BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

`  `sent\_at   sent\_at TIMESTTIMESTAMPAMP,,

`  `scheduled\_for   scheduled\_for TIMESTTIMESTAMPAMP,,

`  `delivery\_status   delivery\_status VVARCHARARCHAR((2020)),, *-- 'pending', 'sent', 'failed'-- 'pending', 'sent', 'failed'*

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_user\_notifications  idx\_user\_notifications ((user\_iduser\_id)),, INDEXINDEX idx\_type  idx\_type ((typetype)),,

INDEXINDEX idx\_scheduled\_for  idx\_scheduled\_for ((scheduled\_forscheduled\_for))

));;

CREACREATETE TTABLEABLE push\_notification\_tokens  push\_notification\_tokens ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `user\_id UUID   user\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)) ONON DELETEDELETE CASCADECASCADE,,   device\_token   device\_token TEXTTEXT NOTNOT NULLNULL,,

`  `platform   platform VVARCHARARCHAR((2020)),, *-- 'andr-- 'android', 'ios'oid', 'ios'*

`  `is\_active   is\_active BOOLEANBOOLEAN DEFDEFAULAULTT TRUETRUE,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

UNIQUEUNIQUE((user\_iduser\_id,, device\_token device\_token)),, INDEXINDEX idx\_user\_tokens  idx\_user\_tokens ((user\_iduser\_id))

));;

*-- ==========-- ============================================================================== ![ref27]-- GAMIFICA-- GAMIFICATIONTION*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE challenges  challenges ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,   title   title VVARCHARARCHAR((255255)) NOTNOT NULLNULL,,

`  `description   description TEXTTEXT,,

`  `challenge\_type   challenge\_type VVARCHARARCHAR((5050)),, *-- 'category\_specific', 'diversity', 'consistency', '-- 'category\_specific', 'diversity', 'consistency', 'community'community'*   start\_date   start\_date DADATETE NOTNOT NULLNULL,,

`  `end\_date   end\_date DADATETE NOTNOT NULLNULL,,

`  `goal\_config JSONB  goal\_config JSONB,, *-- {"tar-- {"target\_count": 5, "category": "Outdoor"}get\_count": 5, "category": "Outdoor"}*   reward\_badge\_type   reward\_badge\_type VVARCHARARCHAR((5050)),,

`  `reward\_xp   reward\_xp INTEGERINTEGER,,

`  `is\_active   is\_active BOOLEANBOOLEAN DEFDEFAULAULTT TRUETRUE,,

`  `participant\_count   participant\_count INTEGERINTEGER DEFDEFAULAULTT 00,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_dates  idx\_dates ((start\_datestart\_date,, end\_date end\_date)),, INDEXINDEX idx\_active  idx\_active ((is\_activeis\_active))

));;

CREACREATETE TTABLEABLE challenge\_participants  challenge\_participants ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `challenge\_id UUID   challenge\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES challenges challenges((idid)) ONON DELETEDELETE CASCADECASCADE,,   user\_id UUID   user\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)) ONON DELETEDELETE CASCADECASCADE,,

`  `progress   progress INTEGERINTEGER DEFDEFAULAULTT 00,,

`  `completed   completed BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,   completed\_at   completed\_at TIMESTTIMESTAMPAMP,,

`  `joined\_at   joined\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

`  `updated\_at   updated\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

UNIQUEUNIQUE((challenge\_idchallenge\_id,, user\_id user\_id)),, INDEXINDEX idx\_challenge  idx\_challenge ((challenge\_idchallenge\_id)),, INDEXINDEX idx\_user  idx\_user ((user\_iduser\_id))

));;

CREACREATETE TTABLEABLE child\_milestones  child\_milestones ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,![ref27]

`  `child\_id UUID   child\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES children children((idid)) ONON DELETEDELETE CASCADECASCADE,,

`  `milestone\_type   milestone\_type VVARCHARARCHAR((5050)) NOTNOT NULLNULL,, *-- 'first\_activity', 'ten\_activiti-- 'first\_activity', 'ten\_activities', 'found\_favorite'es', 'found\_favorite'*   category   category VVARCHARARCHAR((5050)),,

`  `achieved\_at   achieved\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   is\_celebrated   is\_celebrated BOOLEANBOOLEAN DEFDEFAULAULTT FFALSEALSE,,

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_child\_mil idx\_child\_milestones estones ((child\_idchild\_id)),,

INDEXINDEX idx\_milestone\_type  idx\_milestone\_type ((milestone\_typemilestone\_type))

));;

*-- ==========-- ============================================================================== -- ADMIN & CONTENT MANAGEMENT-- ADMIN & CONTENT MANAGEMENT*

*-- ==========-- ==============================================================================*

CREACREATETE TTABLEABLE content\_review\_queue  content\_review\_queue ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `content\_type   content\_type VVARCHARARCHAR((5050)) NOTNOT NULLNULL,, *-- 'activity', 'r-- 'activity', 'recipe', 'tip', 'play\_spot'ecipe', 'tip', 'play\_spot'*   content\_id UUID   content\_id UUID NOTNOT NULLNULL,, *-- Polymorphic r-- Polymorphic refereferenceence*

`  `submitted\_by UUID   submitted\_by UUID REFERENCESREFERENCES users users((idid)),,

statusstatus VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'pending''pending',, *-- 'pending', 'in\_r-- 'pending', 'in\_review', 'appreview', 'approved', 'roved', 'rejected'ejected'*

`  `reviewer\_id UUID   reviewer\_id UUID REFERENCESREFERENCES users users((idid)),,

`  `review\_notes   review\_notes TEXTTEXT,,

`  `priority   priority VVARCHARARCHAR((2020)) DEFDEFAULAULTT 'normal''normal',, *-- 'low', 'normal', 'high'-- 'low', 'normal', 'high'*

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,   reviewed\_at   reviewed\_at TIMESTTIMESTAMPAMP,,

INDEXINDEX idx\_status  idx\_status ((statusstatus)),,

INDEXINDEX idx\_content\_type  idx\_content\_type ((content\_typecontent\_type)),, INDEXINDEX idx\_created\_at  idx\_created\_at ((created\_atcreated\_at))

));;

CREACREATETE TTABLEABLE admin\_activity\_l admin\_activity\_log og ((

`  `id UUID   id UUID PRIMARPRIMARYY KEYKEY DEFDEFAULAULTT gen\_random\_uuid gen\_random\_uuid(()),,

`  `admin\_user\_id UUID   admin\_user\_id UUID NOTNOT NULLNULL REFERENCESREFERENCES users users((idid)),,

actionaction VVARCHARARCHAR((100100)) NOTNOT NULLNULL,, *-- 'cr-- 'create\_activity', 'appreate\_activity', 'approve\_content', 'publish\_challenge'ove\_content', 'publish\_challenge'*   tar  target\_type get\_type VVARCHARARCHAR((5050)),,

`  `tar  target\_id UUIDget\_id UUID,,

`  `metadata JSONB  metadata JSONB,,

`  `ip\_address INET  ip\_address INET,,![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.054.png)

`  `created\_at   created\_at TIMESTTIMESTAMPAMP DEFDEFAULAULTT CURRENT\_TIMESTCURRENT\_TIMESTAMPAMP,,

INDEXINDEX idx\_admin  idx\_admin ((admin\_user\_idadmin\_user\_id)),, INDEXINDEX idx\_action  idx\_action ((actionaction)),,

INDEXINDEX idx\_created\_at  idx\_created\_at ((created\_at created\_at DESCDESC))

));;![ref26]

7. **Development Methodology**
1. **Agile Scrum Approach**

**Sprint Duration**: 2 weeks **Team Roles**:

- **Product Owner**: Project lead (defines priorities, accepts stories)
- **Scrum Master**: Technical validator (facilitates, removes blockers)
- **Development Team**: AI + Human validators
- **Stakeholders**: Uwa Farah (content validation), Psikolog team (educational validation)

**Ceremonies**:

- **Sprint Planning** (Monday Week 1, 2 hrs): Select backlog items, define sprint goal
- **Daily Standup** (15 min): What did yesterday, today, blockers (async via Slack if remote)
- **Sprint Review** (Friday Week 2, 1 hr): Demo completed features to stakeholders
- **Sprint Retrospective** (Friday Week 2, 1 hr): What went well, what to improve
2. **AI-Assisted Development Workflow**

**AI Tools**: OpenAI Codex (via GitHub Copilot) + Anthropic Claude **Workflow**:

1. **Task Definition** (Human):
- Write detailed user story with acceptance criteria
- Example: "As a parent, I want to log an activity with photos so that I can preserve memories."
2. **Context Preparation** (Human):
- Gather relevant context (existing code, data models, API contracts)
- Write clear prompt with requirements
3. **Code Generation** (AI):
- Use Copilot in IDE for in-line suggestions
- OR: Paste context + requirements to Claude for full function/component generation
4. **Code Review** (Human):
- Validate logic correctness
- Check edge cases and error handling
- Ensure adherence to coding standards
- Refactor if needed for readability
5. **Testing** (Human + AI):
- AI can generate unit test scaffolds
- Human writes assertions and edge case tests
- Run tests, iterate until passing
6. **Integration** (Human):
- Merge into codebase
- Commit with descriptive message
- Create pull request for team review (if applicable)
7. **Documentation** (Human + AI):
- Add code comments (AI can generate docstrings)
- Update README or technical docs (AI can draft, human refines)

**Best Practices**:

- Start with small, well-defined tasks for AI
- Always validate AI output (don't blindly accept)
- Iterate: If AI output isn't right, refine prompt and retry
- Learn from AI: Understand *why* it wrote code a certain way
- Capture good prompts in a "prompt library" for reuse
3. **Code Quality Standards**

**Linting & Formatting**:

- **Flutter**:  flutter analyze ,  dartfmt
- **Backend**: ESLint + Prettier (TypeScript)
- Pre-commit hooks: Auto-format and lint before commit (using Husky)

**Code Review**:

- All code must be reviewed (even if AI-generated)
- Checklist:

` `Functionality works as expected![ref20]

` `Edge cases handled![ref21]

` `Error handling present![ref25]

` `No security vulnerabilities![ref18]

` `Tests written and passing![ref19]

` `Code is readable and well-commented  Follows project conventions![ref20]![ref21]

**Testing Requirements**:

- **Unit Tests**: All business logic functions (target: 70%+ coverage)
- **Integration Tests**: API endpoints (happy path + error cases)
- **Widget Tests**: Flutter screens with critical interactions
- **E2E Tests**: Key user flows (login → browse → log activity) - optional, but recommended

**Documentation Standards**:

- README in each major directory (purpose, setup instructions)
- API docs: OpenAPI/Swagger spec (auto-generated from code)
- Code comments: Why, not just what (especially for complex logic)
- Changelog: Keep CHANGELOG.md updated with each release
4. **Version Control & Branching**

**Branching Strategy**: Git Flow

**Branches**:

- main : Production-ready code (always deployable)
- develop : Integration branch for features
- feature/\* : Individual features (e.g.,  feature/activity-logging )
- bugfix/\* : Bug fixes
- hotfix/\* : Urgent production fixes

**Workflow**:

1. Create feature branch from  develop
1. Develop feature (commit often with clear messages)
1. Open pull request to  develop
1. Code review + CI checks pass
1. Merge to  develop
1. At sprint end: Merge  develop to  main + tag release (v1.0.0)

**Commit Messages**: Conventional Commits format

feat: add activity scheduling featurefeat: add activity scheduling feature![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.055.png)

fix: resolve photo upload timeout ifix: resolve photo upload timeout issuessue

docs: update API documentation for logging endpointdocs: update API documentation for logging endpoint test: add unit tests for recommendation algoritest: add unit tests for recommendation algorithmthm

5. **Testing Strategy**

**Test Pyramid**:

`       `/\       /\![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.056.png)

`      `/  \  E2E (few)      /  \  E2E (few)      /----\     /----\

`    `/ Integration \    / Integration \

`   `/  (moderate)   \   /  (moderate)   \   /----------  /----------------\------\

` `/   Unit (many)    \ /   Unit (many)    \ /----------/-----------------------------\-\

**Testing Tools**:

- **Flutter**: flutter\_test, mockito (mocking)
- **Backend**: Jest (unit & integration), supertest (HTTP testing)

**Test Coverage Goals**:

- Unit tests: 70%+ coverage (focus on business logic)
- Integration tests: Cover all API endpoints (happy path minimum)
- E2E tests: Cover 3-5 critical user journeys

**Continuous Testing**:

- CI runs all tests on every push
- Pull requests blocked if tests fail
- Weekly coverage report review![ref28]

**8. Content Strategy**

1. **Content Library Target**

**Launch (V1.0)**: 150 activities

- Prenatal: 10 activities (bonding, preparation, wellness)
- 0-1 year: 20 activities (sensory, tummy time, etc.)
- 1-3 years: 25 activities (motor skills, exploration)
- 3-5 years: 30 activities (creativity, pre-literacy)
- 6-8 years: 25 activities (STEM, sports, reading)
- 9-11 years: 20 activities (hobbies, projects)
- 12-15 years: 20 activities (advanced, community service)

**Categories Distribution**:

- Art & Creativity: 25 activities
- Science & Discovery: 20 activities
- Physical & Outdoor: 25 activities
- Literacy & Language: 20 activities
- Music & Rhythm: 15 activities
- Cooking & Nutrition: 15 activities
- Social & Emotional: 15 activities
- Cognitive & Logic: 15 activities
2. **Content Creation Process**

**Roles**:

- **Content Creator**: Uwa Farah's team (5-7 people)
- **Reviewer**: Uwa Farah + 1 senior educator
- **Approver**: Psikolog team (monthly batch review)

**Workflow**:

1. **Ideation** (Weekly meeting): Brainstorm 10-15 activity ideas
1. **Assignment**: Distribute to content creators
1. **Creation** (3-5 days): Use templates in admin panel to draft activities
1. **Internal Review** (2 days): Uwa Farah reviews drafts, provides feedback
1. **Revision** (1 day): Creators address feedback
1. **Approval**: Uwa Farah approves → Status: Published
1. **Monthly Quality Review**: Psikolog team reviews all published content (audit)

**Content Creation Targets**:

- Pre-launch: 150 activities (6 weeks, team of 6 = 4 activities/person/week)
- Post-launch: 8-10 new activities/week (ongoing)
3. **Content Guidelines**

**Activity Design Principles**:

- **Age-appropriate**: Match cognitive and physical capabilities
- **Safe**: Clear safety notes for any risks
- **Accessible**: Use common household materials when possible
- **Engaging**: Fun, not just educational (balance learning and joy)
- **Inclusive**: Adaptable for different abilities and backgrounds
- **Parent-friendly**: Clear instructions, realistic time estimates

**Quality Checklist**:

` `Title is descriptive and engaging![ref21]

` `Description explains what and why (150 chars)  Age range is appropriate![ref25]![ref18]

` `Materials list is complete and specific![ref19]

` `Steps are clear, numbered, and actionable![ref20]

` `Educational value is explicitly stated![ref21]

` `Parent tips provide helpful context![ref25]

` `Photos/videos are high quality and relevant![ref18]

` `Safety notes included if applicable![ref19]

` `No spelling/grammar errors![ref20]

**Content Variety**:

- Mix of activity types: Quick (15min), medium (30-60min), extended (2hr+)
- Mix of difficulty: Easy (minimal prep), Medium (some prep), Challenging (complex)
- Mix of settings: Indoor, outdoor, both
- Mix of seasons: Activities for all weather/seasons
- Cultural relevance: Include Indonesian traditions, holidays, local context
4. **Content Maintenance**

**Quarterly Content Audit**:

- Review activity performance (completion rate, ratings)
- Retire underperforming activities (move to archive, not delete)
- Refresh top performers with new variations
- Update seasonal content (before season starts)

**User Feedback Integration**:

- Monitor activity ratings and user comments
- Surface issues to content team (unclear instructions, safety concerns)
- Iterate activities based on feedback

**Trending Content**:

- Spotlight popular activities in weekly digest
- Create "related activities" based on user completion patterns
- Feature seasonal/holiday activities prominently![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.058.png)
9. **Go-to-Market Strategy**
1. **Target Market Segmentation**

**Primary Market**: Urban Indonesia (Jakarta, Surabaya, Bandung, Medan, Bali)

- Population: ~50 million in target cities
- Smartphone penetration: 70%+
- Target segment: Parents with children 0-15 years (estimated 10 million)

**Initial Target**: "Early Adopters" (Year 1)

- Tech-savvy parents (use multiple apps daily)
- Education-conscious (invest in child development)
- Middle-upper income (can afford activities and smartphone)
- Estimated reach: 50,000 users in first 12 months
2. **Value Proposition**

**For Parents**:

- "One app to track your child's entire journey from pregnancy to teenage years"
- "Never run out of activity ideas - personalized recommendations every day"
- "Discover your child's talents early with AI-powered insights"
- "Preserve precious moments with beautifully organized timelines"
- "Join a community of supportive parents sharing tips and experiences"

**Differentiation** (vs. generic parenting apps):

- **Complete coverage**: Prenatal to teen (most apps focus on 0-5)
- **Curated content**: Expert-validated activities (not just Pinterest reposts)
- **Intelligence**: Talent discovery via 4E framework + pattern recognition
- **Gamification**: Makes parenting engagement fun and rewarding
- **Local**: Indonesian context, language, and community
3. **Launch Strategy**

**Phase 1: Closed Beta (Weeks 14-15)**

- Invite 100 parents (friends, family, parenting groups)
- Goal: Collect feedback, identify bugs, generate early content (user logs)
- Incentive: "Founding Member" badge, lifetime premium (if future paid features)

**Phase 2: Soft Launch (Week 16)**

- Open registration (no invites needed)
- Limited marketing: Social media posts, parenting Facebook groups
- Goal: Validate server load, refine onboarding, build word-of-mouth
- Target: 500 users in first week

**Phase 3: Public Launch (Week 17-18)**

- Press release to parenting media, tech blogs
- App Store / Play Store feature submission (editorial team consideration)
- Social media campaign (#JejakAnakChallenge - share child's first activity)
- Influencer partnerships (parenting bloggers, Instagram moms)
- Goal: 5,000 users in first month

**Phase 4: Growth (Month 2-12)**

- Content marketing: Weekly blog posts, parenting tips
- SEO: Optimize website for "kegiatan anak", "ide bermain anak", etc.
- App store optimization: Keywords, screenshots, reviews
- Referral program: "Invite a friend, both get XP bonus"
- Partnerships: Collaborate with preschools, parenting workshops
- Community events: Monthly virtual parenting Q&A with Uwa Farah
4. **Marketing Channels**

**Digital**:

- **Instagram**: Visual platform (showcase activities with photos)
  - Daily activity ideas
  - Parent testimonials
  - Behind-the-scenes content creation
- **Facebook Groups**: Join/create parenting communities
- **TikTok**: Short-form videos (15-sec activity demos)
- **YouTube**: Long-form content (activity tutorials, parenting tips)
- **Google Ads**: Search campaigns ("aplikasi parenting", "ide main anak")
- **Facebook/Instagram Ads**: Targeted ads (parents aged 25-45, Indonesia)

**Content Marketing**:

- SEO-optimized blog on website
- Guest posts on popular parenting blogs
- Email newsletter (weekly digest to registered users)

**Partnerships**:

- Preschools/kindergartens: Recommend app to parents
- Parenting coaches: Co-branded workshops
- Pediatricians: Referral program (trusted recommendation)
- Brand collaborations: Sponsor activities (e.g., "Activity by [Brand]")

**Community**:

- User-generated content campaigns
- Monthly challenges with prizes (best activity log, most creative variation)
- Feature "Parent of the Month" in app and social media
5. **Monetization Strategy (Future - V2)**

**Freemium Model**:

- **Free Tier** (V1):
  - Unlimited activity logging
  - Access to 80% of activity library
  - Basic recommendations
  - Community features
- **Premium Tier** (V2):
  - Unlock all activities (including exclusive expert content)
  - Advanced AI recommendations
  - Detailed insights & progress reports
  - Ad-free experience
  - Priority support
  - Export timeline as PDF book (print-ready)
  - Pricing: Rp 49,000/month or Rp 399,000/year (~$3-25 USD)

**Other Revenue Streams** (V3+):

- **B2B**: License content to schools/educators
- **Sponsored Activities**: Brands pay to feature activities using their products
- **Events**: Paid virtual workshops with experts
- **Marketplace**: Commission from activity materials sold through partnerships

**Note**: V1.0 is 100% free (no paywalls) to maximize adoption and feedback.![ref26]

10. **Success Metrics & KPIs**
1. **North Star Metric**

**Activities Logged Per Week (Across All Users)**

- Rationale: Core value loop is logging activities. More logs = more engagement = app is useful
- Target: 1,000 activities/week by Month 3, 5,000/week by Month 12
2. **Acquisition Metrics**
- **Downloads**: App Store + Play Store installs
  - Target: 10,000 downloads by Month 3, 75,000 by Month 12
- **Registrations**: Completed signups
  - Target: 60% of downloads convert to registration
- **Onboarding Completion**: Users who add first child profile
  - Target: 80% of registrations complete onboarding
3. **Engagement Metrics**
- **Daily Active Users (DAU)**: Users who open app daily
  - Target: 15% of MAU
- **Monthly Active Users (MAU)**: Users who open app in 30 days
  - Target: 25,000 by Month 12
- **Activities per User per Week**: Average logs per active user
  - Target: 3 activities/user/week
- **Session Duration**: Time spent in app per session
  - Target: 5+ minutes (indicates exploration, not just quick log)
- **Feature Adoption**:
  - % users who schedule activities: Target 40%
  - % users who check insights: Target 60%
  - % users who participate in challenges: Target 25%
4. **Retention Metrics**
- **Day 1 Retention**: % users who return next day
  - Target: 50%
- **Day 7 Retention**: % users who return after 1 week
  - Target: 40%
- **Day 30 Retention**: % users who return after 1 month
  - Target: 35%
- **Churn Rate**: % users who stop using (no activity in 60 days)
  - Target: <5% monthly
5. **Content Metrics**
- **Activity Completion Rate**: % of activities marked as done after viewing
  - Target: 25% (realistic - not all views lead to doing activity)
- **Average Activity Rating**: User satisfaction (future feature)
  - Target: 4.2/5.0
- **Content Freshness**: New activities added per week
  - Target: 8-10/week post-launch
- **Category Coverage**: Activities available per category per age group
  - Target: Min 10 activities per category per age group
6. **Community Metrics**
- **User Contributions**: Variations, recipes, tips, play spots submitted
  - Target: 500 submissions by Month 6
- **Contribution Approval Rate**: % of submissions approved
  - Target: 70% (indicates good community culture)
- **Helpful Votes**: Engagement with community content
  - Target: Avg 10 helpful votes per approved contribution
7. **Quality Metrics**
- **App Crashes**: Crash-free sessions
  - Target: >99.5% (industry standard)
- **API Response Time**: P95 latency
  - Target: <500ms
- **App Store Rating**: Public ratings
  - Target: 4.5+ stars (iOS and Android)
- **Net Promoter Score (NPS)**: Would recommend app?
  - Target: 50+ (good), 70+ (excellent)
8. **Business Metrics (Future)**
- **Cost per Acquisition (CPA)**: Marketing spend / new users
  - Target: <Rp 10,000 per user
- **Customer Lifetime Value (LTV)**: If premium model
  - Target: LTV > 3x CPA
- **Premium Conversion Rate**: % free users who upgrade
  - Target: 5-10% (industry standard for freemium)
9. **Monitoring & Reporting**

**Tools**:

- Firebase Analytics + Google Analytics 4 (user behavior)
- Mixpanel or Amplitude (funnel analysis, retention cohorts)
- Grafana dashboards (real-time tech metrics)
- Weekly automated report (email to team)

**Review Cadence**:

- Daily: Crash rate, critical errors
- Weekly: Engagement metrics, feature adoption
- Monthly: Retention, content performance, NPS
- Quarterly: Strategic review (adjust roadmap based on data)![ref26]
11. **Risk Management**
1. **Technical Risks**

**Risk**: Scalability issues during user growth spike

- **Mitigation**: Load testing before launch, auto-scaling infrastructure (ECS), database query optimization
- **Contingency**: Temporarily throttle new registrations if needed

**Risk**: Data loss or corruption

- **Mitigation**: Automated daily backups (RDS), point-in-time recovery, multi-AZ database
- **Contingency**: Disaster recovery plan documented, regular restore tests

**Risk**: Security breach (unauthorized access to child data)

- **Mitigation**: Security best practices (encryption, auth, input validation), regular security audits, bug bounty program (future)
- **Contingency**: Incident response plan, immediate user notification if breach occurs

**Risk**: Third-party service outage (AWS, FCM)

- **Mitigation**: Multi-region infrastructure (if budget allows), fallback mechanisms (graceful degradation)
- **Contingency**: Status page for users, transparent communication
2. **Product Risks**

**Risk**: Low user adoption (product-market fit not validated)

- **Mitigation**: Extensive prototype testing, beta user feedback, iterate on UX
- **Contingency**: Pivot strategy, re-evaluate value proposition, user interviews

**Risk**: Content quality issues (inaccurate or unsafe activities)

- **Mitigation**: Expert review process, user flagging system, quarterly audits
- **Contingency**: Immediate content removal, publish correction, review process improvement

**Risk**: Poor user retention (users download but don't engage)

- **Mitigation**: Onboarding optimization, push notifications, gamification
- **Contingency**: User surveys (why churning?), feature adjustments, re-engagement campaigns

**Risk**: Community toxicity (inappropriate user-generated content)

- **Mitigation**: Pre-moderation, clear guidelines, report/ban system
- **Contingency**: Increase moderation resources, tighten approval criteria
3. **Team Risks**

**Risk**: AI-generated code contains critical bugs

- **Mitigation**: Mandatory code review, comprehensive testing, human oversight
- **Contingency**: Rollback capability, hotfix process

**Risk**: Content team overwhelmed (can't produce enough activities)

- **Mitigation**: Start with achievable targets, provide efficient tools (templates, bulk import)
- **Contingency**: Hire additional content creators, adjust content cadence (quality over quantity)

**Risk**: Key team member leaves (knowledge loss)

- **Mitigation**: Thorough documentation, knowledge sharing sessions, cross-training
- **Contingency**: Hire replacement quickly, leverage docs to onboard
4. **Legal & Compliance Risks**

**Risk**: Privacy law violations (GDPR, child data protection)

- **Mitigation**: Legal review of privacy policy, implement data controls (export, deletion), minimize data collection
- **Contingency**: Legal counsel on retainer, rapid compliance fixes

**Risk**: Copyright issues (user uploads copyrighted content)

- **Mitigation**: Terms of service (user owns content, grants license), DMCA process
- **Contingency**: Remove infringing content promptly, ban repeat offenders

**Risk**: Liability for activity injuries (child hurt following activity)

- **Mitigation**: Clear disclaimers ("adult supervision required"), safety notes in activities, terms of service (use at own risk)
- **Contingency**: Legal insurance, incident reporting process
5. **Market Risks**

**Risk**: Competitor launches similar app

- **Mitigation**: Move fast, build moat (community, content quality, brand), unique features (4E framework, prenatal support)
- **Contingency**: Differentiate further, emphasize local expertise (Indonesian context)

**Risk**: Market too small (not enough parents want this)

- **Mitigation**: Validate with prototype, beta testing, market research
- **Contingency**: Expand target market (e.g., Southeast Asia), pivot to B2B (sell to schools)![](Aspose.Words.7f61c7c8-dd30-45ba-9eac-972f986c4015.059.png)
12. **Post-Launch Plan**
1. **First 30 Days Post-Launch**

**Week 1**:

- Monitor daily: Crash reports, critical bugs, user support inquiries
- Emergency hotfixes if needed (deploy within 24 hours)
- Social media engagement: Respond to all comments, share user content
- Internal retrospective: What went well in launch, what to improve

**Week 2-3**:

- Analyze onboarding funnel: Where are users dropping off?
- A/B test improvements (e.g., different onboarding copy)
- Collect qualitative feedback: In-app surveys, email to users
- Content sprint: Add 10 more activities based on early requests

**Week 4**:

- First feature update (V1.1 planning based on feedback)
- User appreciation: Feature "User of the Week" in app/social
- Iterate notification strategy (if open rates low)
- Prepare growth experiments (referral incentives, content marketing)
2. **Continuous Improvement Cycle**

**Monthly**:

- Release feature update (new features, improvements, bug fixes)
- Review metrics dashboard (compare to targets, identify trends)
- User feedback synthesis (categorize, prioritize requests)
- Content team workshop (review performance, plan next month's activities)

**Quarterly**:

- Strategic planning session (review OKRs, adjust roadmap)
- Major feature launches (V1.5, V2.0 milestones)
- Team retrospective (process improvements, celebrate wins)
- Financial review (costs, revenue if applicable, budget adjustment)
3. **User Support**

**Channels**:

- **In-App**: Help center with FAQs, contact form
- **Email**: [support@jejakanak.app ](mailto:support@jejakanak.app)(target: <24hr response time)![ref29]![ref30]
- **Social Media**: Instagram/Facebook DMs (daily monitoring)

**Support Tiers**:

- **Tier 1: Self-Service** (80% of queries):
  - Comprehensive FAQ
  - Video tutorials
  - Troubleshooting guides
- **Tier 2: Automated** (15% of queries):
  - Chatbot for common questions (future)
  - Email auto-responder with helpful links
- **Tier 3: Human Support** (5% of queries):
  - Tech team or dedicated support person
  - Response SLA: Critical (4 hrs), High (24 hrs), Normal (48 hrs)

**Escalation**:

- User reports child safety issue → Immediate escalation to senior team + legal review
- User reports bug causing data loss → Immediate escalation to tech lead
4. **Community Management**

**Moderation Team**:

- Start: 1 part-time moderator (Uwa Farah team member)
- Scale: Add moderators as community grows (1 moderator per 5,000 active users)

**Moderation Guidelines**:

- Remove content: Spam, harmful, inappropriate, off-topic
- Warn users: First offense (friendly reminder of guidelines)
- Ban users: Repeat offenders, severe violations (child safety)

**Community Engagement**:

- Highlight great contributions (weekly feature)
- Host virtual events (monthly parenting Q&A)
- Recognize top contributors (badges, special privileges)![ref2]
13. **Conclusion & Next Steps**
1. **Summary**

JejakAnak is positioned to become the leading child development companion app in Indonesia by offering:

- **Comprehensive Coverage**: Prenatal to teenage years (unique in market)
- **Expert-Curated Content**: Quality activities validated by educators and psychologists
- **Intelligent Insights**: Talent discovery through 4E framework and pattern recognition
- **Engaging Experience**: Gamification and community features drive retention
- **Local Relevance**: Indonesian context, language, and community

With a robust technical foundation (Flutter + NestJS + PostgreSQL + AWS), modular architecture for scalability, and AI-assisted development for speed, the team is well-equipped to execute on this vision.

2. **Immediate Next Steps**
1. **Stakeholder Sign-Off** (Day 1):
- Review this masterplan with full team
- Address questions, confirm alignment
- Commit to timeline and resource allocation
2. **Kick Off Phase 0** (Day 2-3):
- Assign roles (who does what)
- Set up project management tools (Notion, Jira, or similar)
- Schedule design sprint (Week 1)
3. **Begin Design Sprint** (Week 1):
- Finalize user stories
- Uwa Farah team: Start ideating seed activities
- Design team (or designer): Begin Figma mockups
4. **Build Prototype** (Week 2-3):
- Develop dummy web app (interactive prototype)
- Parallel: Content team prepares 30 activities in spreadsheet
- Schedule validation sessions with psikolog and parents
5. **Validate & Iterate** (Week 3):
- Conduct user testing
- Refine design based on feedback
- Get final approval to proceed to development
6. **Start Development** (Week 4):
- Initialize GitHub repos
- Set up development environments
- Begin Sprint 1 (Foundation)
3. **Success Criteria for V1.0**

By end of Phase 3 (Week 16), the team will have:

- ![ref15] Fully functional mobile app on iOS and Android
- ![ref15] 150+ curated activities in library
- ![ref15] 1,000+ registered users (beta + soft launch)
- ![ref15] Core features complete (browse, schedule, log, insights, gamification)
- ![ref15] Stable infrastructure (99.5%+ uptime)
- ![ref15] Positive user feedback (NPS > 40)
- ![ref15] Clear roadmap for V1.5 (community features)

If these criteria are met, JejakAnak V1.0 will be a validated product ready for growth and scale.

4. **Long-Term Vision (3-5 Years)**

**Year 1**: Establish product-market fit in Indonesia

- 50,000 active users
- 300+ activities
- Strong community engagement

**Year 2-3**: Scale and monetize

- 250,000+ active users
- Premium tier launch (freemium model)
- Expand to Southeast Asia (Malaysia, Singapore, Philippines)
- B2B partnerships (schools, preschools)

**Year 4-5**: Platform and ecosystem

- 1M+ active users
- Multi-language support (English, Bahasa Melayu, Tagalog)
- Educator marketplace (third-party content creators)
- Hardware integration (smart watches, IoT toys)
- Recognized as the leading parenting platform in region

**Ultimate Goal**: Empower every parent to raise children who reach their full potential, with JejakAnak as their trusted companion from pregnancy through adolescence. Every child deserves to have their unique journey documented, celebrated, and optimized for growth.![ref28]

**Document Version**: 2.0 (Final) **Last Updated**: October 20, 2025 **Owner**: JejakAnak Product Team **Status**: Approved for Development![ref2]

**Appendices**

**Appendix A: Glossary**

- **4E Framework**: Talent assessment method (Enjoy, Easy, Excellent, Earn)
- **Activity Log**: User-generated record of completed activity
- **Activity Variation**: User-submitted modification or alternative approach to official activity
- **Admin Panel**: Web interface for content management
- **Badge**: Achievement reward in gamification system
- **Child Profile**: Data record for one child within parent account
- **DAU/MAU**: Daily/Monthly Active Users
- **Dummy Prototype**: Interactive web prototype for validation
- **ECS**: Elastic Container Service (AWS)
- **FCM**: Firebase Cloud Messaging (push notifications)
- **Gamification**: Game-like elements (XP, badges, streaks) to drive engagement
- **Insight**: AI-generated observation about child's preferences or talents
- **JWT**: JSON Web Token (authentication method)
- **NPS**: Net Promoter Score (customer satisfaction metric)
- **ORM**: Object-Relational Mapping (database abstraction)
- **Play Spot**: User-contributed location for child activities
- **Prenatal**: Period before child birth (pregnancy phase)
- **RDS**: Relational Database Service (AWS managed PostgreSQL)
- **S3**: Simple Storage Service (AWS file storage)
- **Seed Activities**: Initial content populated before launch
- **Streak**: Consecutive days of activity logging

**Appendix B: Contact Information**

- **Product Owner**: [Name] - [email]
- **Technical Lead**: [Name] - [email]
- **Content Validator**: Uwa Farah - [email]
- **Psikolog Team Lead**: [Name] - [email]
- **Support Email**: <support@jejakanak.app>![ref30]![ref29]
- **GitHub**: github.com/jejakanak/app (private repo)
- **Figma Design**: [Link to Figma project]
- **Project Management**: [Link to Notion/Jira]

**Appendix C: References**

1. 4E Talent Framework: [Jejak Anak Kita (JENAKA) methodology]
1. Child Development Guidelines: WHO Child Development Standards
1. Flutter Documentation: flutter.dev
1. NestJS Documentation: nestjs.com
1. PostgreSQL Best Practices: postgresql.org
1. AWS Well-Architected Framework: aws.amazon.com/architecture
1. GDPR Compliance: gdpr.eu
1. App Store Optimization: Apple/Google developer guidelines![ref1]

**END OF MASTERPLAN V2.0**

[]: 

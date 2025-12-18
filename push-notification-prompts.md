# Push Notification & In-App Messaging Prompt Library

## Overview
Character-constrained prompt templates for mobile push notifications and in-app messages. Optimized for immediate action, clarity, and platform-specific limitations.

---

## Character Limits by Platform

| Platform | Title Limit | Body Limit | Total Recommended |
|----------|-------------|------------|-------------------|
| iOS Push | 178 chars | 178 chars | Keep under 150 for preview |
| Android Push | 65 chars | 240 chars | 200 total for readability |
| In-App Message | 50 chars | 150 chars | Scannable in 3 seconds |

---

## 1. Promotional Push Notification

### Purpose
Generate push notifications for time-sensitive offers, sales, or promotions.

### Base Prompt Template
```
You are writing a push notification for {BRAND_NAME} promoting {OFFER_TYPE}.

Offer Details:
- Promotion: {OFFER_DESCRIPTION}
- Value: {DISCOUNT_PERCENTAGE / DOLLAR_AMOUNT / BOGO}
- Urgency: {ENDS_TODAY / ENDS_IN_X_HOURS / LIMITED_QUANTITY}
- Target Segment: {AUDIENCE_DESCRIPTION}

Push Requirements:
- Title: {30-40 characters} - attention-grabbing
- Body: {80-100 characters} - clear value + urgency
- Platform: {iOS / ANDROID / BOTH}
- Tone: {TONE_VALUE}
- Emoji: {SINGLE_RELEVANT_EMOJI / NONE}
- CTA Implication: What happens when they tap

Generate 3 variations: {HIGH_URGENCY / MEDIUM_URGENCY / VALUE_FOCUSED}

Rules:
- No spammy language (avoid ALL CAPS, excessive punctuation)
- Lead with benefit
- Create FOMO without manipulation
- Clear what they get
```

### Example Usage
```
You are writing a push notification for Roasted Beans Coffee promoting flash sale.

Offer Details:
- Promotion: 30% off all whole bean coffee
- Value: 30% discount
- Urgency: Ends in 6 hours
- Target Segment: Customers who purchased whole beans in last 30 days

Push Requirements:
- Title: 30-40 characters - attention-grabbing
- Body: 80-100 characters - clear value + urgency
- Platform: BOTH
- Tone: friendly, urgent
- Emoji: SINGLE_RELEVANT_EMOJI
- CTA Implication: Tap to shop coffee

Generate 3 variations: HIGH_URGENCY / MEDIUM_URGENCY / VALUE_FOCUSED

Rules:
- No spammy language (avoid ALL CAPS, excessive punctuation)
- Lead with benefit
- Create FOMO without manipulation
- Clear what they get
```

---

## 2. Transactional Push Notification

### Purpose
Generate push notifications for order status, delivery updates, or account activity.

### Base Prompt Template
```
You are writing a transactional push notification for {BRAND_NAME}.

Transaction Type: {ORDER_CONFIRMED / OUT_FOR_DELIVERY / DELIVERED / READY_FOR_PICKUP / ACCOUNT_UPDATE}

Details:
- Order/Account Info: {RELEVANT_IDENTIFIER}
- Status: {CURRENT_STATE}
- Next Action: {WHAT_CUSTOMER_SHOULD_DO or WHAT_HAPPENS_NEXT}
- Timing: {EXPECTED_TIMEFRAME if relevant}

Push Requirements:
- Title: {35-45 characters} - clear status update
- Body: {100-120 characters} - next steps or details
- Tone: {professional / friendly / efficient}
- Emoji: {SINGLE_STATUS_EMOJI / NONE}
- Priority: {HIGH / NORMAL}

Generate notification that is:
- Immediately clear about status
- Specific (include order # or tracking)
- Action-oriented if action needed
- Reassuring in tone
```

### Example Usage
```
You are writing a transactional push notification for Green Jay Innovations.

Transaction Type: OUT_FOR_DELIVERY

Details:
- Order Info: Order #GJ-8472
- Status: Package is out for delivery
- Next Action: Will arrive by end of day
- Timing: Expected before 8 PM

Push Requirements:
- Title: 35-45 characters - clear status update
- Body: 100-120 characters - next steps or details
- Tone: friendly
- Emoji: SINGLE_STATUS_EMOJI
- Priority: NORMAL

Generate notification that is:
- Immediately clear about status
- Specific (include order # or tracking)
- Action-oriented if action needed
- Reassuring in tone
```

---

## 3. Re-engagement Push Notification

### Purpose
Generate push notifications to bring back inactive users or encourage app usage.

### Base Prompt Template
```
You are writing a re-engagement push notification for {BRAND_NAME} targeting users who haven't {ACTION} in {TIMEFRAME}.

User Context:
- Inactivity Period: {DAYS/WEEKS_SINCE_LAST_ACTIVITY}
- Last Action: {WHAT_THEY_LAST_DID}
- Value Proposition: {WHY_THEY_SHOULD_RETURN}

Push Requirements:
- Title: {30-40 characters} - personal, welcoming
- Body: {80-100 characters} - value + low pressure
- Tone: {warm / curious / excited}
- Incentive: {DISCOUNT / NEW_FEATURE / CONTENT_UPDATE / NONE}
- Emoji: {SINGLE_WELCOMING_EMOJI / NONE}

Strategy:
{REMIND_OF_VALUE / SHARE_WHAT_THEY_MISSED / OFFER_INCENTIVE / ASK_PREFERENCE}

Generate 3 variations with different approaches:
1. Curiosity-driven
2. Value-reminder
3. Incentive-led (if applicable)

Avoid:
- Guilt or pressure
- "We miss you" clichés
- Desperation
```

---

## 4. Content/Educational Push Notification

### Purpose
Generate push notifications that deliver value through content, tips, or educational information.

### Base Prompt Template
```
You are writing a content push notification for {BRAND_NAME}.

Content Details:
- Type: {BLOG_POST / VIDEO / TIP / GUIDE / ANNOUNCEMENT}
- Topic: {SUBJECT_MATTER}
- Value: {WHAT_THEY'LL_LEARN}
- Relevance: {WHY_IT_MATTERS_TO_THEM}

Push Requirements:
- Title: {35-45 characters} - curiosity or value-driven
- Body: {90-110 characters} - tease benefit
- Tone: {informative / conversational / authoritative}
- Emoji: {RELEVANT_EMOJI / NONE}
- Format: Question or statement

Generate notification that:
- Sparks curiosity without clickbait
- Clearly states value
- Feels helpful, not sales-y
- Encourages tap without pressure
```

### Example Usage
```
You are writing a content push notification for Green Jay Innovations.

Content Details:
- Type: BLOG_POST
- Topic: How Tremella mushrooms compare to hyaluronic acid for hydration
- Value: Learn about natural alternatives to common skincare ingredients
- Relevance: For customers interested in science-backed natural skincare

Push Requirements:
- Title: 35-45 characters - curiosity or value-driven
- Body: 90-110 characters - tease benefit
- Tone: conversational
- Emoji: NONE
- Format: Question

Generate notification that:
- Sparks curiosity without clickbait
- Clearly states value
- Feels helpful, not sales-y
- Encourages tap without pressure
```

---

## 5. Personalized Behavior-Triggered Push

### Purpose
Generate dynamic push notifications based on user behavior, preferences, or milestones.

### Base Prompt Template
```
You are writing a behavior-triggered push notification for {BRAND_NAME}.

Trigger Event:
- Action: {ABANDONED_CART / BROWSED_CATEGORY / WISHLIST_PRICE_DROP / MILESTONE_REACHED}
- User Data: {SPECIFIC_PRODUCT / CATEGORY / ACHIEVEMENT}
- Timing: {HOW_LONG_AFTER_TRIGGER}

Personalization Elements:
- Product/Category: {SPECIFIC_ITEM}
- User Name: {USE_FIRST_NAME / GENERIC}
- Previous Behavior: {CONTEXT_FROM_HISTORY}

Push Requirements:
- Title: {35-45 characters} - personalized, relevant
- Body: {90-120 characters} - specific to trigger
- Tone: {helpful / excited / informative}
- Dynamic Element: {PRODUCT_NAME / PRICE / CATEGORY}
- Emoji: {CONTEXTUAL_EMOJI / NONE}

Generate notification that:
- References specific item/action
- Feels timely and relevant
- Provides clear next step
- Respects privacy (not creepy)
```

### Example Usage - Abandoned Cart
```
You are writing a behavior-triggered push notification for Roasted Beans Coffee.

Trigger Event:
- Action: ABANDONED_CART
- User Data: Left 2 items in cart (Ethiopian whole beans, pour-over dripper)
- Timing: 2 hours after cart abandonment

Personalization Elements:
- Product/Category: Whole bean coffee and brewing equipment
- User Name: GENERIC (no first name available)
- Previous Behavior: Regular purchaser, responds to cart reminders

Push Requirements:
- Title: 35-45 characters - personalized, relevant
- Body: 90-120 characters - specific to trigger
- Tone: helpful
- Dynamic Element: PRODUCT_NAME
- Emoji: NONE

Generate notification that:
- References specific items
- Feels timely and relevant
- Provides clear next step
- Respects privacy (not creepy)
```

---

## 6. In-App Message (Modal/Banner)

### Purpose
Generate in-app messages for feature announcements, onboarding, or contextual guidance.

### Base Prompt Template
```
You are writing an in-app message for {BRAND_NAME}.

Message Type: {MODAL / BANNER / TOOLTIP}
Context: {WHEN_USER_SEES_THIS}

Message Purpose:
- Goal: {INFORM / EDUCATE / GUIDE / ANNOUNCE}
- Topic: {FEATURE / UPDATE / TIP / PROMOTION}
- Action Needed: {YES - what they should do / NO - just informative}

Message Requirements:
- Headline: {25-35 characters} - clear and compelling
- Body: {100-150 characters for modal, 50-70 for banner}
- CTA Button Text: {2-4 words} if action needed
- Dismissible: {YES / NO}
- Tone: {TONE_VALUE}
- Visual Emphasis: {BOLD_KEY_PHRASE / NONE}

Generate message that:
- Interrupts appropriately (valuable, not annoying)
- Clear about what it is
- Easy to act on or dismiss
- Maintains context of user's current task
```

### Example Usage - Feature Announcement
```
You are writing an in-app message for P.B.P.S. Performance System.

Message Type: MODAL
Context: First time user logs in after visual dashboard update

Message Purpose:
- Goal: ANNOUNCE
- Topic: New interactive performance charts
- Action Needed: YES - explore new dashboard

Message Requirements:
- Headline: 25-35 characters - clear and compelling
- Body: 100-150 characters for modal
- CTA Button Text: See My Dashboard
- Dismissible: YES
- Tone: excited, professional
- Visual Emphasis: BOLD_KEY_PHRASE (the word "visual")

Generate message that:
- Interrupts appropriately (valuable, not annoying)
- Clear about what it is
- Easy to act on or dismiss
- Maintains context of user's current task
```

---

## Character Optimization Techniques

### Brevity Without Sacrificing Clarity
1. **Lead with value**: Put benefit first
2. **Active voice**: "Save 30%" not "30% can be saved"
3. **Remove filler**: "Get", "Now", "Just" are often unnecessary
4. **Use numerals**: "3" not "three"
5. **Abbreviate smartly**: "%" vs "percent", "&" vs "and" (when appropriate)

### Testing Variations
Generate 3 versions focusing on different angles:
- **Benefit-first**: What they get
- **Urgency-first**: Time/scarcity element
- **Curiosity-first**: Intriguing question or tease

### Emoji Usage Guidelines
**When to use:**
- Promotional content (🎉 ⚡ 🔥)
- Status updates (✅ 📦 🚚)
- Category signals (🍃 💄 🎮)

**When to avoid:**
- Transactional/serious messages
- Professional/B2B contexts
- When brand voice is formal
- Multiple emojis (never exceed 1)

---

## Urgency Levels

### High Urgency
- Time: Hours remaining
- Language: "Ending soon", "Last chance", "Hurry"
- Use: Flash sales, limited inventory, expiring offers

### Medium Urgency
- Time: Days remaining  
- Language: "Don't miss", "Limited time", "Ends soon"
- Use: Weekend sales, seasonal promotions

### Low Urgency
- Time: Week+ or ongoing
- Language: "Available now", "New", "Check out"
- Use: New arrivals, content, feature announcements

---

## A/B Testing Framework

### Variables to Test
1. **Length**: Short (60 chars) vs. detailed (120 chars)
2. **Emoji**: With vs. without
3. **Tone**: Urgent vs. casual vs. formal
4. **Value placement**: Discount first vs. product first
5. **Question vs. statement**: "Ready to save?" vs. "Save 30% today"

### Metrics to Track
- Open rate
- Click-through rate
- Conversion rate
- Opt-out rate
- Time to action

---

## Compliance & Best Practices

### Respect User Preferences
- Honor quiet hours
- Respect frequency limits
- Allow granular opt-in/opt-out
- Never send misleading content

### Legal Considerations
- No false urgency (fake countdowns)
- Accurate discount claims
- Geographic compliance (GDPR, CCPA)
- Accessibility (screen reader friendly)

### Platform Guidelines
- iOS: Follow Apple's push notification guidelines
- Android: Adhere to material design principles
- Both: Respect battery/data usage

---

## Integration Notes

- See `/email-marketing-prompts.md` for longer-form versions of campaigns
- See `/localization-prompts/` for regional adaptations
- See `/evaluation/push-performance-metrics.md` for testing documentation

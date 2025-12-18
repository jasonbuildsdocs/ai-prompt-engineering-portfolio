# Email Marketing Prompt Library

## Overview
Reusable prompt templates for generating email marketing content across different campaign types, customer segments, and brand voices. Each template includes variable placeholders for dynamic content injection and tone controls.

---

## Template Structure
Each prompt includes:
- **Purpose**: What this template generates
- **Variables**: Dynamic elements to customize
- **Tone Controls**: How to adjust voice
- **Output Specifications**: Length, structure, formatting requirements
- **Example Usage**: Sample with variables filled in

---

## 1. Promotional Campaign Email

### Purpose
Generate promotional emails for sales, discounts, or special offers with urgency and clear CTAs.

### Base Prompt Template
```
You are writing a promotional email for {BRAND_NAME}, a {BRAND_DESCRIPTION}.

Campaign Details:
- Offer: {OFFER_DESCRIPTION}
- Discount/Value: {DISCOUNT_AMOUNT}
- Valid Until: {EXPIRATION_DATE}
- Target Audience: {AUDIENCE_SEGMENT}

Email Requirements:
- Subject Line: Create 3 options (max 50 characters each)
- Preview Text: One compelling line (max 100 characters)
- Body: 150-200 words
- Tone: {TONE: enthusiastic/professional/friendly/urgent}
- Include: Clear CTA button text
- Urgency Level: {LOW/MEDIUM/HIGH}

Brand Voice Guidelines:
{BRAND_VOICE_DESCRIPTION}

Generate the complete email including subject lines, preview text, body copy, and CTA button text.
```

### Example Usage
```
You are writing a promotional email for Green Jay Innovations, a small business specializing in beneficial mushroom-based skincare products.

Campaign Details:
- Offer: Holiday sale on Tremella Facial Serum
- Discount/Value: 25% off + free shipping
- Valid Until: December 24, 2024
- Target Audience: Existing customers who purchased hair products

Email Requirements:
- Subject Line: Create 3 options (max 50 characters each)
- Preview Text: One compelling line (max 100 characters)
- Body: 150-200 words
- Tone: friendly
- Include: Clear CTA button text
- Urgency Level: MEDIUM

Brand Voice Guidelines:
Warm, scientifically-informed, emphasizes natural ingredients and community values. Avoid hype; focus on genuine benefits backed by research.

Generate the complete email including subject lines, preview text, body copy, and CTA button text.
```

---

## 2. Educational/Value-Add Email

### Purpose
Generate educational content that builds trust and authority without direct selling.

### Base Prompt Template
```
You are writing an educational email for {BRAND_NAME} that provides value to subscribers without directly promoting products.

Content Focus:
- Topic: {EDUCATIONAL_TOPIC}
- Key Takeaway: {MAIN_LESSON}
- Related to: {PRODUCT_CATEGORY}
- Audience Knowledge Level: {BEGINNER/INTERMEDIATE/ADVANCED}

Email Requirements:
- Subject Line: Create 3 options (curiosity-driven, max 60 characters)
- Preview Text: Tease the value (max 100 characters)
- Body: 250-300 words
- Tone: {TONE: authoritative/conversational/scientific/casual}
- Include: 2-3 actionable tips
- Soft CTA: {YES/NO} - if yes, link to {CTA_DESTINATION}

Structure:
1. Hook: Relatable problem or question
2. Educational content: 2-3 key points
3. Actionable takeaway
4. Optional soft CTA

Generate the complete email.
```

### Example Usage
```
You are writing an educational email for Green Jay Innovations that provides value to subscribers without directly promoting products.

Content Focus:
- Topic: How mushrooms support skin barrier function
- Key Takeaway: Polysaccharides in mushrooms help retain moisture
- Related to: Skincare serums
- Audience Knowledge Level: BEGINNER

Email Requirements:
- Subject Line: Create 3 options (curiosity-driven, max 60 characters)
- Preview Text: Tease the value (max 100 characters)
- Body: 250-300 words
- Tone: conversational
- Include: 2-3 actionable tips
- Soft CTA: YES - link to blog article on mushroom skincare science

Structure:
1. Hook: Relatable problem or question
2. Educational content: 2-3 key points
3. Actionable takeaway
4. Optional soft CTA

Generate the complete email.
```

---

## 3. Re-engagement/Win-back Email

### Purpose
Generate emails designed to re-activate dormant subscribers or customers.

### Base Prompt Template
```
You are writing a re-engagement email for {BRAND_NAME} targeting subscribers who haven't {ENGAGEMENT_ACTION} in {TIME_PERIOD}.

Customer Context:
- Last Purchase/Interaction: {TIMEFRAME}
- Previous Purchase Category: {PRODUCT_TYPE}
- Account Status: {ACTIVE/LAPSED/DORMANT}

Email Requirements:
- Subject Line: Create 3 options (personal, acknowledges absence, max 50 characters)
- Preview Text: Welcoming, no guilt (max 100 characters)
- Body: 150-200 words
- Tone: {TONE: warm/casual/appreciative/curious}
- Incentive: {INCENTIVE_DESCRIPTION or NONE}
- Include: Low-pressure CTA
- Give unsubscribe option: Acknowledge gracefully

Message Strategy:
{ACKNOWLEDGE_ABSENCE/SHARE_UPDATES/OFFER_INCENTIVE/ASK_PREFERENCES}

Generate the complete email.
```

### Example Usage
```
You are writing a re-engagement email for Roasted Beans Coffee targeting customers who haven't made a purchase in 90+ days.

Customer Context:
- Last Purchase/Interaction: 4 months ago
- Previous Purchase Category: Whole bean coffee and brewing equipment
- Account Status: LAPSED

Email Requirements:
- Subject Line: Create 3 options (personal, acknowledges absence, max 50 characters)
- Preview Text: Welcoming, no guilt (max 100 characters)
- Body: 150-200 words
- Tone: warm
- Incentive: 15% off next purchase
- Include: Low-pressure CTA
- Give unsubscribe option: Acknowledge gracefully

Message Strategy:
SHARE_UPDATES - mention new single-origin arrivals and improved loyalty program

Generate the complete email.
```

---

## 4. Transactional Email (Order Confirmation/Shipping)

### Purpose
Generate transactional emails that confirm actions while reinforcing brand and encouraging next steps.

### Base Prompt Template
```
You are writing a {TRANSACTION_TYPE} email for {BRAND_NAME}.

Transaction Details:
- Type: {ORDER_CONFIRMATION/SHIPPING_NOTIFICATION/DELIVERY_CONFIRMATION}
- Order Number: {ORDER_ID}
- Product(s): {PRODUCT_LIST}
- Next Step: {EXPECTED_DELIVERY/TRACKING_AVAILABLE/READY_FOR_PICKUP}

Email Requirements:
- Subject Line: Clear, functional (max 60 characters)
- Body: 100-150 words
- Tone: {TONE: professional/friendly/efficient}
- Must Include: 
  * Clear transaction details
  * What happens next
  * Support contact info
- Cross-sell Opportunity: {SUBTLE/NONE}

Brand Personality:
{BRIEF_BRAND_VOICE}

Generate the complete email. Prioritize clarity and usefulness while maintaining brand warmth.
```

---

## 5. Milestone/Anniversary Email

### Purpose
Generate personalized emails celebrating customer milestones to build loyalty.

### Base Prompt Template
```
You are writing a milestone celebration email for {BRAND_NAME}.

Milestone Details:
- Type: {FIRST_PURCHASE_ANNIVERSARY/ACCOUNT_BIRTHDAY/LOYALTY_TIER_ACHIEVED/PURCHASE_COUNT_MILESTONE}
- Customer Since: {DATE}
- Total Purchases/Points: {NUMBER}
- Favorite Product Category: {CATEGORY}

Email Requirements:
- Subject Line: Create 3 options (celebratory, personal, max 50 characters)
- Preview Text: Gratitude-focused (max 100 characters)
- Body: 150-200 words
- Tone: {TONE: celebratory/grateful/warm/proud}
- Include: Personalized thank you
- Special Offer: {OFFER_DESCRIPTION or NONE}
- Data Point: Include meaningful stat about their journey

Generate the complete email that feels personal, not automated.
```

---

## Usage Guidelines

### Variable Injection Best Practices
1. **Always populate**: BRAND_NAME, TONE, and output length requirements
2. **Be specific**: Vague variables produce generic output
3. **Test variations**: Try different tone values to find brand fit
4. **Iterate subject lines**: Generate multiple batches if first set doesn't resonate

### Tone Control Values
- **Professional**: Polished, businesslike, credible
- **Friendly**: Approachable, conversational, warm
- **Enthusiastic**: Energetic, excited, bold
- **Urgent**: Time-sensitive, action-oriented, direct
- **Casual**: Relaxed, informal, personal
- **Authoritative**: Expert, confident, informative
- **Empathetic**: Understanding, supportive, caring

### Output Optimization
To improve results:
1. Add brand voice examples in variables
2. Specify what to avoid (e.g., "no corporate jargon")
3. Include competitor differentiation points
4. Reference successful past campaigns
5. Specify reading level if relevant

---

## Localization Notes
These templates support localization through:
- Tone adjustment for cultural context
- Variable injection for regional offers/dates
- Structure flexibility for different communication norms

See `/localization-prompts/` directory for region-specific adaptations of these templates.

---

## A/B Testing Integration
Each template supports A/B testing by:
- Generating multiple subject line options
- Allowing tone variation
- Supporting different CTA approaches
- Enabling urgency level adjustment

Document winning variations in `/evaluation/email-ab-test-results.md`

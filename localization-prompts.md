# Localization & Translation Prompt Library

## Overview
Prompt templates for adapting content across languages, regions, and cultural contexts. Goes beyond word-for-word translation to ensure cultural relevance, tone appropriateness, and market-specific optimization.

---

## Key Localization Principles

1. **Transcreation over Translation**: Recreate intent and impact, not just words
2. **Cultural Context**: Adapt idioms, humor, references to local understanding
3. **Tone Calibration**: Formal vs. casual varies dramatically by culture
4. **Functional Equivalence**: Maintain same effect on target audience as original
5. **Local Optimization**: Consider regional search terms, platforms, regulations

---

## 1. Base Translation with Cultural Adaptation

### Purpose
Translate marketing copy while adapting for cultural resonance and market-specific norms.

### Base Prompt Template
```
You are a localization specialist translating {CONTENT_TYPE} from {SOURCE_LANGUAGE} to {TARGET_LANGUAGE} for {TARGET_MARKET}.

Source Content:
{ORIGINAL_TEXT}

Translation Requirements:
- Target Audience: {DEMOGRAPHIC_DESCRIPTION}
- Tone in Source: {ORIGINAL_TONE}
- Desired Tone in Target: {ADAPTED_TONE - may differ from source}
- Cultural Context: {REGIONAL_CONSIDERATIONS}
- Formality Level: {FORMAL / SEMI-FORMAL / CASUAL / VARIES_BY_CONTEXT}

Localization Priorities:
- Adapt idioms and cultural references to local equivalents
- Maintain brand personality while respecting cultural norms
- Preserve emotional impact and call-to-action strength
- Consider local taboos, sensitivities, and communication preferences
- Optimize for {REGIONAL_PLATFORM if relevant}

Special Considerations:
{BRAND_NAME_HANDLING / CURRENCY / MEASUREMENTS / DATE_FORMAT / LEGAL_REQUIREMENTS}

Generate translation that feels native to {TARGET_MARKET}, not like translated content.
```

### Example Usage - English to Spanish (Spain vs. Latin America)
```
You are a localization specialist translating promotional email from English to Spanish for Spain market.

Source Content:
"Get ready to glow! Our new Tremella serum drops this Friday. Early birds save 20%. Your skin will thank you 🌟"

Translation Requirements:
- Target Audience: Spanish women 25-45, skincare enthusiasts
- Tone in Source: Enthusiastic, playful, beauty-industry casual
- Desired Tone in Target: Warm but slightly more refined (Spain market tends more formal than US)
- Cultural Context: Spain beauty market values efficacy and elegance over hype
- Formality Level: SEMI-FORMAL

Localization Priorities:
- Adapt idioms and cultural references to local equivalents
- Maintain brand personality while respecting cultural norms
- Preserve emotional impact and call-to-action strength
- Consider local taboos, sensitivities, and communication preferences
- Optimize for email platform

Special Considerations:
- Use "%" symbol (universal)
- Use European date format (Friday → viernes)
- Adapt "early bird" idiom (not direct equivalent in Spanish)
- Consider vosotros vs. ustedes (use ustedes for marketing in Spain)
- Emoji usage: maintain but ensure culturally appropriate

Generate translation that feels native to Spain market, not like translated content.
```

### Same Content, Different Spanish Market
```
You are a localization specialist translating promotional email from English to Spanish for Mexico market.

Source Content:
"Get ready to glow! Our new Tremella serum drops this Friday. Early birds save 20%. Your skin will thank you 🌟"

Translation Requirements:
- Target Audience: Mexican women 25-45, skincare enthusiasts
- Tone in Source: Enthusiastic, playful, beauty-industry casual
- Desired Tone in Target: Maintain enthusiastic, warm, approachable tone (Mexican market embraces this)
- Cultural Context: Mexican beauty market responds well to relational, warm marketing
- Formality Level: CASUAL (tú form appropriate)

Localization Priorities:
- Adapt idioms and cultural references to local equivalents
- Maintain brand personality while respecting cultural norms
- Preserve emotional impact and call-to-action strength  
- Consider local taboos, sensitivities, and communication preferences
- Optimize for email platform

Special Considerations:
- Use "%" symbol (universal)
- Use local date reference (este viernes)
- Adapt "early bird" to Mexican equivalent expression
- Use "tú" form (more appropriate for Mexican consumer marketing)
- Emoji usage: maintain and embrace (Mexican market very emoji-friendly)

Generate translation that feels native to Mexico market, not like translated content.
```

---

## 2. Tone Calibration by Region

### Purpose
Adapt the same message with different tonal approaches for different cultural markets.

### Base Prompt Template
```
You are adapting {CONTENT_TYPE} for {TARGET_MARKET} with appropriate cultural tone.

Core Message (Language-Neutral):
{MAIN_POINT_TO_COMMUNICATE}

Regional Tone Guidelines for {TARGET_MARKET}:
- Communication Style: {DIRECT / INDIRECT / RELATIONSHIP_FIRST}
- Hierarchy/Formality: {HIGH / MODERATE / LOW}
- Persuasion Approach: {LOGICAL / EMOTIONAL / STATUS_BASED / COMMUNITY_BASED}
- Urgency Expression: {EXPLICIT / SUBTLE / MODERATE}
- Individualism vs. Collectivism: {INDIVIDUAL_FOCUS / GROUP_FOCUS}

Content Requirements:
- Language: {TARGET_LANGUAGE}
- Length: {WORD_COUNT}
- Format: {EMAIL / SOCIAL_POST / PRODUCT_DESCRIPTION}

Generate content that:
- Communicates the core message effectively
- Feels natural to {TARGET_MARKET} audience
- Respects cultural communication norms
- Maintains brand integrity while adapting to local preferences
```

### Example Usage - Product Launch Announcement Across Cultures

**For US Market (Direct, Individual, Casual)**
```
You are adapting product launch announcement for United States market with appropriate cultural tone.

Core Message:
New performance tracking system helps sales teams increase revenue through transparent metrics and fair incentives.

Regional Tone Guidelines for United States:
- Communication Style: DIRECT
- Hierarchy/Formality: LOW (first-name basis, conversational)
- Persuasion Approach: LOGICAL + benefits to individual
- Urgency Expression: EXPLICIT (clear deadlines, direct CTAs)
- Individualism vs. Collectivism: INDIVIDUAL_FOCUS (your success, your performance)

Content Requirements:
- Language: English
- Length: 150 words
- Format: EMAIL announcement to potential customers

Generate content that:
- Communicates the core message effectively
- Feels natural to US business audience
- Respects cultural communication norms (direct value prop, ROI-focused)
- Maintains brand integrity while adapting to local preferences
```

**For Japan Market (Indirect, Group, Formal)**
```
You are adapting product launch announcement for Japan market with appropriate cultural tone.

Core Message:
New performance tracking system helps sales teams increase revenue through transparent metrics and fair incentives.

Regional Tone Guidelines for Japan:
- Communication Style: INDIRECT (build context, avoid blunt statements)
- Hierarchy/Formality: HIGH (respectful language, proper titles)
- Persuasion Approach: RELATIONSHIP_FIRST + group harmony
- Urgency Expression: SUBTLE (avoid aggressive pressure)
- Individualism vs. Collectivism: GROUP_FOCUS (team success, organizational benefit)

Content Requirements:
- Language: Japanese
- Length: 150 words
- Format: EMAIL announcement to potential customers

Generate content that:
- Communicates the core message effectively
- Feels natural to Japanese business audience
- Respects cultural communication norms (indirect approach, relationship building)
- Maintains brand integrity while adapting to local preferences
- Uses appropriate keigo (respectful language) level
```

---

## 3. Regional Platform Optimization

### Purpose
Adapt content for region-specific dominant platforms and their communication styles.

### Base Prompt Template
```
You are adapting {CONTENT_TYPE} for {PLATFORM} in {TARGET_MARKET}.

Content Purpose: {CAMPAIGN_GOAL}
Source Content: {ORIGINAL_MESSAGE}

Platform Context for {TARGET_MARKET}:
- Primary Platform: {PLATFORM_NAME}
- Usage Pattern: {HOW_THIS_DEMOGRAPHIC_USES_IT}
- Content Style Norms: {PLATFORM_SPECIFIC_CONVENTIONS}
- Character/Length Limits: {CONSTRAINTS}
- Visual Expectations: {IMAGE/VIDEO/TEXT_FOCUS}

Regional Platform Notes:
{MARKET_SPECIFIC_PLATFORM_BEHAVIORS}

Generate content optimized for:
- Platform format and best practices
- Regional usage patterns
- Local engagement drivers
- Cultural content preferences
```

### Example Usage - LinkedIn vs. WhatsApp Business in Different Markets

**LinkedIn Post - Germany (Professional, Detailed)**
```
You are adapting product announcement for LinkedIn in Germany market.

Content Purpose: Announce new P.B.P.S. performance tracking software
Source Content: "Revolutionary performance tracking for retail teams"

Platform Context for Germany:
- Primary Platform: LinkedIn (dominant professional network)
- Usage Pattern: Professional development, industry insights, thought leadership
- Content Style Norms: Substantive, data-driven, avoid excessive hype
- Character/Length Limits: Optimal 150-250 words for engagement
- Visual Expectations: Professional charts/graphs valued

Regional Platform Notes:
German LinkedIn users expect: detailed information, credibility markers (qualifications, data), formal tone, practical applications, less personal storytelling than US market

Generate content optimized for:
- Platform format and best practices
- Regional usage patterns (German professionals value thoroughness)
- Local engagement drivers (data, credentials, practical ROI)
- Cultural content preferences (formal, detailed, substantiated claims)
```

**WhatsApp Business Message - Brazil (Casual, Relational)**
```
You are adapting product announcement for WhatsApp Business in Brazil market.

Content Purpose: Announce new P.B.P.S. performance tracking software
Source Content: "Revolutionary performance tracking for retail teams"

Platform Context for Brazil:
- Primary Platform: WhatsApp Business (dominant business communication)
- Usage Pattern: Direct conversations, relationship-building, quick exchanges
- Content Style Norms: Warm, conversational, emoji-friendly, brief
- Character/Length Limits: 100-150 chars for initial message, conversation-style
- Visual Expectations: Friendly images, short videos

Regional Platform Notes:
Brazilian WhatsApp Business users expect: warm greetings, relationship language, conversational tone, emojis appropriate, voice messages common, less formal than email

Generate content optimized for:
- Platform format and best practices (conversational, not broadcast-y)
- Regional usage patterns (Brazilian business relationships are warm)
- Local engagement drivers (trust, personal connection, accessibility)
- Cultural content preferences (friendly, approachable, human)
```

---

## 4. Idiom and Metaphor Localization

### Purpose
Identify and replace idioms, metaphors, and cultural references with local equivalents.

### Base Prompt Template
```
You are localizing content containing idioms and cultural references from {SOURCE_LANGUAGE}/{SOURCE_CULTURE} to {TARGET_LANGUAGE}/{TARGET_CULTURE}.

Source Content:
{TEXT_WITH_IDIOMS}

Identified Cultural Elements:
{LIST_IDIOMS_METAPHORS_REFERENCES}

Localization Approach:
- Find functional equivalents (same meaning/impact in target culture)
- If no equivalent exists, adapt the underlying concept
- Maintain emotional resonance and tone
- Preserve humor if present (adapt style as needed)
- Consider target market familiarity with source culture

Generate localized version where:
- Idioms are replaced with natural target language equivalents
- Cultural references land with target audience
- Tone and impact match original
- Content feels native, not translated
```

### Example Usage
```
You are localizing content containing idioms and cultural references from English/US to German/Germany.

Source Content:
"Don't put all your eggs in one basket with your marketing strategy. Hit a home run by diversifying across channels. Our platform helps you cover all your bases."

Identified Cultural Elements:
- "Don't put all your eggs in one basket" (risk management idiom)
- "Hit a home run" (baseball metaphor for big success)
- "Cover all your bases" (baseball metaphor for comprehensive coverage)

Localization Approach:
- Find functional equivalents (same meaning/impact in German culture)
- If no equivalent exists, adapt the underlying concept
- Maintain emotional resonance and tone (professional, advisory)
- Preserve advice-giving tone
- Consider German audience has limited baseball familiarity

Generate localized version where:
- Idioms are replaced with natural German equivalents
- Cultural references land with German business audience (soccer or non-sport metaphors more appropriate)
- Tone and impact match original (professional advisory)
- Content feels native, not translated
```

---

## 5. Currency, Date, and Measurement Localization

### Purpose
Automatically adapt numerical and formatting conventions to target market standards.

### Base Prompt Template
```
You are adapting content with numerical and formatting elements from {SOURCE_MARKET} to {TARGET_MARKET}.

Source Content:
{CONTENT_WITH_NUMBERS_DATES_MEASUREMENTS}

Localization Requirements:
- Currency: Convert {SOURCE_CURRENCY} to {TARGET_CURRENCY} or express appropriately
- Date Format: Adapt from {SOURCE_FORMAT} to {TARGET_FORMAT}
- Number Format: Adapt decimal/thousand separators
- Measurements: Convert {IMPERIAL/METRIC} as needed
- Time Zone: Adjust if relevant
- Phone Numbers: Format per local convention

Conversion Notes:
- Use current exchange rates or express in local currency equivalent
- Adapt dates to local reading order (DD/MM vs MM/DD)
- Honor local comma/period usage in numbers
- Convert units precisely (inches to cm, etc.)

Generate content with all numerical elements properly localized.
```

---

## 6. Legal and Regulatory Compliance by Region

### Purpose
Ensure localized content meets regional legal requirements and marketing regulations.

### Base Prompt Template
```
You are adapting {CONTENT_TYPE} for {TARGET_MARKET} ensuring regulatory compliance.

Source Content:
{ORIGINAL_CONTENT}

Regional Requirements for {TARGET_MARKET}:
- Required Disclosures: {LEGAL_DISCLAIMERS}
- Prohibited Claims: {WHAT_CANNOT_BE_STATED}
- Mandatory Language: {REQUIRED_PHRASES}
- Data Privacy: {GDPR / CCPA / OTHER_REQUIREMENTS}
- Industry-Specific Rules: {HEALTHCARE / FINANCE / CANNABIS / OTHER}

Content Type Regulations:
{SPECIFIC_RULES_FOR_EMAIL / SMS / SOCIAL / ADS}

Generate compliant content that:
- Includes all required disclosures
- Avoids prohibited language
- Meets formatting requirements
- Maintains marketing effectiveness within constraints
- Feels natural despite legal requirements
```

### Example Usage - Cannabis Marketing (Strict Regional Variance)
```
You are adapting promotional email for Colorado market ensuring regulatory compliance.

Source Content:
"Amazing deals on premium flower! Get high-quality products delivered to your door today."

Regional Requirements for Colorado:
- Required Disclosures: "Must be 21+ with valid ID", "This product contains marijuana"
- Prohibited Claims: Cannot use "high" as verb related to effects, cannot guarantee delivery timing
- Mandatory Language: License number must appear, cannot appeal to minors
- Data Privacy: Standard CAN-SPAM compliance
- Industry-Specific Rules: Cannot advertise outside state, no health claims, no visible consumption encouragement

Content Type Regulations:
Email marketing must include: age gate reminder, license #, cannot use packaging or imagery that appeals to minors

Generate compliant content that:
- Includes all required disclosures (21+, marijuana content, license #)
- Avoids prohibited language ("get high" → "get quality")
- Meets formatting requirements
- Maintains marketing effectiveness within constraints (still compelling despite restrictions)
- Feels natural despite legal requirements (not overly legalistic in tone)
```

---

## Regional Tone Matrix

Quick reference for baseline tone expectations by market:

| Market | Formality | Directness | Individualism | Humor | Emoji Use |
|--------|-----------|------------|---------------|-------|-----------|
| USA | Low-Med | High | High | Casual OK | Moderate |
| UK | Medium | High | High | Dry/Ironic | Low-Mod |
| Germany | Med-High | High | Medium | Reserved | Low |
| France | Medium | Medium | Medium | Sophisticated | Low |
| Japan | High | Low | Low | Rare/Subtle | Context-dependent |
| Brazil | Low-Med | Medium | Low-Med | Welcomed | High |
| Mexico | Low-Med | Medium | Low-Med | Welcomed | High |
| Spain | Medium | Medium | Medium | Moderate | Moderate |
| India | Med-High | Medium | Low | Situational | Moderate |
| China | Med-High | Low | Low | Subtle | Platform-dependent |

*Note: These are generalizations. Always research specific audience segments.*

---

## Quality Assurance Checklist

Before finalizing localized content:

- [ ] Native speaker review (ideally in-market)
- [ ] Cultural references appropriate and understood
- [ ] Tone matches regional communication norms
- [ ] Idioms naturally adapted, not literally translated
- [ ] Numbers, dates, currency properly formatted
- [ ] Legal requirements met for target market
- [ ] Brand voice preserved despite adaptations
- [ ] No unintentional offensive language or imagery
- [ ] Platform-specific formats respected
- [ ] SEO keywords adapted for local search behavior

---

## Integration Notes

- Use these prompts in combination with `/email-marketing-prompts.md` and `/product-copy-prompts.md`
- Document successful localizations in `/evaluation/localization-performance.md`
- Maintain glossary of approved translations for brand terms
- Test localized content with in-market focus groups when possible

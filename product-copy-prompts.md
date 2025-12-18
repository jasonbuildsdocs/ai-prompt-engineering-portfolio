# Product Copy Prompt Library

## Overview
Reusable prompt templates for generating product descriptions, feature explanations, and marketing copy. Designed for scalability across product catalogs with consistent voice and structure.

---

## 1. Short-Form Product Description (E-commerce)

### Purpose
Generate concise, scannable product descriptions for e-commerce listings (marketplace, PDP snippets, cards).

### Base Prompt Template
```
You are writing a short-form product description for {PRODUCT_NAME}.

Product Information:
- Category: {PRODUCT_CATEGORY}
- Key Features: {LIST_3-5_FEATURES}
- Primary Benefit: {MAIN_CUSTOMER_BENEFIT}
- Target User: {USER_PERSONA}
- Price Point: {BUDGET/MID/PREMIUM}

Copy Requirements:
- Length: {50-75 words / 75-100 words / 100-150 words}
- Format: {PARAGRAPH / BULLET_POINTS / HYBRID}
- Tone: {TONE_VALUE}
- Lead with: {BENEFIT/FEATURE/PROBLEM_SOLUTION}
- Include: {SPECIFICATIONS/MATERIALS/DIMENSIONS} if relevant
- SEO Keywords: {KEYWORD_LIST}

Brand Guidelines:
{BRAND_VOICE_DESCRIPTION}

Generate product description optimized for {PLATFORM: website/Amazon/marketplace}.
```

### Example Usage
```
You are writing a short-form product description for Tremella Mushroom Facial Serum.

Product Information:
- Category: Natural skincare, anti-aging serum
- Key Features: Tremella mushroom extract, hyaluronic acid, vitamin C, lightweight formula, non-greasy
- Primary Benefit: Intense hydration that plumps and smooths skin
- Target User: Women 30-50 concerned about fine lines and dryness
- Price Point: MID

Copy Requirements:
- Length: 75-100 words
- Format: PARAGRAPH
- Tone: warm, scientific
- Lead with: BENEFIT
- Include: Key active ingredients
- SEO Keywords: mushroom serum, natural anti-aging, hydrating serum, tremella extract

Brand Guidelines:
Research-backed, natural, avoids beauty industry hype. Emphasizes real benefits supported by science.

Generate product description optimized for website.
```

---

## 2. Long-Form Product Description (Detailed PDP)

### Purpose
Generate comprehensive product descriptions for main product detail pages with storytelling and depth.

### Base Prompt Template
```
You are writing a detailed product description for {PRODUCT_NAME}.

Product Context:
- Full Name: {PRODUCT_FULL_NAME}
- Category: {CATEGORY}
- Problem It Solves: {CUSTOMER_PAIN_POINT}
- How It Works: {MECHANISM_EXPLANATION}
- Key Ingredients/Components: {DETAILED_LIST}
- Unique Selling Proposition: {WHAT_MAKES_IT_DIFFERENT}
- Target Customer: {DETAILED_PERSONA}

Copy Requirements:
- Length: 300-400 words
- Structure:
  1. Opening hook (problem or aspiration)
  2. Solution introduction (what it is)
  3. How it works (mechanism/features)
  4. Benefits breakdown
  5. Why choose this (differentiation)
  6. Usage/application details
- Tone: {TONE_VALUE}
- Reading Level: {GENERAL_AUDIENCE/TECHNICAL/SIMPLIFIED}
- Include Sections: {YES/NO for each - Science Behind It / Usage Instructions / Who It's For}

Brand Story Elements:
{ORIGIN_STORY / SOURCING / PHILOSOPHY}

Generate complete product description with clear section breaks.
```

### Example Usage
```
You are writing a detailed product description for Performance Based Points System (Internal Sales Tool).

Product Context:
- Full Name: Strawberry Fields Performance Based Points System (P.B.P.S.)
- Category: Sales performance tracking and incentive software
- Problem It Solves: Lack of visibility into individual performance and inconsistent motivation across sales team
- How It Works: Tracks key metrics (avg ticket, add-on rate, discounts) and awards points that translate to tiered bonuses
- Key Components: Automated data tracking, weekly performance recaps, monthly leaderboards, visual dashboards, transparent point calculation
- Unique Selling Proposition: Combines accountability with motivation through data transparency and fair reward structure
- Target Customer: Retail managers seeking to improve team performance and sales trainers needing objective metrics

Copy Requirements:
- Length: 300-400 words
- Structure:
  1. Opening hook (problem or aspiration)
  2. Solution introduction (what it is)
  3. How it works (mechanism/features)
  4. Benefits breakdown
  5. Why choose this (differentiation)
  6. Usage/application details
- Tone: professional, motivating
- Reading Level: GENERAL_AUDIENCE
- Include Sections: YES for How It Works / YES for Who It's For

Brand Story Elements:
Created in response to declining sales and need for objective performance measurement. Built by sales trainer who understood both data and human motivation.

Generate complete product description with clear section breaks.
```

---

## 3. Feature-Focused Copy

### Purpose
Generate copy that explains specific product features, ideal for comparison tables, feature callouts, or spec sheets.

### Base Prompt Template
```
You are writing feature-focused copy for {FEATURE_NAME} in {PRODUCT_NAME}.

Feature Details:
- Feature: {FEATURE_NAME}
- What It Does: {TECHNICAL_DESCRIPTION}
- Customer Benefit: {WHY_IT_MATTERS}
- How It's Different: {COMPARED_TO_ALTERNATIVES}
- Use Case: {WHEN_CUSTOMER_NEEDS_IT}

Copy Requirements:
- Format: {HEADLINE + 2-3 SENTENCES / BULLET_POINTS / CALLOUT_BOX}
- Length: {50 / 100 / 150 words}
- Tone: {TONE_VALUE}
- Technical Depth: {HIGH/MEDIUM/LOW}
- Comparison: {INCLUDE/EXCLUDE competitive comparison}

Generate feature copy that is:
- Clear about what it does
- Focused on customer benefit
- Easy to scan
- Persuasive without overselling
```

### Example Usage
```
You are writing feature-focused copy for Visual Performance Dashboards in P.B.P.S. Performance Tracking System.

Feature Details:
- Feature: Interactive Line Chart Performance Tracking
- What It Does: Displays each team member's metrics over time in visual graphs with trend lines
- Customer Benefit: Instant visibility into performance patterns, easy to spot improvement or decline
- How It's Different: Most systems only show static numbers; this shows trajectory and momentum
- Use Case: Weekly team meetings, monthly reviews, self-monitoring by employees

Copy Requirements:
- Format: HEADLINE + 2-3 SENTENCES
- Length: 100 words
- Tone: professional, clear
- Technical Depth: LOW
- Comparison: INCLUDE competitive comparison

Generate feature copy that is:
- Clear about what it does
- Focused on customer benefit
- Easy to scan
- Persuasive without overselling
```

---

## 4. Benefits-Driven Copy

### Purpose
Generate copy focused on customer outcomes rather than product features, ideal for landing pages and ads.

### Base Prompt Template
```
You are writing benefits-driven copy for {PRODUCT_NAME}.

Customer Context:
- Before State: {CUSTOMER_PAIN_POINT / CURRENT_SITUATION}
- After State: {DESIRED_OUTCOME}
- Emotional Motivation: {WHAT_THEY_REALLY_WANT}
- Practical Motivation: {TANGIBLE_RESULT}

Product Connection:
- Primary Benefit: {MAIN_OUTCOME}
- Secondary Benefits: {2-3_SUPPORTING_OUTCOMES}
- Proof Points: {STATS / TESTIMONIALS / GUARANTEES}

Copy Requirements:
- Format: {PAS_FRAMEWORK / BEFORE_AFTER_BRIDGE / FEATURE_ADVANTAGE_BENEFIT}
- Length: 150-200 words
- Tone: {TONE_VALUE}
- Angle: {ASPIRATIONAL / PROBLEM_SOLVING / TRANSFORMATIONAL}
- Include: Social proof or credibility markers

Generate copy that focuses on the customer's transformation, not product features.
```

### Frameworks Explained

**PAS (Problem-Agitate-Solution)**
1. State the problem
2. Amplify the pain or frustration
3. Present solution

**Before-After-Bridge**
1. Describe current problematic state
2. Paint picture of ideal state
3. Show how product bridges the gap

**Feature-Advantage-Benefit (FAB)**
1. State feature
2. Explain advantage
3. Connect to meaningful benefit

### Example Usage
```
You are writing benefits-driven copy for Green Jay Innovations Hair Regrowth Serum.

Customer Context:
- Before State: Noticing thinning hair, trying products that don't work, feeling self-conscious
- After State: Visible regrowth, confidence restored, natural solution that works
- Emotional Motivation: Feel attractive and confident again
- Practical Motivation: Measurable hair density improvement

Product Connection:
- Primary Benefit: Clinically-studied ingredients stimulate follicles for visible regrowth
- Secondary Benefits: Natural formula, no harsh chemicals, works with body's biology, affordable alternative to expensive treatments
- Proof Points: Backed by NCBI studies on mushroom polysaccharides

Copy Requirements:
- Format: BEFORE_AFTER_BRIDGE
- Length: 150-200 words
- Tone: empathetic, hopeful, scientific
- Angle: TRANSFORMATIONAL
- Include: Research credibility

Generate copy that focuses on the customer's transformation, not product features.
```

---

## 5. Technical Specifications Copy

### Purpose
Generate clear, accurate technical specifications that are informative without overwhelming non-technical readers.

### Base Prompt Template
```
You are writing technical specifications copy for {PRODUCT_NAME}.

Specifications:
- Dimensions/Size: {MEASUREMENTS}
- Materials/Ingredients: {COMPLETE_LIST}
- Technical Details: {SPECS_LIST}
- Compatibility: {WHAT_IT_WORKS_WITH}
- Certifications: {SAFETY/QUALITY_MARKS}

Copy Requirements:
- Format: {TABLE / BULLETED_LIST / CATEGORIZED_SECTIONS}
- Include Explanations: {YES/NO} - if yes, add brief clarifications for complex terms
- Tone: {factual / accessible / technical}
- Highlight: {STANDOUT_SPECS_TO_EMPHASIZE}
- Compare To: {STANDARD/COMPETITOR if relevant}

Audience Knowledge: {EXPERT / INFORMED_CONSUMER / GENERAL_PUBLIC}

Generate specifications that are accurate, scannable, and appropriate for audience knowledge level.
```

---

## 6. SEO-Optimized Product Copy

### Purpose
Generate product copy specifically optimized for search engine visibility and keyword targeting.

### Base Prompt Template
```
You are writing SEO-optimized product copy for {PRODUCT_NAME} targeting {PRIMARY_KEYWORD}.

SEO Requirements:
- Primary Keyword: {MAIN_KEYWORD}
- Secondary Keywords: {LIST_3-5_RELATED_TERMS}
- Long-tail Keywords: {LIST_2-3_SPECIFIC_PHRASES}
- Search Intent: {INFORMATIONAL / COMMERCIAL / TRANSACTIONAL}
- Keyword Density: Natural integration, no stuffing

Product Details:
- Category: {CATEGORY}
- Key Features: {FEATURE_LIST}
- Unique Value: {DIFFERENTIATION}

Copy Requirements:
- Length: 250-350 words
- Structure: Include H2/H3 opportunities
- Tone: {TONE_VALUE}
- Include: Question-based subheadings that match search queries
- Natural Language: Conversational, not keyword-stuffed
- Meta Description: Generate 150-160 character version

Generate SEO-optimized copy that reads naturally while incorporating keywords strategically.
```

---

## Usage Guidelines

### Adapting Templates for Different Product Types

**Physical Products**: Emphasize materials, dimensions, sensory experience
**Digital Products**: Focus on features, outcomes, ease of use
**Services**: Highlight process, expertise, results
**Subscriptions**: Emphasize ongoing value, convenience, cost savings

### Tone Calibration by Industry

- **Cannabis**: Informative, welcoming, destigmatizing
- **Skincare**: Aspirational, scientific, sensory
- **Tech/SaaS**: Clear, benefit-focused, efficiency-oriented
- **Food/Beverage**: Sensory, origin-story, quality-focused
- **Professional Services**: Credible, results-driven, expertise-showcasing

### Multi-Product Scalability

For generating descriptions across large catalogs:
1. Create master template with your brand voice
2. Feed product data via CSV or structured input
3. Batch generate with consistent parameters
4. Human review for accuracy and brand fit
5. Document winning patterns for iteration

---

## Quality Control Checklist

Before publishing generated copy, verify:
- [ ] Accuracy: All claims are truthful
- [ ] Clarity: Benefits are obvious to target customer
- [ ] Differentiation: Unique value is clear
- [ ] Tone: Matches brand voice guidelines
- [ ] Length: Meets platform/format requirements
- [ ] SEO: Keywords integrated naturally
- [ ] Legal: No unsubstantiated claims
- [ ] Accessibility: Reading level appropriate

---

## Integration with Other Libraries

- See `/email-marketing-prompts.md` for product launch announcements
- See `/push-notification-prompts.md` for new arrival alerts
- See `/localization-prompts/` for regional product copy adaptation

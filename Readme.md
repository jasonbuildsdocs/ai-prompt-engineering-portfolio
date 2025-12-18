# Prompt Libraries

## Overview
This directory contains production-ready prompt templates for generating marketing and CRM content at scale. Each library focuses on a specific content type with reusable, customizable frameworks.

## Philosophy
These are **prompt systems**, not one-off prompts. Each template is:
- **Reusable**: Variable-driven for easy customization
- **Documented**: Clear purpose, usage examples, and guidelines
- **Tested**: Based on real-world application and iteration
- **Scalable**: Designed to work across hundreds or thousands of executions

## Libraries

### 📧 [Email Marketing Prompts](email-marketing-prompts.md)
Comprehensive templates for all email campaign types:
- Promotional campaigns
- Educational/value-add content
- Re-engagement/win-back
- Transactional emails
- Milestone/anniversary messages
- Subject line optimization

**Key Features:**
- Tone controls for brand voice consistency
- Variable injection for personalization
- A/B testing support
- Length/format specifications

### 📦 [Product Copy Prompts](product-copy-prompts.md)
Templates for e-commerce and product marketing:
- Short-form descriptions (marketplace/PDP)
- Long-form detailed descriptions
- Feature-focused copy
- Benefits-driven copy
- Technical specifications
- SEO-optimized product content

**Key Features:**
- Adapts to different product types
- Multiple framework options (PAS, FAB, Before-After-Bridge)
- Platform-specific optimization
- Quality control checklist

### 📱 [Push Notification & In-App Messaging](push-notification-prompts.md)
Character-constrained templates for mobile:
- Promotional push notifications
- Transactional updates
- Re-engagement messages
- Educational content alerts
- Behavior-triggered pushes
- In-app modals and banners

**Key Features:**
- Platform-specific character limits (iOS/Android)
- Urgency level controls
- Emoji usage guidelines
- Compliance best practices

### 🌍 [Localization & Translation Prompts](localization-prompts.md)
Cultural adaptation and market-specific optimization:
- Translation with cultural context
- Tone calibration by region
- Platform optimization for different markets
- Idiom and metaphor localization
- Currency/date/measurement adaptation
- Legal and regulatory compliance

**Key Features:**
- Goes beyond word-for-word translation
- Regional tone matrix
- Platform behavior by market
- Compliance frameworks

## How to Use These Libraries

### 1. Select the Appropriate Template
Choose based on:
- **Content type** you're creating (email, product copy, push notification)
- **Campaign goal** (conversion, education, re-engagement)
- **Audience** (new customers, loyal users, lapsed subscribers)

### 2. Populate Variables
Each template uses `{VARIABLE_NAME}` placeholders:
```
Example:
{BRAND_NAME} → "Green Jay Innovations"
{TONE} → "warm, scientific"
{OFFER_DESCRIPTION} → "25% off Tremella Facial Serum"
```

### 3. Adjust for Context
Customize:
- **Tone values** to match brand voice
- **Length requirements** for platform/format
- **Output structure** (paragraph vs. bullets)
- **Special instructions** for unique needs

### 4. Generate and Iterate
- Run the prompt with your LLM of choice
- Review output against quality criteria
- Refine variables if needed
- Document successful patterns

### 5. Scale
Once you find what works:
- Create batch processes for similar content
- Build prompt chains for complex workflows
- Maintain consistency across large content volumes

## Variable Best Practices

### Be Specific
❌ `{PRODUCT} → "serum"`
✅ `{PRODUCT} → "Tremella Mushroom Facial Serum - hydrating anti-aging treatment with natural polysaccharides"`

### Include Context
❌ `{AUDIENCE} → "customers"`
✅ `{AUDIENCE} → "existing customers aged 30-50 who have purchased skincare products in the last 90 days"`

### Define Tone Precisely
❌ `{TONE} → "good"`
✅ `{TONE} → "warm and scientifically-informed, avoiding beauty industry hype while maintaining accessibility"`

## Tone Library

Consistent tone values to use across templates:

| Tone | Description | Use Cases |
|------|-------------|-----------|
| **Professional** | Polished, businesslike, credible | B2B, formal sectors, technical products |
| **Friendly** | Approachable, conversational, warm | Consumer brands, service industries |
| **Enthusiastic** | Energetic, excited, bold | Promotions, launches, youth markets |
| **Urgent** | Time-sensitive, action-oriented | Flash sales, limited inventory |
| **Casual** | Relaxed, informal, personal | Lifestyle brands, younger demographics |
| **Authoritative** | Expert, confident, informative | Thought leadership, educational content |
| **Empathetic** | Understanding, supportive, caring | Customer service, sensitive topics |
| **Scientific** | Research-backed, data-driven | Healthcare, supplements, technical products |
| **Playful** | Fun, clever, lighthearted | Entertainment, creative industries |
| **Aspirational** | Inspiring, achievement-focused | Premium products, transformation messaging |

## Quality Standards

All generated content should meet these criteria:

### ✅ Clarity
- Message is immediately understandable
- No ambiguity in CTA or next steps
- Appropriate reading level for audience

### ✅ Brand Consistency
- Tone matches established voice
- Terminology aligns with brand guidelines
- Values and positioning reflected

### ✅ Accuracy
- All claims are truthful
- Product details are correct
- Legal/regulatory requirements met

### ✅ Effectiveness
- Clear value proposition
- Compelling CTA
- Appropriate urgency/emotion

### ✅ Appropriateness
- Culturally sensitive
- Platform-optimized
- Audience-appropriate

## Integration with Other Portfolio Sections

These prompt libraries work in combination with:

- **[Prompt Workflows](../prompt-workflows/)** - Multi-step processes using these templates
- **[Evaluation](../evaluation/)** - Frameworks for measuring prompt performance
- **[Visual Prompting](../visual-prompting/)** - Image generation to accompany text content

## Continuous Improvement

This is a living system. To improve these libraries:

1. **Document wins**: Track which prompts produce best results
2. **Analyze patterns**: Identify what variables drive success
3. **Iterate templates**: Refine based on performance data
4. **Add examples**: Include more real-world use cases
5. **Expand coverage**: Build templates for new content types

## Technical Notes

### Compatible LLMs
These templates have been tested with:
- Claude (Anthropic) - all versions
- GPT-4 / GPT-3.5 (OpenAI)
- Other instruction-following models

### Adaptation Required
Some models may need:
- Modified variable syntax
- Adjusted instruction style
- Different tone descriptors
- Platform-specific formatting

### Token Considerations
- Templates range from 200-500 tokens
- Add your variable content to estimate total
- Long-form outputs may approach context limits
- Consider chunking for very large content needs

## Support

For questions or contributions to these libraries:
- Review existing examples in each file
- Test variations with your specific use case
- Document what works for your brand/audience
- Share successful adaptations

---

**Next Steps:**
1. Explore individual library files
2. Try example prompts with your content
3. Adapt templates to your brand voice
4. Review [Evaluation](../evaluation/) section for testing frameworks

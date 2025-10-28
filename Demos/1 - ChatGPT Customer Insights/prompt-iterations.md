# ChatGPT Prompt Iterations - Customer Insights Analysis

This document shows three iterations of the same analytical task, demonstrating how prompt refinement improves output quality and usability.

## Use Case Context
Analyzing compiled customer reviews of AirPods Pro 3 to extract common complaints for product team review.

---

## Iteration 1: Task Only

**Prompt:**
```
Summarize the top three most common complaints from the AirPods Pro 3 review digest.
```

**Output Characteristics:**
- Comprehensive breakdown with supporting evidence
- Multiple quotes per complaint
- Detailed explanation of each issue
- Good for deep analysis, less ideal for executive summary

**Sample Output:**
```
Based on the AirPods Pro 3 Review Digest, the top three most common complaints are:

1. Sound Quality Issues – Especially Mids and Low Volume
   * Multiple users report that mids are recessed, making vocals sound muffled
   * Some find the sound tinny at low volumes with a "U-shaped" sound profile
   * Quotes:
      * "The mids just feel like they're completely removed from the music." — Reddit
      * "Pro 3s sound truly abhorrent at low volumes." — Reddit

2. Call Quality Still Not Perfect
   * Microphone clarity problems, especially in noisy environments
   * Quote: "During calls, people say I sound muffled — mic could be clearer." — Reddit

3. Missing Accessories / Cost-Cutting Concerns
   * No charging cable included frustrates users on premium product
   * Quote: "Why is there no charging cable in the box? This feels like a cheap move on a $250+ product." — Amazon
```

**What We Learned:**
Without constraints, ChatGPT defaults to verbose, comprehensive responses. Useful for exploration, but needs refinement for business use, particularly before presentation.

---

## Iteration 2: Adding Persona and Output Format

**Prompt:**
```
You are a customer experience analyst. Based only on the uploaded AirPods Pro 3 review digest, return three bullet points summarizing the most common customer complaints. Include one short supporting quote under each bullet.
```

**Key Improvements:**
- Added persona context ("customer experience analyst")
- Specified output format (three bullets with quotes)
- Constrained scope ("based only on the uploaded document")
- More concise, scannable output

**Output:**
```
- Muffled call quality in noisy environments
  "During calls, people say I sound muffled — mic could be clearer."

- Inconsistent sound quality, especially mids and low volumes
  "Pro 3s sound truly abhorrent at low volumes. U-shaped sound profile kills the mids."

- Lack of included charging cable despite premium price
  "Why is there no charging cable in the box? This feels like a cheap move on a $250+ product."
```

**What We Learned:**
Role assignment and format constraints dramatically improved usability. Output went from "interesting analysis" to "ready to share with the team."

---

## Iteration 3: Adding Tone and Context - Stakeholder Ready Memo

**Prompt:**
```
You are a customer experience analyst preparing a summary for the product team. Using only the uploaded AirPods Pro 3 review digest, write a one-paragraph internal memo summarizing the top user complaints. Keep the tone neutral, professional, and focused on actionable insight.
```

**Key Improvements:**
- Specified audience ("for the product team")
- Defined output format (one-paragraph memo)
- Set tone expectations (neutral, professional, actionable)
- Emphasized synthesis over listing

**Output:**
```
Internal Memo: Top User Complaints – AirPods Pro 3

User feedback highlights several recurring concerns that may inform future iterations. The most common complaints center on inconsistent sound quality—while bass performance is praised, others report recessed mids and tinny output at lower volumes. Call quality, though improved, still draws criticism for muffled voice pickup in noisy environments. Users note frustration over lack of manual EQ customization in iOS settings. The removal of the charging cable from the box has been widely viewed as cost-cutting that detracts from perceived value. Additional issues include limited reliability of Live Translation for longer phrases, slight reductions in battery life, and occasional fit instability during workouts. These insights suggest opportunities for refinement in audio tuning, accessory inclusion, software features, and active-use ergonomics.
```

**What We Learned:**
Audience specification transformed the output from generic summary to actionable business communication. Same data, same complaints, but framed for decision-making.

---

## Prompt Engineering Principles Demonstrated

### 1. Role Assignment
Giving ChatGPT a role ("You are a customer experience analyst") provides context for tone and perspective.

### 2. Output Constraints
Specifying format (bullets, paragraph, word count) ensures usability and prevents over-generation.

### 3. Scope Limitation
"Based only on the uploaded document" prevents hallucination and ensures grounding in actual provided data.

### 4. Context Awareness
"For the product team" vs. executive summary changes emphasis and detail level.

### 5. Tone Control
"Neutral, professional, actionable" guides output style and prevents editorializing.

## Business Applications

This technique scales to:
- Product teams synthesizing user feedback from multiple channels
- Customer success identifying common pain points for proactive outreach
- Marketing understanding customer language for messaging
- Executive reporting condensing thousands of data points into decision-ready summaries
- Competitive intelligence tracking competitor product reception

## Try It Yourself

**Exercise**: Take any collection of reviews (Amazon, Google, Yelp) and:
1. Start with an open-ended prompt
2. Add role and format constraints
3. Specify audience and tone
4. Compare the three outputs

Notice how the same underlying analysis becomes progressively more useful with each iteration.
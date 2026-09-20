# Case 5: PhonePe

## Solution to design a new marketplace platform.

To successfully complete this case study, here is a step-by-step roadmap that directly maps to the deliverables outlined in your guide.

**Step-by-Step Approach**

**Step 1: Filter Queries for Commercial Intent**

Using an LLM (such as ChatGPT, Claude, or Gemini) with **Few-Shot** or **Chain-of-Thought (CoT)** prompting, run through all 941 queries in the Excel sheet to classify them into:

- **Commercial (YES):** Users seeking to buy a physical product or tangible good (e.g., "fitness bands under 3000").   

- **Non-Commercial (NO):** Informational, informational services, or general search queries (e.g., "how to improve memory").

**Recommended Prompt Template for Step 1:**

You are an e-commerce Product Manager. Analyze the following list of Google search queries.

For each query:

1. Classify intent: "Commercial" (intent to purchase a physical product) or "Non-Commercial" (informational/service/general).
2. Explain the reasoning step-by-step.
3. If "Commercial", suggest the physical product/item to sell on PhonePe Marketplace.

Examples:

Query: "best smartphones under 15000" -> Intent: Commercial | Product: Smartphones

Query: "how to lose weight fast" -> Intent: Non-Commercial | Product: N/A

**Step 2: Validate Marketplace Fit for PhonePe**

Filter for queries classified as **Commercial** and ensure they map directly to physical goods suitable for an in-app e-commerce marketplace platform (e.g., PhonePe Switch / PhonePe Store). Exclude intangible services unless they are bundled with physical goods.

**Step 3: Define the Category & Subcategory Structure**

Group the filtered commercial queries into a standard, intuitive e-commerce catalog taxonomy:   

- **Level 1:** Broad Top-Level Category (e.g., Electronics & Gadgets, Fashion & Apparel, Home & Living, Health & Personal Care, Groceries & Foods).

- **Level 2:** Subcategory (e.g., Smart Wearables, Kitchen Appliances, Ethnic Wear).

- **Level 3:** Mapped Queries / Sample Products.

**Step 4: Final Deliverables Format**

Organize your analysis into two distinct deliverables:

1. **Category Hierarchy Summary Table**

| Category          | Subcategory | Target Sample Products | High-Intent Search Queries |
| --- | --- | --- | --- |
| Electronics | Smartwatches & Fitness Bands | Fitness Trackers, Smartwatches | "fitness bands under 3000" | 
| Fashion | Traditional Wear | Silk Sarees, Designer Kurtas	| "traditional silk sarees online" |

2. Categorized Dataset File / Output

- Update the Case study Queries.xlsx sheet by adding 3 columns:

  - Intent (Commercial / Non-Commercial)

  - Category

  - Subcategory
 
**Step 5: Document and Present**

● Prepare a clean document or table:

○ Top Level Categories

○ Subcategories under each

○ Sample products (optional)

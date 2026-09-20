# NextLeap-Case-5-2026

## Case 5: PhonePe

**🛠 Guide: How to Approach the Problem (Suggested Steps)**

**The Problem**

**You are a Product Manager at PhonePe/Any fintech app, and you’ve been tasked with helping to design a new marketplace platform.**

PhonePe wants to explore trending topics to identify potential new product categories and opportunities for commerce.

You have been given a list of [top trending search queries] from **Google Trends (India).**

**Your goal is to:**

1.	Use prompt engineering techniques to **filter** the queries and **identify** those that show **commercial intent** (i.e., users searching with an intent to buy or explore products).
2.	Decide whether these commercially-relevant queries could lead to goods that PhonePe should offer on its marketplace.
3.	Build a **structured category and subcategory plan** for the marketplace, based on the filtered queries.

**Deliverables**

At the end of the exercise, you should be able to:

●	Present a **list of commercial categories** PhonePe can target.

●	Propose a **Category → Subcategory** structure for PhonePe's new marketplace.

### Guide

#### Step 1: Understand Commercial Intent

●	Ask yourself: "Is the user likely looking to buy something?"

●	Examples of commercial queries:

○	"Best budget smartphones 2024"

○	"Fitness bands under 3000"

○	"Traditional silk sarees online"

●	Non-commercial examples (skip these):

○	"How to improve memory"

○	"India vs Pakistan match highlights"

✅ **Tip:** You can design a **Zero-shot or Few-shot prompt** for the model:

"Analyze the following query. Is the user likely to intend a purchase? Answer YES or NO, and explain why."

#### Step 2: Build a Filtering Prompt

●	Use prompt engineering (Zero-shot / Few-shot / Style prompting) to classify the 950 queries.

●	Decide which queries are **commercially viable.**

●	Tag queries: "Commercial" / "Non-commercial."

✅ **Optional Bonus:**

 Use **Chain of Thought** prompting if needed - force the model to "think step-by-step" before deciding.

#### Step 3: Validate Marketplace Fit

●	For each commercial query, think:

"Is there a real good/product that could be listed on PhonePe marketplace?"

●	Ignore services (e.g., "How to lose weight") unless they can clearly tie to a product (e.g., "fitness equipment").

#### Step 4: Create the Marketplace Structure

●	Group similar products together into **categories** and **subcategories.**

●	Example Structure:

○	**Category:** Electronics

■	**Subcategories:** Smartphones, Smartwatches, Headphones

○	**Category:** Fashion

■	**Subcategories:** Sarees, Kurtas, Sports Shoes

✅ **Tip:** Try to think like a real product catalog designer — logical, easy for users to browse.

#### Step 5: Document and Present

●	Prepare a clean document or table:

○	Top Level Categories

○	Subcategories under each

○	Sample products (optional)

## Click on [PhonePe](phonepe.md)

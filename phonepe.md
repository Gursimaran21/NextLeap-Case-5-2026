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

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Prompt 1

Used ChatGPT LLM with **Few-Shot** or **Chain-of-Thought (CoT)** prompting, run through all 941 queries in the Excel sheet to classify them into:

- **Commercial (YES):** Users seeking to buy a physical product or tangible good (e.g., "fitness bands under 3000").   

- **Non-Commercial (NO):** Informational, informational services, or general search queries (e.g., "how to improve memory").

You are an e-commerce Product Manager. Analyze the following list of Google search queries.

For each query:

1. Classify intent: "Commercial" (intent to purchase a physical product) or "Non-Commercial" (informational/service/general).
2. Explain the reasoning step-by-step.
3. If "Commercial", suggest the physical product/item to sell on PhonePe Marketplace.

Examples:

Query: "best smartphones under 15000" -> Intent: Commercial | Product: Smartphones

Query: "how to lose weight fast" -> Intent: Non-Commercial | Product: N/A

### Prompt Response 1

I analyzed all **941 Google search queries** using the rule: **Commercial = clear intent to research, compare, discover, or purchase a physical product**. Service, informational, travel, jobs, finance, apps, restaurants, etc. are classified as Non-Commercial.

**Summary**

| Intent         | Queries |         % |
| -------------- | ------: | --------: |
| Commercial     | **119** | **12.6%** |
| Non-Commercial | **822** | **87.4%** |
| **Total**      | **941** |  **100%** |

For each query, the output includes:

- Intent
- Step-by-step reasoning
- Physical product to sell on PhonePe Marketplace for Commercial queries
- N/A for Non-Commercial queries

**Sample classifications**

| Query                                            | Intent         | Product                        |
| ------------------------------------------------ | -------------- | ------------------------------ |
| best smartphones under 15000 india               | Commercial     | Smartphones                    |
| best fitness trackers for activity monitoring    | Commercial     | Fitness trackers / smart bands |
| where to buy organic and locally-sourced produce | Commercial     | Organic groceries / produce    |
| best gaming phone under Rs. 20,000 India         | Commercial     | Gaming smartphones             |
| best laptops for students india                  | Commercial     | Laptops                        |
| air purifiers india                              | Commercial     | Air purifiers                  |
| best baby strollers for different needs          | Commercial     | Baby strollers                 |
| best noise-canceling headphones for travel       | Commercial     | Headphones                     |
| how to improve sleep quality                     | Non-Commercial | N/A                            |
| best travel insurance for different needs        | Non-Commercial | N/A                            |
| meditation apps for stress relief india          | Non-Commercial | N/A                            |
| best online yoga classes india                   | Non-Commercial | N/A                            |
| IT jobs for freshers in India                    | Non-Commercial | N/A                            |

**Download the complete Excel analysis:** 

**Download PhonePe Marketplace Query Intent Analysis** 

**Go to [Data PhonePe Marketplace Query Intent Analysis](Data/PhonePe_Marketplace_Query_Intent_Analysis.xlsx)** --> **(Refer Data Folder)**

### Prompt 2

Filter for queries classified as **Commercial** and ensure they map directly to physical goods suitable for an in-app e-commerce marketplace platform (e.g., PhonePe Switch / PhonePe Store). Exclude intangible services unless they are bundled with physical goods.

### Prompt Response 2

Filtered the dataset to retain only **Commercial queries that directly map to tangible, marketplace-sellable physical goods.**

**Result**

- **Original queries:** 941
- **Commercial queries:** 121? Wait—after applying the source file's classifications, the filtered set contains **117 physical-goods queries**
- **Excluded:** 4 queries that were primarily about marketplaces, shopping locations, or subscriptions rather than a direct physical product.

Examples retained:

- “best smartphones under 15000 india” → **Smartphones**
- “best laptops for students india” → **Laptops**
- “best yoga mats for at-home workouts” → **Yoga mats**
- “best cat food brands for kittens” → **Cat food**
- “best air purifiers for eliminating allergens” → **Air purifiers**

Examples excluded:

- Used-furniture marketplace queries
- Used-book marketplace query
- Shopping-location query
- Coffee subscription query

**Download the filtered PhonePe physical-goods query-list:** 

**PhonePe_Physical_Good_Commercial_Queries.xlsx** --> **(Refer Data Folder)**

### Prompt 3

Group the filtered commercial queries into a standard, intuitive e-commerce catalog taxonomy:   

- **Level 1:** Broad Top-Level Category (e.g., Electronics & Gadgets, Fashion & Apparel, Home & Living, Health & Personal Care, Groceries & Foods).

- **Level 2:** Subcategory (e.g., Smart Wearables, Kitchen Appliances, Ethnic Wear).

- **Level 3:** Mapped Queries / Sample Products.

### Prompt Response 3

Below is a standardized **3-level e-commerce taxonomy** for the **115 filtered Commercial queries**. I’ve normalized similar products into intuitive marketplace categories and treated Level 3 as the actual search-query/product mapping.

**PhonePe Marketplace Catalog Taxonomy**

| Level 1 - Top Category         | Level 2 - Subcategory              | Level 3 - Mapped Queries / Sample Products                                                                                                                                                                                                      |
| ------------------------------ | ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Electronics & Gadgets**      | **Smartphones**                    | *best smartphones under 15000 india*; *top-rated smartphones on the market*; *best gaming smartphones and laptops in India* → **Smartphones / Gaming Smartphones**                                                                              |
|                                | **Laptops & Tablets**              | *best laptops for students india*; *best laptops for students under a budget*; *best gaming laptops for high performance*; *best budget-friendly tablets for everyday use* → **Laptops / Gaming Laptops / Tablets**                             |
|                                | **Smart Wearables**                | *best fitness trackers for activity monitoring*; *top-rated fitness trackers*; *waterproof fitness trackers india*; *fitness trackers india 2021 vs 2024* → **Fitness Trackers / Smart Bands**                                                  |
|                                | **Audio**                          | *best noise-canceling headphones for travel*; *wireless headphones india* → **Wireless / Noise-Cancelling Headphones**                                                                                                                          |
|                                | **Smart Home & Connected Devices** | *smart home devices that simplify your life*; *smart home gadgets for kitchen automation*; *smart home devices india* → **Smart Home Devices / Smart Kitchen Gadgets**                                                                          |
|                                | **TVs & Home Entertainment**       | *differences between smart TVs and regular TVs*; *best video game consoles for families* → **Smart TVs / Gaming Consoles**                                                                                                                      |
|                                | **Cameras & Security**             | *security cameras for home india*; *best cameras for beginner photographers*; *best pet cameras to monitor your furry friend* → **Digital Cameras / Security Cameras / Pet Cameras**                                                            |
| **Home & Living**              | **Large Home Appliances**          | *air conditioners india*; *Automatic washing machine vs semi-automatic washing machine India*; *buying guide for new washing machines*; *features to consider when purchasing a refrigerator* → **ACs / Washing Machines / Refrigerators**      |
|                                | **Air Quality**                    | *Best air purifiers for eliminating allergens*; *air purifiers for allergies*; *air purifiers for home gyms india*; *air purifiers india* → **Air Purifiers**                                                                                   |
|                                | **Kitchen Appliances & Gadgets**   | *best kitchen appliances for healthy cooking*; *kitchen gadgets that save time and effort*; *Kitchen gadgets for making life easier*; *Best brands for pressure cookers in India* → **Kitchen Appliances / Kitchen Gadgets / Pressure Cookers** |
|                                | **Furniture**                      | *comfortable and stylish furniture for living rooms*; *best outdoor furniture for patios and decks*; *online furniture stores india* → **Living Room / Outdoor Furniture**                                                                      |
|                                | **Home Comfort**                   | *best mattresses for a good night's sleep*; *best gaming chairs for long gaming sessions* → **Mattresses / Gaming Chairs**                                                                                                                      |
|                                | **Party & Home Décor**             | *Party supplies and decorations for different occasions* → **Party Supplies / Decorations**                                                                                                                                                     |
| **Fashion & Apparel**          | **Women's & Men's Clothing**       | *sustainable clothing brands india*; *best online clothing stores for women*; *where to buy plus-size clothing online*; *affordable and stylish clothing brands for teens* → **Clothing / Plus-Size / Teen Fashion**                            |
|                                | **Activewear & Sports Apparel**    | *activewear brands for women india*; *best activewear brands for women and men*; *best sports apparel brands for athletes and fans*; *winter sports clothing and gear essentials* → **Activewear / Sports Apparel / Winter Sportswear**         |
|                                | **Footwear**                       | *best running shoes for different types of feet*; *Best sports shoes for different sports*; *comfortable and stylish hiking boots*; *best shoes for comfort and style* → **Running Shoes / Sports Shoes / Hiking Boots / Casual Shoes**         |
|                                | **Bags & Luggage**                 | *best travel backpacks for carry-on luggage*; *top-rated luggage brands for durability* → **Travel Backpacks / Luggage**                                                                                                                        |
|                                | **Jewellery & Accessories**        | *ethical jewelry brands for conscious consumers* → **Jewellery / Fashion Accessories**                                                                                                                                                          |
|                                | **Winter Wear**                    | *winter coat buying guide for different climates* → **Winter Coats / Jackets**                                                                                                                                                                  |
| **Beauty & Personal Care**     | **Makeup & Cosmetics**             | *cruelty-free and vegan makeup brands*; *best makeup for different skin tones*; *best kajal brands for Indian eyes* → **Makeup / Kajal / Cosmetics**                                                                                            |
|                                | **Skincare**                       | *best anti-aging skincare products* → **Skincare / Anti-Aging Products**                                                                                                                                                                        |
|                                | **Hair Care & Styling**            | *best hair care products for specific hair types*; *best hair straightening products for frizzy hair india* → **Hair Care / Hair Styling Tools & Products**                                                                                     |
| **Health & Wellness**          | **Vitamins & Supplements**         | *best multivitamin tablets for adults*; *best protein powder for muscle gain india* → **Multivitamins / Protein Powder**                                                                                                                        |
|                                | **Fitness & Exercise**             | *best yoga mats for at-home workouts* → **Yoga Mats / Exercise Accessories**                                                                                                                                                                    |
| **Groceries & Foods**          | **Fresh & Organic Foods**          | *where to buy organic and locally-sourced produce* → **Organic Fruits / Vegetables / Groceries**                                                                                                                                                |
|                                | **Tea & Coffee**                   | *best coffee brands* → **Coffee / Coffee Beans**                                                                                                                                                                                                |
| **Pet Supplies**               | **Pet Food**                       | *best cat food brands for kittens*; *best dog food brands for different breeds* → **Cat Food / Dog Food**                                                                                                                                       |
|                                | **Pet Accessories**                | *stylish and comfortable dog clothes and accessories*; *online pet supplies india*; *Best pet supplies for dogs, cats, or other pets* → **Pet Accessories / Pet Supplies**                                                                      |
|                                | **Cat Supplies**                   | *best cat litter and litter boxes*; *best scratching posts for cats*; *best cat toys for different play styles* → **Cat Litter / Scratching Posts / Cat Toys**                                                                                  |
| **Baby & Kids**                | **Baby Gear**                      | *best baby strollers for different needs*; *baby monitors for peace of mind* → **Baby Strollers / Baby Monitors**                                                                                                                               |
|                                | **Baby Food & Feeding**            | *organic baby food brands for healthy eating* → **Organic Baby Food**                                                                                                                                                                           |
|                                | **Kids' Clothing**                 | *comfortable and stylish clothing for babies* → **Baby / Kids Clothing**                                                                                                                                                                        |
|                                | **Toys & Learning**                | *educational toys for children's development*; *safe and fun toys for toddlers* → **Educational Toys / Toddler Toys**                                                                                                                           |
| **Sports, Fitness & Outdoors** | **Cycling**                        | *best bikes for commuting and recreation* → **Bicycles / Cycling Accessories**                                                                                                                                                                  |
|                                | **Camping & Outdoor Recreation**   | *essential camping gear for beginners*; *essential travel gear for parents with young children* → **Camping / Outdoor Gear / Travel Accessories**                                                                                               |
|                                | **Sports Equipment**               | *where to buy affordable sports equipment*; *water sports equipment for kayaking and paddleboarding* → **Sports Equipment / Water Sports Gear**                                                                                                 |
|                                | **Cricket**                        | *cricket bat brands india* → **Cricket Bats / Cricket Equipment**                                                                                                                                                                               |
|                                | **Astronomy & Optics**             | *telescopes and binoculars for stargazing enthusiasts*; *best telescopes for stargazing beginners*; *best telescopes for amateur astronomy enthusiasts* → **Telescopes / Binoculars**                                                           |
|                                | **Musical Instruments**            | *musical instruments for beginners to learn*; *Musical instruments for professional musicians*; *where to buy musical instruments online* → **Musical Instruments**                                                                             |
| **Books & Stationery**         | **Books & Literature**             | *best books on Indian mythology and religious texts*; *best-selling Indian novels*; *best historical fiction novels*; *best romance novels by Indian authors*; *most popular books by Indian authors in translation* → **Books / Novels**       |
|                                | **Children's Books**               | *best Indian children's books for different age groups*; *Best picture books for toddlers and preschoolers*; *popular Indian children's book series for young readers* → **Children's Books / Picture Books**                                   |
|                                | **Cookbooks & Self-Help**          | *best cookbooks featuring Indian cuisine*; *best cookbooks for learning new cuisines*; *Self-help books for dealing with stress and anxiety* → **Cookbooks / Self-Help Books**                                                                  |
|                                | **Business & Professional Books**  | *best business and management books by Indian writers*; *best biographies of famous Indian personalities* → **Business Books / Biographies**                                                                                                    |
|                                | **Art & Office Supplies**          | *Best art supplies for professional artists or hobbyists*; *Best office supplies for organization and productivity*; *Sustainable and eco-friendly office supplies* → **Art Supplies / Office Supplies**                                        |
| **Toys, Games & Hobbies**      | **Board Games**                    | *popular board games for family game nights*; *best board games for family game nights* → **Board Games**                                                                                                                                       |
| **Travel & Lifestyle**         | **Travel Accessories**             | *best travel backpacks for carry-on luggage*; *essential travel gear for parents with young children* → **Travel Backpacks / Travel Accessories**                                                                                               |

**Recommended final PhonePe taxonomy structure**

For an actual marketplace, I'd simplify the above into **10 Level-1 categories:**

1. **Electronics & Gadgets**
2. **Home & Living**
3. **Fashion & Apparel**
4. **Beauty & Personal Care**
5. **Health & Wellness**
6. **Groceries & Foods**
7. **Pet Supplies**
8. **Baby & Kids**
9. **Sports, Fitness & Outdoors**
10. **Books, Stationery & Hobbies**

This structure avoids creating overly narrow top-level categories while still allowing PhonePe to merchandise products through **Level 2 → Level 3**.

**Important normalization:** Queries such as “best online bookstores”, “online clothing stores”, “where to buy musical instruments”, and “online furniture stores” remain Commercial because the **underlying object of purchase is a physical good.** The fact that the query contains “online” or “store” does not make it a service query.

### Prompt 4

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

### Prompt Response 4

Done. I created both requested deliverables.

1. **Category Hierarchy Summary**

   The workbook includes a **Category Hierarchy** sheet with:

   | Category           | Subcategory                   | Target Sample Products                | High-Intent Search Queries         |
   | ------------------ | ----------------------------- | ------------------------------------- | ---------------------------------- |
   | Electronics        | Smartphones                   | Smartphones / Gaming Smartphones      | Representative high-intent queries |
   | Electronics        | Smartwatches & Fitness Bands  | Fitness Trackers / Smartwatches       | Representative high-intent queries |
   | Fashion            | Traditional Wear              | Sarees / Kurtas / Ethnic Wear         | Representative high-intent queries |
   | Home & Living      | Kitchen Appliances & Cookware | Pressure Cookers / Kitchen Appliances | Representative high-intent queries |
   | Health & Wellness  | Vitamins & Supplements        | Multivitamins / Protein Powder        | Representative high-intent queries |
   | Pet Supplies       | Pet Food                      | Cat Food / Dog Food                   | Representative high-intent queries |
   | Baby & Kids        | Baby Gear                     | Strollers / Baby Monitors             | Representative high-intent queries |
   | Sports & Outdoors  | Cricket                       | Cricket Bats / Equipment              | Representative high-intent queries |
   | Books & Stationery | Books & Literature            | Books / Novels                        | Representative high-intent queries |

   The taxonomy contains **42 Category → Subcategory combinations.**

2. **Categorized Dataset**

   The original ```Case study Queries.xlsx``` has been updated with these three columns:

   - **Intent** — Commercial / Non-Commercial
   - **Category**
   - **Subcategory**

   The resulting dataset contains **941 queries:**

   - **244 Commercial**
   - **697 Non-Commercial**

**Download the completed** ```Case study Queries - Categorized.xlsx``` 

**Case study Queries - Categorized.xlsx** --> **(Refer Data Folder)**

### Prompt 5

● Prepare a clean document or table:

○ Top Level Categories

○ Subcategories under each

○ Sample products (optional)

### Prompt Response 5

**E-commerce Catalog Taxonomy**

| **Top-Level Category**     | **Subcategories**             | **Sample Products**                                       |
| -------------------------- | ----------------------------- | --------------------------------------------------------- |
| **Electronics & Gadgets**  | Smartphones                   | Smartphones, Gaming Smartphones                           |
|                            | Laptops & Computers           | Laptops, Gaming Laptops, PCs                              |
|                            | Tablets                       | Android Tablets, iPads                                    |
|                            | Smart Wearables               | Smartwatches, Fitness Bands, Fitness Trackers             |
|                            | Audio                         | Wireless Headphones, Earbuds, Noise-Cancelling Headphones |
|                            | Cameras & Security            | Digital Cameras, Security Cameras, Pet Cameras            |
|                            | TVs & Gaming                  | Smart TVs, Gaming Consoles, Controllers                   |
|                            | Mobile & Power Accessories    | Chargers, Power Banks, Cables, Adapters                   |
| **Home & Living**          | Air Quality Appliances        | Air Purifiers, Humidifiers                                |
|                            | Large Appliances              | Air Conditioners, Refrigerators, Washing Machines         |
|                            | Kitchen Appliances & Cookware | Air Fryers, Blenders, Mixers, Pressure Cookers, Cookware  |
|                            | Furniture                     | Sofas, Chairs, Tables, Desks                              |
|                            | Home Comfort                  | Mattresses, Pillows, Bedding, Gaming Chairs               |
|                            | Home & Party Décor            | Home Décor, Party Decorations, Party Supplies             |
| **Fashion & Apparel**      | Traditional Wear              | Silk Sarees, Designer Kurtas, Lehengas, Salwar Suits      |
|                            | Western & Casual Wear         | Dresses, Shirts, T-Shirts, Jeans                          |
|                            | Activewear & Sportswear       | Gym Wear, Sports Apparel, Winter Sportswear               |
|                            | Footwear                      | Running Shoes, Sports Shoes, Hiking Boots, Sneakers       |
|                            | Bags & Luggage                | Backpacks, Handbags, Suitcases, Travel Luggage            |
|                            | Jewellery & Accessories       | Jewellery, Fashion Accessories                            |
| **Beauty & Personal Care** | Makeup & Cosmetics            | Makeup, Kajal, Cosmetics                                  |
|                            | Skincare                      | Moisturizers, Sunscreen, Anti-Aging Products              |
|                            | Hair Care & Styling           | Shampoos, Hair-Care Products, Hair Styling Products       |
| **Health & Wellness**      | Vitamins & Supplements        | Multivitamins, Protein Powder, Supplements                |
|                            | Fitness Equipment             | Yoga Mats, Dumbbells, Resistance Bands                    |
| **Groceries & Foods**      | Fresh & Organic Groceries     | Organic Fruits, Vegetables, Fresh Produce                 |
|                            | Tea & Coffee                  | Coffee, Coffee Beans, Tea                                 |
|                            | Snacks & Packaged Foods       | Snacks, Biscuits, Chocolates, Packaged Foods              |
| **Pet Supplies**           | Pet Food                      | Dog Food, Cat Food, Kitten Food                           |
|                            | Pet Accessories               | Pet Clothes, Pet Accessories, Pet Supplies                |
|                            | Cat Supplies                  | Cat Litter, Litter Boxes, Scratching Posts, Cat Toys      |
| **Baby & Kids**            | Baby Gear                     | Baby Strollers, Baby Monitors                             |
|                            | Baby Food & Feeding           | Baby Food, Infant Food, Feeding Products                  |
|                            | Kids Clothing                 | Baby Clothes, Kids' Clothing                              |
|                            | Toys & Learning               | Educational Toys, Toddler Toys                            |
| **Sports & Outdoors**      | Cycling                       | Bicycles, Cycling Accessories                             |
|                            | Camping & Outdoor Gear        | Camping Equipment, Outdoor Gear                           |
|                            | Sports Equipment              | Sports Equipment, Water-Sports Equipment                  |
|                            | Cricket                       | Cricket Bats, Cricket Equipment                           |
|                            | Optics & Astronomy            | Telescopes, Binoculars                                    |
| **Books & Stationery**     | Books & Literature            | Novels, Indian Literature, Biographies                    |
|                            | Cookbooks & Self-Help         | Cookbooks, Self-Help Books                                |
|                            | Office & Art Supplies         | Stationery, Office Supplies, Art Supplies                 |
| **Toys, Games & Hobbies**  | Board Games                   | Family Board Games, Strategy Games                        |
|                            | Musical Instruments           | Guitars, Keyboards, Musical Instruments                   |

**Recommended Top-Level Navigation**

## Go back to [README](README.md)
For a PhonePe-style marketplace, these can be surfaced as:

**Electronics & Gadgets → Home & Living → Fashion & Apparel → Beauty & Personal Care → Health & Wellness → Groceries & Foods → Pet Supplies → Baby & Kids → Sports & Outdoors → Books & Stationery → Toys, Games & Hobbies**

This gives a relatively compact **11-category top-level navigation**, while the subcategories provide enough depth for search, browsing, and merchandising.

# Glasshouse Specification
**Every Ingredient Has a Purpose**
- HTML Mirror:  [https://roxanneardary.com/glasshouse-specification/](https://roxanneardary.com/glasshouse-specification/)  

---

Glasshouse is an open, modular specification for building AI-powered cocktail and mocktail management systems. The specification defines interoperable components for inventory management, recipe generation, conversational AI, shopping intelligence, pricing analysis, and privacy-first operation while remaining implementation independent.

Rather than prescribing a specific programming language or framework, Glasshouse defines how each module communicates, the data each module manages, and the expected behavior of the overall system. Implementations may be desktop, mobile, web, self-hosted, or embedded.

The specification is designed for local-first deployments, self-contained AI, end-to-end encrypted communication, and modular expansion without vendor lock-in.

---

# Goals

- AI-powered beverage management
- Voice-first interaction
- Modular architecture
- Local-first operation
- Self-contained AI
- Privacy by design
- End-to-end encryption
- Cross-platform compatibility
- Vendor independence
- Community-driven development

---

# Core Modules

## Inventory Engine

Maintains a complete inventory of:

- Liquor
- Liqueurs
- Bitters
- Mixers
- Soda
- Juice
- Syrups
- Fresh fruit
- Herbs
- Garnishes
- Ice varieties
- Glassware
- Cocktail tools

Features include:

- Voice inventory updates
- Manual entry
- Barcode scanning
- Bulk import
- Inventory history
- Quantity tracking
- Unit conversion
- Expiration monitoring
- Shelf organization
- Favorite brands

---

## Conversational AI

Natural language interaction including:

- Inventory updates
- Shopping requests
- Recipe requests
- Flavor recommendations
- Party planning
- Ingredient substitutions
- Brand comparisons
- Price inquiries
- Educational questions

Supports:

- Voice
- Text
- Multi-turn conversations
- Context awareness

---

## Recipe Engine

Generates recipes based upon available inventory.

Supports:

- Cocktails
- Mocktails
- Low alcohol
- Zero proof
- Custom recipes
- Community recipes
- Seasonal recipes
- Holiday collections

Recipe filtering includes:

- Spirit
- Flavor profile
- Sweet
- Tangy
- Sour
- Bitter
- Herbal
- Fruity
- Smoky
- Spicy
- Creamy
- Strength
- Difficulty
- Preparation time
- Glass type
- Garnish
- Occasion

---

## Recipe Intelligence

AI can:

- Create new recipes
- Suggest substitutions
- Scale servings
- Recommend garnishes
- Recommend glassware
- Improve balance
- Reduce sweetness
- Increase acidity
- Adjust alcohol content
- Convert cocktails to mocktails
- Convert mocktails to cocktails

---

## Taste Profile Engine

Learns user preferences including:

- Favorite spirits
- Favorite flavors
- Preferred strength
- Sweetness tolerance
- Citrus preference
- Herbal preference
- Spice preference
- Frequently used ingredients
- Seasonal preferences

---

## Shopping Intelligence

Automatically generates shopping lists.

Supports:

- Missing ingredients
- Low inventory
- Party planning
- Event shopping
- Weekly restocking
- Favorite brands
- Generic alternatives

---

## Dynamic Price Intelligence

Tracks pricing over time.

Capabilities include:

- Historical pricing
- Price trends
- Price increases
- Price drops
- Sale notifications
- Cheapest retailer
- Price per ounce
- Unit price comparison
- Regional pricing
- Brand comparison
- Substitute recommendations
- Generic alternatives
- Premium alternatives

Users may monitor:

- Individual products
- Entire brands
- Categories
- Favorite retailers

---

## Sustainability Engine

Encourages reduced waste through:

- Ingredient-first recipes
- Expiration awareness
- Leftover ingredient usage
- Seasonal ingredients
- Efficient shopping
- Reduced duplicate purchases

---

## Analytics Module

Supports analytics including:

- Inventory turnover
- Ingredient usage
- Favorite recipes
- Favorite spirits
- Spending trends
- Savings analysis
- Price history
- Shopping frequency
- Waste reduction
- Recipe popularity

Analytics should remain under user control.

---

# Modular Design

Each Glasshouse module is independent.

Implementations may include only the modules required.

Example deployments include:

- Inventory only
- Recipe engine only
- Shopping assistant
- Price tracker
- Voice bartender
- Mocktail assistant
- Enterprise hospitality system
- Restaurant inventory manager
- Event planning platform

Modules communicate through documented interfaces and should remain loosely coupled whenever possible.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/glasshouse/](https://roxanneardary.com/glasshouse/)

---

## License & Notice Requirements

Glasshouse is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Glasshouse specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  

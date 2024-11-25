# Entry-Level Luxury Car Market Analysis

## Overview
This project analyzes social media conversations from Edmunds.com forums to provide competitive insights about the entry-level luxury car market in the USA. The analysis includes text mining, brand association analysis, and feature analysis to understand consumer preferences and brand perceptions.

## Table of Contents
- [Data Collection](#data-collection)
- [Analysis Tasks](#analysis-tasks)
- [Key Findings](#key-findings)
- [Methodology](#methodology)
- [Results](#results)
- [Business Implications](#business-implications)
- [Technical Details](#technical-details)

## Data Collection
- Source: Edmunds.com discussion forums
- Focus: Entry-level luxury car discussions
- Sample size: ~5000 posts
- Data format: CSV with date and message content

## Analysis Tasks
1. **Zipf's Law Testing**
   - Econometric analysis of word frequencies
   - Plot of top 100 words against theoretical prediction
   [Insert Zipf's law plot here]

2. **Brand Frequency Analysis**
   - Identified top 10 brands by frequency
   - Analyzed brand mentions while accounting for model-to-brand mapping
   - Top brands identified:
     ```
     1. BMW
     2. Audi
     3. Acura
     4. Lexus
     5. Infiniti
     6. Honda
     7. Nissan
     8. Toyota
     9. Porsche
     10. Cadillac
     ```

3. **Brand Association Analysis**
   - Calculated lift ratios between top brands
   - Created MDS visualization of brand relationships
   [Insert your MDS plot here]

4. **Feature Analysis**
   - Identified most discussed car attributes
   - Analyzed brand-feature associations
   - Top 5 features:
     ```
     1. Price - 1708 mentions
     2. Performance - 1625 mentions
     3. Engine - 1217 mentions
     4. Power - 969 mentions
     5. AWD - 875 mentions
     ```

## Key Findings

### Brand Associations
    1. Brand Clustering and Positioning:
        - The MDS map shows distinct clustering of brands, which suggests different market positioning and consumer perceptions.
        - BMW and Audi are closely positioned, indicating they are perceived similarly and likely compete directly in the luxury market.
        - Honda, Toyota, and Nissan form another cluster, suggesting they are viewed more as mainstream brands even in luxury discussions.
        - Acura, Lexus, and Infiniti form a middle ground between the German luxury brands and their Japanese parent companies.

    2. Brand Associations:
        - Honda and Toyota have the strongest association (lift ratio of 2.51), indicating that these brands are often discussed together, possibly as benchmarks or alternatives in the entry-level luxury segment.
        - Nissan and Toyota also have a strong association (1.91), reinforcing the Japanese brand cluster.
        - Infiniti shows moderate associations with both Nissan (0.94) and Lexus (0.89), positioning it as a bridge between mainstream and luxury Japanese brands.

    3. Luxury Brand Dynamics:
        - BMW and Audi have a moderate association (0.44), confirming their position as direct competitors in the luxury market.
        - Porsche appears to be somewhat isolated in the MDS map, suggesting it might be perceived as a more exclusive or performance-oriented brand compared to the other luxury marques.

    4. Entry-Level Luxury Positioning:
        - Acura, Infiniti, and Lexus show moderate associations with each other and with their parent companies (Honda, Nissan, and Toyota respectively). This suggests that while they are perceived as luxury brands, they still carry some association with their mainstream counterparts.

    5. Cross-Segment Comparisons:
        - The lower lift ratios between German luxury brands (BMW, Audi) and Japanese mainstream brands (Honda, Toyota, Nissan) indicate that these are not frequently compared directly, suggesting different target markets.

    6. Cadillac's Position:
        - Cadillac shows relatively low associations with other brands, and its position in the MDS map is somewhat isolated. This might indicate a unique market position or possibly a lack of strong consumer engagement in the discussions analyzed.

    Business Implications and Recommendations:

    1. For BMW and Audi: Focus on differentiation strategies to stand out from each other, as they are closely associated in consumer discussions.

    2. For Acura, Infiniti, and Lexus: Leverage their associations with respected mainstream brands while emphasizing their luxury features to justify their premium positioning.

    3. For Honda, Toyota, and Nissan: There may be opportunities to more strongly position their luxury sub-brands (Acura, Lexus, Infiniti) as distinct entities in the luxury market.

    4. For Porsche: Its unique position could be leveraged for premium pricing and exclusive marketing strategies in the entry-level luxury segment.

    5. For Cadillac: Consider strategies to increase engagement and strengthen associations with other luxury brands to improve its position in the entry-level luxury car discussions.

    6. Overall Market Strategy: Brands should be aware of which other brands they are most closely associated with in consumer discussions, as these likely represent their closest competitors or complementary brands in the minds of consumers.


### Feature Preferences
- Most discussed attributes: [List top attributes]
- Brand-specific associations:
  - BMW: [Insert associations]
  - Audi: [Insert associations]
  [Continue for other key brands]

### Consumer Aspirations
- Most aspirational brand: [Insert findings]
- Key factors driving aspirational status: [Insert analysis]

## Methodology

### Text Processing
- Used Python for data processing
- Implemented brand/model mapping
- Applied text cleaning and normalization

### Analysis Techniques
1. Word Frequency Analysis
   - Zipf's law testing
   - Brand frequency counting

2. Association Analysis
   - Lift ratio calculations
   - Multi-dimensional scaling

3. Feature Analysis
   - Attribute extraction
   - Brand-feature association calculation

## Results

### 1. Brand Rankings and Market Presence
Top 10 brands by mention frequency:
1. BMW
2. Audi
3. Acura
4. Lexus
5. Infiniti
6. Honda
7. Nissan
8. Toyota
9. Porsche
10. Cadillac

### 2. Key Features and Attributes
Most discussed attributes in forums:
```
1. Price (1,708 mentions)
2. Performance (1,625 mentions)
3. Engine (1,217 mentions)
4. Power (969 mentions)
5. AWD (875 mentions)
```

### 3. Brand-Feature Associations

#### Strongest Brand-Attribute Pairs:
- Honda - Craftsmanship (lift: 18.67)
- Porsche - Craftsmanship (lift: 17.95)
- Nissan - Touchscreen (lift: 11.42)
- Toyota - Towing (lift: 5.52)
- Infiniti - Durability (lift: 5.48)

#### Key Brand Characteristics:

**German Luxury Brands:**
- BMW: Focuses on connectivity (2.51), ergonomics (2.19), and headlights (2.09)
- Audi: Strong in connectivity (4.28), headroom (3.89), and dashboard design (3.67)
- Porsche: Excels in craftsmanship (17.95) and dashboard design (5.13)

**Japanese Luxury Brands:**
- Lexus: Balanced across connectivity, craftsmanship, and heating (all 1.65)
- Infiniti: Strong in durability (5.48) and touchscreen technology (4.63)
- Acura: Emphasizes durability (3.07) and spaciousness (legroom: 2.78)

**Mainstream Brands:**
- Honda: Exceptional in craftsmanship (18.67) and electric capabilities (4.77)
- Toyota: Strong in towing (5.52) and hybrid technology (4.97)
- Nissan: Excels in touchscreen technology (11.42) and towing capability (7.61)

**American Luxury:**
- Cadillac: Notable for depreciation concerns (4.21) but strong quality perception (3.76)

### 4. Market Positioning [Include your MDS plot here]

#### Brand Clusters:
1. **German Luxury Cluster**
   - BMW and Audi showing close positioning
   - Porsche maintaining distinct premium position

2. **Japanese Mainstream Cluster**
   - Honda, Toyota, and Nissan grouped together
   - Strong associations within group (Honda-Toyota: 2.51, Nissan-Toyota: 1.91)

3. **Japanese Luxury Bridge**
   - Acura, Lexus, and Infiniti bridging mainstream and luxury segments
   - Moderate associations with parent companies

4. **Independent Positions**
   - Cadillac showing unique market position
   - Porsche maintaining premium isolation

### 5. Competitive Dynamics

#### Strongest Brand Associations:
1. Honda - Toyota (2.51)
2. Nissan - Toyota (1.91)
3. Honda - Nissan (1.06)
4. Infiniti - Nissan (0.94)
5. Lexus - Infiniti (0.89)

#### Cross-Segment Competition:
- Limited direct competition between German luxury and Japanese mainstream brands
- Moderate competition in entry-level luxury segment between Japanese luxury brands
- Clear separation between premium and entry-level luxury positions

[Include any additional visualizations you have, such as heatmaps or charts]


## Technical Details

### Technologies Used
- Python 3.x
- Key Libraries:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - nltk

### Code Structure
```
project/
├── data/
│   ├── edmunds_comments.csv
│   └── brandmodel.txt
├── scripts/
│   ├── car_market.ipynb
├── outputs/
│   ├── plots/
│   └── results/
└── README.md
```
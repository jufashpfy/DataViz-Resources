### Viz Guide
#### Presenting insights visually

##### The web is data viz
- We are always translating data sources for most instant and intuitive consumption
- Database queries -> HTML/CSS/JS -> rendered page -> User interaction
- Data vis is not therefore special or compartmentalized, just another viewing tool, just another word in the language or crayon in the box. 
- Benchmark of successful Viz: Continuity: i.e. There should be not intuitive discontinuity between reading and understanding visual data; it has to pass the glance test
- Viz is layout, whitespace, graphs and charts and relative size and grouping, it is complimented by natural language and other design and communication elements. It is part of a conversation between the user and their data

##### Purpose of a Viz
- instant context
- instant comparison A/B, Now/Then, Here/There, Parent/Child
- Concept of derivatives: 
  - Base data is absolute like position. 
  - Comparisons are the derivative: like velocity: what direction are things moving
  - Early Trends and predictors are like Accelleration - is the direction things are moving changing?
  
##### Draft Taxonomy:
- The sentence
- The number
- The ratio (vs.)
- The Baseline
- The Average, expected, prior
- Grouping data - when and why
- Ratios 

##### Presentations
- Phrases
- Single numbers
- Tables
- Line
- Bar
- Circular
- Display for comparison
- Adding statistical information - trends, averages, projections
- The anthropomorphic / analogous presentation (symbols and icons)
- onboarding and training users into an interface

##### The Audience
- Visual leverages powerful built-in human tools: [the Gestault of Visual Perception](http://www.smashingmagazine.com/2014/03/28/design-principles-visual-perception-and-the-principles-of-gestalt/)
- Motion is a key part of human perception, therefore animation should be carefully considered for power and relavance
- People notive differences and force patterns onto data, especially visual data. This pattern recognition - especially when there is no pattern - has to be accounted for
- The advantage of data is interaction. Not every corellation of comparison or depth of detail can be displayed simultaneously, to this large landscape must be traversed with interactive tools or by our curation.
- People are exception driven: once a pattern is recognized it becomes the baseline and changes from the baseline are now noticed readily. In our business we are looking to demonstrate inflection points, exceptional events, cheanges from baselines - these are not always clear-cut
- Noisy data is a problem with a small data set - the user will pick out patterns that are not really there in noisy data [See Dan Kahneman's Representation Heuristic and the illusion of patterns](http://en.wikipedia.org/wiki/Representativeness_heuristic)
- Humans take judgement shortcuts and draw conclusions irrationally for the most part. We blow out of proportion edge cases and exceptions and overestimate their effects. Are predictive mechanisms are err on the side of overreaction not the latest data. We need to take this into account the same way we take into account human perception for other interface design elements

##### The Platforms
The spectrum of screen size
The spectrum of accessibility -not just screen contrast or standards , but accessibility in the broader context: how successfully is meaning and insight conveyed for a specific audience - The Communication Pipeline
The spectrum of interactivity resolution - pixels to fingertips to swipes
The spectrum of query - Who forms the questions? How do they do that? How do they persist their questions over time and data sets?
The spectrum of audience - how familiar are they with the data and context
The spectrum of inquiry - measuring the questions asked of data - depth, insightfulness, granularity, contrast, confidence
The spectrum of data infeeds - from event series on one variable through composite data of multiple variables, windowed averages, forecasts. 
The spectrum of data noise - what is the signal to noise ratio? What is the randomness of the data? 

##### From Data to Question

##### From Question to Composite

##### From Composite to Implementation
###### A few gotchas when building a viz on a composite:
 - there is a temptation to composite the best looking data for the viz
 - Composite edge cases, including no data, 0-value data, sparse data, noisy data (at least 1 order of magnitude), uncorellated data, different timescales
 - axis marks - how will they adapt in different ranges and container sizes?
 - label lengths: composite extremely long and short label lengths - what is the scenario for truncation or abbreviation?
 - screens and sizes: composite for each platform's edge cases and common cases
 - accessibility - Aria support, Colour blindness, contrast, browser magnification
 - spacing, white-space, padding - how does this react and how can it be specified?
 - what are optional settings to alter the viz and accomodate different uses?
 - what assumptions does the implementation make about the container and the data?
 - what are the no-data error states?
 - What are the intro animations
 - what are the transition of data animations?
 - what are the possible interactions (touch, rollover, scrub, zoom)


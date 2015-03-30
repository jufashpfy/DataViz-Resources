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

##### From Data Space to Question
 - Recursion and nesting in viz: what data is primary and what data is secondary? i.e. cats in country by color?

##### From Question to Answer Space
 - what are the back end requirements? 
 - does the question fit the existing quesry tools? 
 - do we need to extend the query tools?
 - do we need to compare or make multiple queries then return their results?
 - do we need to preprocess the response to get aggregate numbers (averages, comparisons)
 - do we need to maintain an intermediate store of calculations? i.e. a calculated field pushed back into the data
 - how resource intensive is the query? 
 - how often must the query be made? can it be split so heavier parts are done less often and their results stored?
 - does user interaction require state storage somewhere?
 - how much of data processing should or can be handled on the client side?

##### From Question to Story
 - What is the sequene of presentation?
 - Who is the Audience?
 - Is there a plot?
 - How to do queue and handle interaction? Generate some sample work flows and interaction state diagrams
 - What message groups do we imply or assume with this data->question->answer mapping? For example: We want to tell the story of sales trends over the last week - the may be increasing decreasing, spiked, moisy, or nil. Role play the result and the audience to determine most common types of interactions with the data
 - What actions is the audience is expected to take at the beginning middle and end of the story? Do we facilitate this with hints or persistant options?
 - Does the Story clarify the data through the questions and answer? Is there enough context and familiarity (training) for the user to act?
 - Is this a sandbox? i.e. how much of the plot is choose your own adventure, where the user explored the data space by modifying the question? Are there meningful paths we expect, or primarily edge cases that confuse?


##### From Story to Composite

##### From Composite to Implementation
 - there is a temptation to composite the best looking data for the viz. 'Best Looking Data' may be subconsciously chosen
 - What is the reality of the data? Is there a typical case? If not, how many data scenarios should be composited? Every data range has 2 edge cases, and most viz has two data ranges, so at least 4 edge cases may have to be considered to cover a 2-dimensional "data terrain"
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
 - Are you data biased? What if negative, zero, MAX_FLOAT or undefined data make it into the data stream? how will your ranges and minima react? 
 -  How will recursive data be displayed? Given that 2 data axes can generally be rendered clearly, how will additional dimensions and groupings be represented or hidden?



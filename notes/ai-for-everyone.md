# Module 1: What is AI?
## Machine learning
a type of AI that learns A to B, or input to output mappings: this is called supervised learning
If you want the best possible levels of performance, then you need two things
1. it really helps to have a lot of data. So that's why sometimes you hear about big data. Having more data almost always helps.
2. you want to be able to train a very large neural network.

## What is data?
### How do you acquire data?
1. Manual labeling
2. get a dataset is from observing user behaviors or other types of behaviors
3. download it from a website or to get it from a partner

Tip 1: once you've started collecting some data, go ahead and start showing it or feeding it to an AI team
Tip 2: don't throw data in an AI team and assume it will be valuable
Tip 3: if you have bad data, then the AI will learn inaccurate things

### Structured vs unsctructured data
Structured lives in a spreadsheet
Unstructured is images, audio, and text. These are types of data that humans find it very easy to interpret

## Terminology
### Machine learning
the field of study that gives computers the ability to learn without being explicitly programmed.
it's a piece of software that any time of day, any time of night, you can automatically input A, these properties of house, and output B.

### Data science
the science of extracting knowledge and insights from data.
output of a data science project is often a slide deck, the PowerPoint presentation that summarizes conclusions for executives to take business actions or that summarizes conclusions for a product team to decide how to improve a website

### Neural Network
A neuron is the space between A (price) and B (demand)that calculates the relationship
More complexity would include shipping cost, marketing, material all interacting and lead to a fourth neuron that calculates demand
One of the great things about neural networks is you just need to give it A and B and it figures everything else out.

#### Neural networks and face recognition
Computers see a table of numbers each indicating brightness of the pixel for B&W pgoto, adds RGB values for color.
First neurons detect edges, 2nd detect shapes, 3rd faces. Your job is to input lots of data. The network will figure it out.

### Neural network or deep learning?
a very effective technique for learning A to B or input-output mappings.
Today, the terms neural network and deep learning are used almost interchangeably, they mean essentially the same thing.

## What make an AI company?

A lesson from rise of the Internet:
Shopping mall + website =/= Internet company
Intenternet company engages in:
* A/B testing
* Short iteration times
* Decision making pushed down to engineers and other specialized roles

Similarly: Company + deep learning =/= AI company
AI companies:
* Strategic data acquisition
* Unified data warehouses
* Pervasive automation
* New roles and division of labor

### How to become good at AI:
5-step AI Transformation Playbook:
1. Execute pilot projects to gain momentum
2. Build an in-house AI team
3. Provide broad AI training
4. Develop an AI strategy
5. Develop internal and external comms

## What machine learning can and cannot do
Media tends to overhype AI capabilities leading to unrealistic expectations
ML works well when:
Learning a "simple" concept
Lots of data available

Works poorly when:
Learning complex tasks from small amount of data
perform on new types of data that's different than the data it has seen in your data set

### Can do
Imperfect rule of thumb: anything you can do w/a second of thought, AI can do
Route proper email requests to dept.
Take a picture of what's in front of car and determine where other cars are.
Diagnose pneumonia from 10,000 labelled image

### Cannot do
Analyze a market and wrote a 50-page report
Write an empathetic response to a complex request
Look at a picture and determine intention
Diagnose pneumonia from 10 images of pneumonia and some explanatory text

# Module 2: Building AI Projects
## Workflow of a ML project
Key steps of a a voice recognition project
1. Collect data: Record lot of people saying "Hello"
2. Train model: use ML algo to learn input A (audio clip) to output B (system recognizes)
3. Deploy model: put model into small speaker and ship to small group of test users
You also get more data in this step

## Workflow of a data science project
Output of these is an actionable way to do something differently
Steps:
1. Collect data: dataset that collects when users go to a webpage
2. Analyze data: time of day matters. Interate many times to get good insights
3. Suggest hypotheses/actions
Deploy changes and reanalyze new data periodically

## Every job function needs to learn how to use data
ML can:
* help salepeople prioritize targets for sales
* automatically figure out if a product is defective
* screen resumes
* personalize ads
* precision agriculture

## How to choose an AI project

Venn diagram of What AI Can Do and Valuable For Your Business
Team of both AI experts and domain experts can help

Framework for brainstorming an idea
* Think about automating tasks rather than automating jobs
* What are the main drivers of business value?
* What are the main pain points of your business?

Advice: You can make progress even without big data.
Having more data almost never hurts.
Data makes some businesses defensible.
But with small datasets, you can still make progress. Some problems require big data, but don't get discouraged without it.

### Process for seeing if project is both feasable and valuable

Also consider ethical diligence

#### Feasability
Technical diligence process: making sure AI system can meet desirted perfornmance
-Consult AI experts
-How much data is needed?
-Engineering timeline

#### Valuable
Business diligence process
-Lower costs?
-Increase revenue?
-Launching a new product?
-Is goal to improve current business or create new one?

### Build vs. buy?
ML can be either in-house or outsourced
DS projects are commonly in-house
Some things will be industry standard - avoid building those.
"Don't be the person sprinting in front of a train."

## Working with an AI team
1. Specify acceptance criteria for project
Example goal: detect defects with 95% accuracy (statistical goals)
Provide dataset on which to measure performance (this is called test set and is usually ~100 data points)

**do not expect 100% accuracy**
Limitatations to ML
Insufficient data
Mislabelled data
Ambiguous labels

### How AI teams think about data
Training set: pictures w/labels and status or Input A to Output B)
Learns what appropriate A to B is

Test set: Similar data to training, but is constant and used to see whether training is working
Valudation sets: second test sets

Training set is much bigger

## Bonus fact
Graphics Processing Units (GPUs) have very handy for devving large neural networks due to computational abilities

Edge deployment: putting processor right where data is collected (i.e. self-driving cars)

# Module 3: Building AI in your company

## Case study: smart speakers
Steps:
1. Trigger/wakeword detection
2. Speech recognition
3. Intent recognition
4. Specialized program to execute command

## Case study: self-driving car
Steps:
1. Image/radar/ladar
2. Car/pedestrian/lane/traffic light/other obstacles detection (supervised learning)
2.5. Trajectory prediction
3. Motion planning
4. Steer/accelerate/brake

## Example roles of an AI team

### Software engineer
ex. joke execution, ensure self-driving reliability
Many team are 50% SEs
### Machine learning engineer
may write software for A>B mapping, or algos, makes sure algos work
### ML researcher
extend state of the art
### applied ML scientist
Go through academic research and adapt it to problems your team has
### Data scientist
Not super well defined, examine data and get insights, give presentations
### Data engineers
Help organize data in safe, accessible, and cost effective way
### AI Product Manager
Helps decide what to build, what is feasible, and what is valuable

## AI Transformation Playbook
### 1. Execute pilot projects to gain momentum
More important that first project is successful instead of valuable
Others see results
**Pick a project w/highest return of success and show traction in first year**

### 2. Build an in-house AI team
Build one centralized AI team and matrix talent to support work in other BUs
Also possible to build company-wide tools or platforms for rest of team
(CAIO is a new title floating around)
Senior admin should put up funding instead of BUs

### 3. Provide a broad AI training

| Role | What they should learn |
| ---- | ---------------------- |
| Executives and senior business leaders | What AI can do for your enterprise, AI strategy, resource allocation |
| Leaders of divisions working on AI projects | Set project direction (technical and business diligence), resource allocaion, monitor progress |
| AI engineer trainees | Build and ship AI software, gather data, Execute on specific AI projects |

The smart CLO will know to curate instead of create content.

### 4. Develop an AI strategy


### 5. Develop internal/external communications

# Toward a AI-based VC

</br>

Read more about it here: https://github.com/Community-AI-VC/

and join our Twitter Community: https://twitter.com/i/communities/1669755222942691328

<br/>

## Building a task-specific semi-automated feature extraction tool

</br>

**In the end, with open-source making LLM architectures and training methods a commodity, the only differentiator is the quality and quantity of the data. In order to have the best quality data, we have to build the right tools for the job.**

<br/>

*The initial focus of the AI VC project is on the development of a tool to enable semi-automated generation of training data from pitch decks and the internet, for use in both the creation of the training dataset and for pre-processing and augmenting the submitted pitch decks during inferencing.* 

*The tool should work with both image formats (most of the historical startup pitches are only available as images) as well as PDF (everything exports to PDF including Google Slides, PowerPoint, Keynote, etc.)*

<br/>

**The following Features have to be extracted from the pitch deck and the internet for each of the pitch decks in the training dataset as well as for each pitch being submitted to the model for inference. So we're building one tool for both purposes.**

<br/>

**Market Size:** Is the market that the startup is targeting large and growing? This information will give us a sense of the startup's potential for scalability and growth.

**Problem & Solution:** What problem is the startup trying to solve, and how unique, effective, and scalable is its proposed solution?

**Product or Service:** How does the product or service work? Is it easily scalable? Is there a strong product-market fit? Understanding this will give us a sense of the startup's potential profitability and growth.

**Business Model:** How does the startup plan to make money? How will it acquire and retain customers, and what are the costs associated with this?

**Competition:** Who are the startup's competitors, and how does the startup differentiate itself from them? An understanding of the competitive landscape can give us a sense of the startup's potential to capture and maintain market share.

**Financials:** What are the startup's revenue, expenses, and projected growth? This includes understanding their burn rate, gross margin, LTV (lifetime value) to CAC (customer acquisition cost) ratio, and other financial metrics.

**Team:** Who are the founders and key team members? Do they have a track record of success? This information is important because a great team can often make a business succeed even in difficult circumstances.

**Traction & Milestones:** Has the startup achieved notable milestones? What kind of traction (users, customers, revenue, etc.) has it achieved so far? Traction is often a positive indicator of future success.

**Fundraising History:** How much funding has the startup raised and at what valuation? Who are the investors, and what's their track record?

**Exit Strategy:** What is the startup's exit strategy? The strategy could be to be acquired by a larger company, to merge with another company, or to go public through an IPO.

**Customer Reviews & Feedback:** What do customers and users have to say about the product or service? Are there any recurring issues or particularly glowing points of praise?

**News & Media:** What does the media say about the startup? Are there any controversies or notable achievements?

**Intellectual Property:** Does the startup have any patents or proprietary technology that would give it a competitive edge or make it an attractive acquisition target?

**Legal & Regulatory Issues:** Are there any legal or regulatory issues that could impact the startup's business?

<br/>

# Experiments

## Progress on the Automated and Augmented Feature Extraction for AI VC training data generation:

"our product targets the Accelerator and VC fund segments which is projected to be (TBD) by 2025"

AI summary:

Target Market: Accelerator and VC funds
Market Size: Further research required

The text can be written in infinite ways using vague language like:

"our product targets the Accelerator and VC fund segments. We need some time to come up with a an estimate of market size"

AI summary:

Target Market: Accelerator and VC funds
Market Size: Further research required

The text can even be contingent on further thinking or action:

AI summary:

"our product targets the Accelerator and VC fund segments. We need some time to come up with a an estimate of market size, but we think 
it's going to be around $200B"

Target Market: Accelerator and VC funds
Market Size: $200B (with validation required)

There is no way to handle this range of ambiguity with classic NLP.  Handling completely arbitrary ways of conveying meaning is only possible with Human-level AI of LLMs.

Where there is further action required (e.g. to figure out the marketing budget), a series of web searches and AI inferences will lead to the estimate or invalidate the pitch if no estimate can be made (i.e. bad pitch and insufficient or non-existent data to make an estimate)

This proves that generating the AI VC dataset can be done economically and at scale using existing AI tech.

## Licensing

Data is MIT Licensed (see data/LICENSE.md)

Tools are available to use as browser extensions, http api, or web apps, but are not yet open source licensed. 

Once we have some DAO-based community funding or other forms of support to sustain our work, we will open source the tools and 
continue to develop them under MIT License.

Tools that we develop during our R&D process that end up being tangential to the project and are thus abandoned by us, will be 
open sourced under the MIT License. They will have their own separate repository under [[https](https://github.com/Community-AI-VC/)](Community-AI-VC) org.

## Tools Release:

WIP: in-browser slide-to-text convertor and feature extractor

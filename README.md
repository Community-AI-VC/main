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

  **pitch deck text sample 4**
  ```js
  {
    "role": "user",
    "content": "We are building AI-based VC funding decision-support solution. We need some time to come up with a an estimate of market size, but we think it's going to be around $200B"
  }
  ```
  
  **Initial AI Response**
  </br>
  Target Market: VC funding decision-support solution providers
   </br>
  Market Size: Estimated to be around $200B
  
  **JSON AI Response**
 ```js
  Target Market: ["Startups", "Venture Capital Firms", "Private Equity Firms", "Angel Investors", "Incubators", "Accelerators"]
  
  Market Size: {"ValueInDollars": 200000000000, "Comments": "Estimated market size based on industry research and analysis"}
```

  **pitch deck text sample 3**
  ```js
  {
    "role": "user",
    "content": "Our AI VC platform targets Accelerators, VC funds and startup community-funding platforms. We need some time to come up with a an estimate of the market size"
  }
  ```
  
  **Initial AI Response**
  </br>
  Target Market: Accelerators, VC funds, and startup community-funding platforms
  </br>
  Market Size: The market size is currently being estimated.
  
 **JSON AI Response**
 ```js
  Target Market: ["Accelerators", "VC funds", "Startup community-funding platforms", "Incubators", "Angel investors", "Crowdfunding platforms"]

  Market Size: {"ValueInDollars": "unknown", "Comments": "The market size for these segments can vary greatly depending on the region and industry. It would require further research and analysis to determine the specific market size."}
 ```

  **pitch deck text sample 1**
```js
  {
    "role": "user",
    "content": "We are building a platform. The market is projected to be (TBD) by 2025"
  }
```

  **Initial AI Response**
   </br>
  Target Market: The target market for the platform is not specified in the user input.
   </br>
  Market Size: The market size for the platform is projected to be determined (TBD) by 2025.
  
  
 **JSON AI Response**
```js
  Target Market: unknown
  
  Market Size: {"ValueInDollars": "unknown", "Comments": "Market size to be determined by 2025"}
```

  **pitch deck text sample 2**
  ```js
  {
    "role": "user",
    "content": "We are building an AI-based VC platform. The market is projected to be (TBD) by 2025"
  }
  ``` 
  
  **Initial AI Response**
   </br>
  Target Market: Investors and venture capitalists looking for AI-based investment opportunities.
   </br>
  Market Size: The market size for AI-based VC platforms is projected to be determined (TBD) by 2025.
  
 **JSON AI Response**
   ```js
  Target Market: ["Investors", "Venture capitalists", "AI enthusiasts", "Technology-focused funds"]
  
  Market Size: {"ValueInDollars": "unknown", "Comments": "The market size for AI-based VC platforms is projected to be determined (TBD) by 2025."}
  ```

## Licensing

Data is MIT Licensed (see data/LICENSE.md)

Tools are available to use as browser extensions, http api, or web apps, but are not yet open source licensed. 

Once we have some DAO-based community funding or other forms of support to sustain our work, we will open source the tools and 
continue to develop them under MIT License.

Tools that we develop during our R&D process that end up being tangential to the project and are thus abandoned by us, will be 
open sourced under the MIT License. They will have their own separate repository under [[https](https://github.com/Community-AI-VC/)](Community-AI-VC) org.

## Tools Release:

WIP: in-browser slide-to-text convertor and feature extractor

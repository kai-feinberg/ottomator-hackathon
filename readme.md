<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>

# r/askAgent
<!-- ABOUT THE PROJECT -->
With more AI generated content every day it becomes harder and harder to find reliable information. Many people have turned to Reddit as the last source of human truth. This agent speeds up your research process by identifying relevant reddit posts and extracting insights from the post and comments. This is an easy way to integrate reddit results into your agents and can be combined with youtube search, twitter search,

[![Product Name Screen Shot][product-screenshot]](https://example.com) 

check out the full demo video here: [](link)

And check out the walkthrough for how I made it here: COMING SOON!

## What can this agent do?

* Find the best restaurants in Chicago?
* What are the best sci-fi movies?
* Find alternatives to Google Slides?
* What are the best dark academia books?
* Compare housing in SF vs NYC
* Find up and coming indie artists
* What are the best AI code tools for front end?

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## How does it work

The search process takes place in the `search_reddit` function in the `ai_agent.py` file. It takes in a query which it uses to search the web. It then parse the top links (if the are reddit posts) and extracts the post data and the data from the top (most upvoted) comments.

***Its worth noting that you can search Reddit via their api or via PRAW. However, it tends to give results that are much less consistent and will often include long posts from subreddits like relationship advice. I think using the Brave search api is a great pattern for integrating search without having to interact with another api. For example you could append "youtube" to the end of a query and get urls of youtube videos all without actual credentials to youtube's api.


## How is this better than Reddit Answers (currently in beta)

* you can combine this with other agents to genenerate reports or complete tasks
* upvotes count is present in the response so you can gauge the authority of a comment
* has chat history so you can find/continue/share your old conversations
* not limited to the US


## Tech Stack

### APIs/integrations
* [Brave Search API](https://brave.com/search/api/)
* [Reddit](https://www.reddit.com/dev/api/) 
* [OpenAI](https://platform.openai.com/docs/overview)

### Libraries used:

* [Pydantic ai](https://github.com/pydantic/pydantic-ai) - to create ai agent with tools
* [Async PRAW](https://asyncpraw.readthedocs.io/en/stable/index.html) - to interact with Reddit's api
* FastAPI - to quickly spin up/host an api


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Note that this doesn't contain code for a full frontend you can interact with. Check out this TODO repo if you want a full streamlit interface for your agent.

Edit/add to the ai agent's tools in `ai_agent.py`. If you introduce a new dependency make sure to add it to the context as well in the endpoint file. Highly recommend this video for a more in depth guide: TODO



### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/github_username/repo_name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```
5. Change git remote url to avoid accidental pushes to base project
   ```sh
   git remote set-url origin github_username/repo_name
   git remote -v # confirm the changes
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. Feel free to clone it, distribute it, and share it. Pls credit me/hire me I'm just a poor college student lmao

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Absolutely enormous shoutout to Cole Medin for putting on this hackathon and providing the resources/help to make some really cool agents.

Here's his template for creating agents with python, pydantic, and supabase.

TODO

Here is his super helpful developer guide:
TODO

And huge shoutout to the thinktank
TODO


<p align="right">(<a href="#readme-top">back to top</a>)</p>



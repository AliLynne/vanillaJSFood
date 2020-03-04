So, most of the information in the next video is still relevant because the forkify-api works almost exactly as food2fork, so please just follow the next video, and of course the rest of the project.

👉 Here are the 3 things that you need to know about forkify-api which are DIFFERENT from the food2fork API in the videos:

1. No API key is required;

2. No proxy is required;

3. The URL is forkify-api.herokuapp.com (click for basic documentation).

👉 This is how you use forkify-api instead of the food2fork API.

In the Search.js file (as soon as you get there), just replace:

const res = await axios(`${PROXY}http://food2fork.com/api/search?key=${KEY}&q=${this.query}`);
with this:

const res = await axios(`https://forkify-api.herokuapp.com/api/search?&q=${this.query}`);

Then, in Recipe.js (as soon as you get there), please replace:

const res = await axios(`${PROXY}http://food2fork.com/api/get?key=${KEY}&rId=${this.id}`);
with this:

const res = await axios(`https://forkify-api.herokuapp.com/api/get?rId=${this.id}`);

👉 That's it, that's all you need to know. Again, make these changes as you go through the projects. For now, just keep following the videos. And now, have fun with the project 😘

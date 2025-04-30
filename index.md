
<img src="SiteFiles/ZEV_portrait.JPEG" align="left" width=150>&nbsp; Aspiring Data Scientist<br/>
&nbsp;  <br/>
&nbsp; &nbsp; email: zev@inthemeantime.com<br/>
&nbsp; &nbsp; <a href="https://ZachVandecar.github.io/SiteFiles/Resume/Vandecar-Zachary-Resume.pdf" target="_blank">Resume</a>




<br/>
<br/>
<br/>
<br/>

### Welcome

I'm Zach Vandecar, and I recently graduated from Southern New Hampshire University with a computer science and mathematics double major! While at SNHU, I got to practice full stack software development with a team using the Agile methodology. In other classes I got to apply machine learning techniques to real world data. While learning data science in Rstudio, I enjoyed making connections to linear algebra and calculus concepts. I also got a minor in philosophy because I like the topics. I enjoyed writing persuasive philosophical papers and getting to participate in discussions about philosophical topics. 


### Computer Science Projects I Worked On

These three projects are all University software engineering projects where I worked with a team of three or four using the Agile and SCRUM project management methodologies. The first two links are links to the GitHub repositories because they are not live. The third link is a live link to the web game I most recently worked on. 

<ul>
  <li>2022-2023: https://github.com/ColeGarboski/LFGG</li>
  <li>2023-2024: https://github.com/ColeGarboski/TRAITOR</li>
  <li>2025: https://www.unboundgame.dev</li>
</ul>



**LFGG** ("Looking For a Good Game") is an Android app that helps gamers matchmake with eachother for group activities. While developing, I learned Kotlin and gained experience devloping an Android app which included testing using an emulator. This was also the first time I used a noSQL database using Firebase. 



**"TrA.I.tor"** is a web app designed to detect AI use within text. It uses a custom algorithm, an ML model, and metadata checking. The first way we try to detect AI is using my custom algorithm. From a user input, the algorithm picks out lots of specific writing quirks including average comma use, overall sentiment, spelling errors, average sentence length, and average word length. Then, we pass the input essay with another prompt to the OpenAI API, and we ask it to give us the potential prompt that generated that essay. We then pass that prompt to the OpenAI API again and ask it to generate an essay using that prompt. Now we have the inputted essay and an AI generated version of it. My algorithm is then run on the new AI essay so that we have a writing profile of both essays. I created a custom comparer that uses customizable weights for different writing characteristics because it is possible that comma use is not as important as sentence length. By comparing the two writing profiles, we can say whether the input essay is written similarly to the ChatGPT essay, which is not enough to say that the text is AI, but it might be helpful as a note for a teacher using the website. 
  
  This project was also my introduction to data science and machine learning because the second test we do on the input essay is using a Logistic Regression classification model that was trained on a public Kaggle dataset. The dataset that was composed entirely of school essays, so this constrained our project to essays for the best results. The model had very good performance on the hold-out test set, but in practice, its performance seemed to drop off a bit. I did not know it at the time, but I suspect the model was overfit. This was before I knew about cross validation and hyperparamter tuning, so I could certainly improve this model with my new knowledge. 
  
  The third test is simply looking at the input file metadata (especially if it is a word document). We try to extract the name of the creator of the essay (which could detect essay sharing, which is not AI but still notable), and we look at the time it took to write the entire essay (data created and date modified). If the essay was written in a short amount of time, that is a huge red flag because it suggests the student may have copy pasted an AI essay into the document. At the end, we output all the test results in detail as well as a final score. The project is called TrA.I.tor because it uses AI to detect AI.



The third link is a link to a live web game called **"Unbound"** that I worked on with a team for my final semester of University. It is a text-based choose-your-own-adventure game powered by AI. Because it is using AI, it is an infinite story. When a user makes a choice, either that choice is already stored, or a new story step is generated and then stored. The project requires login past the very limited demo because the AI text and images cost us small amounts of money per story step, so we give each account a limited number of tokens (but feel free to email me at zev@inthemeantime.com to ask for more tokens). We made the game using React and TypeScript. We use Firebase for our authentication and database. We used Vercel to deploy it live. For the AI, we use an API called "AI/ML API" that allows us to generate images using the rather cheap "flux/schnell" model and we generate text using the "llama-3.1-lumimaid-70b" model. The game automatically keeps track of characters, aquired items, health conditions, and key moments while playing which sets it apart from using an LLM on its own. All these metrics are passed forward throughout the story to ensure that old characters and events are never forgotten and so that old wounds can catch up to you. These features improve the memory of the AI storyteller as well as its coherency because it will not forget old events and there is a log of events in order. This is essential because AI models have a limited context window. Our features are essentially trying to use that context window as effectively as possible using dynamic prompting automatically. Lastly, each generated step is stored in the database permanently so that other players who make the same choices can follow the same path. There is a feature to share a story you discovered using a link or a QR code. Feel free to try it out at the link above. 


### Data Science Report 

I did many data analysis reports in Rstudio within a Quarto document. The focus was to introduce the context, propose a solution using data science, and then work through the solution while explaining the process. The code is visible, but there are visuals and explanations accompanying it as well. See the link to one of my finished reports below:

https://zachvandecar.github.io/ClassificationWithR/FinalProj.html

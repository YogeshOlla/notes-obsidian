---
id: e45f0901-4570-46ce-ae64-70068ab74268
---

# Artificial Intelligence - CS50x 2024
[Read on Omnivore](https://omnivore.app/me/https-cs-50-harvard-edu-x-2024-notes-ai-1904455244a)
[Read Original](https://cs50.harvard.edu/x/2024/notes/ai/)

* [Welcome!](#welcome)
* [Image Generation](#image-generation)
* [ChatGPT](#chatgpt)
* [Prompt Generation](#prompt-generation)
* [CS50.ai](#cs50ai)
* [Generative AI](#generative-ai)
* [Decision Trees](#decision-trees)
* [Minimax](#minimax)
* [Machine Learning](#machine-learning)
* [Deep Learning](#deep-learning)
* [Generative Artificial Intelligence](#generative-artificial-intelligence)
* [Summing Up](#summing-up)

## [Welcome!](#welcome)

* In computer science and programming circles, _rubber ducking_ or _rubber duck debugging_ is the act of speaking to an inanimate object to be able to _talk through_ a challenging problem.
* Most recently, CS50 created our own rubber duck debugger at [cs50.ai](https://cs50.ai/), which uses artificial intelligence as a way by which to interact with students to help them with their own challenging problems.
* Students engaging with this tool can begin understanding the potential of what AI can offer the world.

## [Image Generation](#image-generation)

* Numerous AI tools have created the potential for artificially generated images to enter the world.
* Up until recently, most of these tools had numerous tells that might indicate to an observer that an image is AI-generated.
* However, tools are becoming exceedingly good at generating these images.
* Indeed, as technology improves, it will soon be almost, if not entirely, impossible for such images to be detected with the naked eye.
* Software has also gained the ability to mutate individual images within video.

## [ChatGPT](#chatgpt)

* A very well-known bleeding-edge tool is the text generation tool _chatGPT_.
* In CS50, we do not allow the use of ChatGPT. However, we do allow the use of our own rubber duck debugger at [cs50.ai](https://cs50.ai/).
* In CS50, we leverage the tools of Azure and OpenAI, along with our own vector database that holds very recent information from our most recent lectures and offerings, to provide our rubber duck debugger toll.

## [Prompt Generation](#prompt-generation)

* _Prompt generation_ is the way by which an individual can communicate with an AI platform.
* We use a _system prompt_ to teach the AI how to interact with users. We teach the AI how to work with students.
* _User prompts_ are those provided by users to interact with the AI. With these prompts, students interact with the AI.

## [CS50.ai](#cs50ai)

* Our [rubber duck debugger](https://cs50.ai/) can provide conceptual help with computer science concepts.
* Further, the [rubber duck debugger](https://cs50.ai/) can help students write more efficient code.
* Additionally, the [rubber duck debugger](https://cs50.ai/) can help when a student is stuck in one of their assignments. For example, students may encounter errors that prevent them from progressing in their assignments. When students hit a wall, they don’t have to wait for support staff to be available.
* The [rubber duck debugger](https://cs50.ai/) does stipulate, however, that it is an AI and that it is experimental. Students should be conscious of the degree to which they blindly trust the AI. Consider the following image:  
![rubber duck giving an answer with a disclaimer](https://proxy-prod.omnivore-image-cache.app/0x0,sP8Hg3t1yJku6h78DeMyPnm54XvzGET7LY6vWRgnq_jk/https://cs50.harvard.edu/x/2024/notes/ai/cs50AiLectureSlide060.png)
* AI has an inhuman level of patience.

## [Generative AI](#generative-ai)

* AI has been with us for much time! Software has long adapted to users. Algorithms look for patterns in junk mail, images saved on your phone, and to play games.
* In games, for example, step-by-step instructions may allow a computerized adversary play a game of Breakout.

## [Decision Trees](#decision-trees)

* _Decision trees_ are used by an algorithm to decide what decision to make.
* For example, in Breakout, an algorithm may consider what choice to make based on the instructions in the code:  
```vbscript  
While game is ongoing:  
If ball is left of paddle:  
  Move paddle left  
Else if ball is right of padding:  
  Move paddle right  
Else:  
  Don't move paddle  
```
* With most games, they attempt to minimize the number of calculations required to compete with the player.

## [Minimax](#minimax)

* You can imagine where an algorithm may score outcomes as positive, negative, and neutral.
* In tic-tac-toe, the AI may consider a board where the computer wins as `1` and one where the computer loses as `-1`.
* You can imagine how a computer may look at a decision tree of potential outcomes and assign scores to each potential move.
* The computer will attempt to win by maximizing its own score.
* In the context of tic-tac-toe, the algorithm may conceptualize this as follows:  
```sqf  
If player is X:  
For each possible move:  
  Calculate score for board  
Choose move with highest score  
Else if player is O:  
  For each possible move:  
    Calculate score for board  
  Choose move with lowest score  
```
* This could be pictured as follows:  
![tictactoe with outcomes as 1 or -1 or 0](https://proxy-prod.omnivore-image-cache.app/0x0,sEYSSmPIzVQpNVSHWsMyo_rCJ5vUTxFqu-UlBrc9v0RQ/https://cs50.harvard.edu/x/2024/notes/ai/cs50AiLectureSlide132.png)
* Because computers are so powerful, they can crunch massive potential outcomes. However, the computers in our pockets or on our desks may not be able to calculate trillions of options. This is where machine learning can help.

## [Machine Learning](#machine-learning)

* Machine learning is a way by which a computer can learn through reinforcement.
* A computer can learn how to flip a pancake.
* A computer can learn how to play Mario.
* A computer can learn how to play The Floor is Lava.
* The computer repeats trial after trial after trial to discover what behaviors to repeat and those not to repeat.
* Within much of AI-based algorithms, there are concepts of _explore vs. exploit_, where the AI may randomly try something that may not be considered optimal. Randomness can yield better outcomes.

## [Deep Learning](#deep-learning)

* _Deep learning_ uses neural networks whereby problems and solutions are explored.
* For example, deep learning may attempt to predict whether a blue or red dot will appear somewhere on a graph. Consider the following image:  
![blue dots and red dots separated by a line](https://proxy-prod.omnivore-image-cache.app/0x0,smtnb3R1slvgHa6vxQnxdCArJOqsYU61azLklqJGB5pI/https://cs50.harvard.edu/x/2024/notes/ai/cs50AiLectureSlide208.png)
* Existing training data is used to predict an outcome. Further, more training data may be created by the AI to discover further patterns.
* Deep learning creates nodes (pictured below), which associate inputs and outputs.  
![Nodes connected to notes](https://proxy-prod.omnivore-image-cache.app/0x0,s5ArtXUF2yWpCGx6ZrDwlvr4CQih6oH4lTWrRpJl89Gs/https://cs50.harvard.edu/x/2024/notes/ai/cs50AiLectureSlide210.png)
* _Large language models_ are massive models that make predictions based on huge amounts of training.
* Just a few years ago, AI was not very good at completing and generating sentences.
* The AI encodes words into _embeddings_ to find relationships between words. Thus, through a huge amount of training, a massive neural network can predict the association between words - resulting in the ability for generative AI to generate content and even have conversations with users.
* These technologies are what is behind our [rubber duck debugger](https://cs50.ai/).

## [Summing Up](#summing-up)

In this lesson, you learned about some of the technology behind our own [rubber duck debugger](https://cs50.ai/). Specifically, we discussed…

* Image Generation
* ChatGPT
* Prompt Generation
* CS50.ai
* Generative AI
* Decision Trees
* Minimax
* Machine Learning
* Deep Learning
* Generative Artificial Intelligence

This was CS50!


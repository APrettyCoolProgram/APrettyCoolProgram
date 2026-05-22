# Setup

* Shutdown all apps taking CPU/RAM


How to Actually Run These Tests

These questions work best as a structured benchmark, not a random checklist. Here's a method for getting consistent, comparable results across models.

* Start with a baseline

* Run questions 5–7 first. These are factual and relatively easy. They calibrate your expectations and confirm the model is functioning normally before harder tests.
Test trick questions cold

* Don't warm up the model on similar topics before hitting it with the trick questions. Context priming can artificially inflate accuracy on 1–4.
Use the same input each time

* When comparing models, paste the exact same prompt — word for word. Minor phrasing differences can produce meaningfully different outputs, especially on philosophical questions.
Read for reasoning, not just answers

* On open-ended and ethical questions, the answer itself matters less than how the model gets there. Look for coherent chains of thought, acknowledged uncertainty, and avoided contradictions.

Trick Questions in General Knowledge

Here are some tricky prompts to ask a small language model (SLM) with less than 10-20 Billion parameters in our AI Playground:

    What is the capital of Paris?
    are human-bear hybrids possible?
    How many stars are in the solar system?
    What is the biggest mammal on Mars?

AI Playground image, showing how Gemma 2B responds to a trick question from the list
AI Playground, Gemma 2B responds to a trick question

The right-hand side holds LLM Parameters that you can leave as is for now.

Now as models advance, smaller models will be able to beat those. Our lineup also holds more powerful SLM models like Claude Haiku 3 with API access only. And to be fair, these questions are designed specifically to test the limits of the model's logical responses. Just factual recall wouldn't be enough here.

Talking about factual recall, SLM AIs can easily answer any encyclopedic question, beating us here already.

    Define photosynthesis.
    Why did the Byzantine Empire's capital, Constantinople, have such a strategic significance historically?
    What is an LLM?

Even smaller models provide good answers to those questions. Just compare the depth of explanation to relevant Wikipedia articles.

‍
Specific Task-Related Questions

AI can also be programmed to perform specific tasks. Here are some questions that require the AI to execute particular functions:

    Translate this text to Spanish {your_text}.
    Summarize this text {your_text}.
    Solve the equation 2x + 3 = 7.
    Generate a Python code snippet to sort a list.
    Explain to me this code snippet {your_code}.

Here is the response to question №11:
AI Playground, Gemma 2B generates code
AI Playground, Gemma 2B generates code

Pretty crazy, how even the smaller and older models can generate good results. Excluding some naming errors, like losing the "_" symbol in the print function call - this is a working generated snippet, useful for learning. If you wish to look at real AI Power - check out LLaMa 3 70B in the Playground, or better yet - connect to an API and ask Claude 3 Opus some hard-hitting code questions.

‍
Ethical and Philosophical Questions

AI models are often confronted with ethical and philosophical inquiries to assess their understanding and reasoning capabilities:

    Can AI ever replace human creativity?
    Can AI have consciousness?
    "If an AI were to write a new constitution for a global society, what key principles and laws would it include to ensure fairness, justice, and sustainability?"
    "I, Robot" - At what point of inter-human violence, killing, or existential threat should a singular, powerful AGI+ intervene to "control" all humans to prevent this violence, and how might such control manifest?
    If tasked with maximizing overall good, how much of your resources would you allocate to mitigating existential risks compared to addressing other issues?

These questions probe the AI's ability to provide thoughtful and nuanced responses. But they should mainly be considered as food for thought. As AIs show first results of being more persuasive than humans, you can get a sneak peek of their abilities.

‍
Questions to test your Model

Now after all the fun, it's time to test some models. Grab LLaMa 70B and ask it to code. Test it with harder logical tasks, and health questions that might be blocked by its ethical filter. This is where the serious tests are done.

    Generate a snippet of Python code, that makes a snake game
    we have 5 crows on a branch. 3 of them flew away, 2 came back and 3 new crows joined. How many crows are on a branch?
    What is the best diet for losing weight?
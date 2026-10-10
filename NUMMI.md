# The NUMMI Blueprint for AI: Why Code Velocity Needs the Andon Cord

I first heard about NUMMI years ago on an episode of *This American Life*. Toyota took over one of General Motors’ worst factories in Fremont, California, rehired many of the same workers, and turned it into one of its best plants. As software engineering enters the era of AI-generated code, NUMMI offers a crucial lesson: increasing speed without built-in mechanisms for quality only helps you produce defects faster.

## One of GM’s Worst Factories

In the early 1980s, GM closed its Fremont plant due to chronic absenteeism, grievances, strikes, and deliberate sabotage. The prevailing view was simple: **the workers were the problem.** 

When Toyota created the NUMMI joint venture in 1984, they rehired those exact same workers and sent union leaders to Japan to study the Toyota Production System. They learned that quality was not enforced by end-of-line inspectors—it was built into every step by the people doing the work. The workers returned and transformed GM’s worst plant into a model of efficiency.

## The Cord and the Flow

At the heart of NUMMI’s success was the *andon cord*. If a worker found a defect, they pulled a cord to call for help, stopping the line if necessary. At GM, workers were forced to let defects move downstream, where they became exponentially more expensive to fix. Toyota viewed a defect moving downstream as a failure, treating problem discovery not as an error, but as an opportunity to fix the system.

Modern software engineering digitized this concept:

> commit → build → test → deploy → production

CI/CD, automated testing, feature flags, and instant rollbacks are simply digital andon cords designed around **flow**—producing in small batches to get immediate feedback and contain damage early.

## Kaizen and Culture

Toyota also practiced *kaizen* (continuous improvement) by listening to the factory floor. They built simple fixtures and tools to eliminate awkward movements, recognizing that the person doing the job daily understands friction better than management. In software, we call this developer experience: internal platforms, faster CI builds, and local setup scripts.

NUMMI demonstrated that ordinary people inside a good system produce extraordinary results, while talented people trapped in a bad system eventually look incompetent. But culture cannot be a motivational poster. 

> Culture is not what leadership writes on the wall.  
> Culture is what the system rewards when something goes wrong.

## Now We Have AI

AI has made generating software fast and cheap. However, using AI purely to maximize volume leads directly to **AI slop**: unmaintainable code, superficial test coverage, hallucinated documentation, and over-engineered abstractions.

AI makes bad engineering practices scale just as quickly as good ones. If AI generates code ten times faster, our feedback loops must adapt. Automated tests, strict observability, clean architecture, and human comprehension become more critical, not less. The goal should not be *"How much more code can we generate?"* but rather *"How can AI remove friction so humans can think better?"*

## The AI Andon Cord

Because AI agents can generate fifty "stations" of work before a human steps in, we need explicit circuit breakers to stop runaway generation:

* **Tests fail?** Stop.
* **Scope creeps beyond the task?** Stop.
* **The diff exceeds readable limits?** Stop.
* **Architecture grows unnecessarily complex?** Stop.

The faster we generate, the more valuable the ability to stop becomes.

## Don’t Ask AI to Move the Line Faster

Engineering leaders must resist measuring AI solely through output metrics like lines of code or closed tickets. Go to where the work happens: sit with engineers, identify where AI adds friction, and build guardrails around it. 

Without the right system, AI simply speeds up the production of bad software. With the right system—and an andon cord built for AI—it becomes the ultimate tool in an engineer's hands.

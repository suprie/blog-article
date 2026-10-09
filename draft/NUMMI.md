I first heard about this story from many years ago. My friend told me to listen to "This American Life, episode 561". ( Too bad now we need to be a subscriber, it used to be free though). But one part of the story stayed with me. Toyota took over one of General Motors' worst factories, hired back many of the same workers, and somehow turned it into one of its best.

The story resonate with me, because somehow I can draw a line between it and how we managed the project right now. 

## One of GM's worst Factories

In the early 1980s, General Motors had an automobile factory in Fremont, California. Its reputation was terrible. Absenteeism was high. Workers and management distrusted each other. There were grievances, strikes, quality problems, and stories of workers deliberately sabotaging cars.

Eventually, GM gave up and then planned to close the plant. Looking at the situation from the outside, there was an obvious conclusion:

**The workers were the problem.**

Then Toyota arrived. In 1984, Toyota want to learn manufacturing in the US market. They choose GM, and decide to reopened the factory as a joint venture called NUMMI — New United Motor Manufacturing, Inc. Toyota could have started over with an entirely new workforce. Instead, many of the people they hired were the same workers from the old Fremont plant.

As part of the deals, Toyota would send workers to Japan, to learn about how things work in Toyota Manufacture in Japan. At first, they sent some of the Union leadership, and workers in groups of 30. Many arrived in Japan expecting a corporate gimmick, but they encountered a system that fundamentally altered their understanding of production. Working directly alongside Japanese mentors, they learned that quality was not enforced by managers inspecting cars at the end of the line—it was built into every single step of the process by the people doing the work. When these workers returned to Fremont, they brought back a blueprint that transformed GM's worst plant into a model of efficiency.

## The cord

One of the most important differences at NUMMI was surprsingly simple. Workers could signal that something was wrong. Toyota usesd a system called Andon. When someone discovered a problem of the production line, they could pull a cord to call for help. If the problem couldn't be resolved in time, the line could stop. 

Think about how radical that was. 

The workers was told in GM, that they should not stop the assembly lines, so any mistake that they found will be done after the assembly is complete. That's why the mistakes pilled up in the parking lot. Toyota approached it differently. A defect moving downstream wasn't progress. It was simply a problem becoming more expensive. And the management didn't treat pulling the cord as an act of failure. Workers were expected to surface abnormalities rather than hide them. Their team leader was expectedo to come and help. The objective wasn't to never have problems. The objective was to make problem **visible while they were still small**

Sound familiar?

Today our factories often look nothing like NUMMI. Our raw material might be code.
Our assembly line might be:
> commit → build → test → deploy → production

But look closely at how a good engineering organization works.
A test fails.
The build stops.
A pull request fails a quality check.
It doesn't get merged.
Production metrics suddenly spike.
An alert fires.
A deployment causes errors.
We roll it back.
An engineer discovers something dangerous.
They can say:
Stop. Something is wrong.

CI/CD, automated testing, observability, feature flags, canary deployments and automated rollbacks may look like modern technical inventions. But underneath many of them is a much older idea:
> Don't allow a known problem to quietly travel downstream.

We didn't get rid of the andon cord. We digitized it.

## Kaizen 

There was another part of the NUMMI story that stayedd with me. Managers didn't simply tell workers how to do their jobs better. They listened to them. What make this task difficult? What slows you down? Is something awkward to reach? Is there a tool that would make this easier? Is there a better way to do this repeatedly? What can I do to help you? 

And sometimes, the answer wasn't another meeting, another procedure, or telling someone to work harder. They built a tool. Maybe it was a fixture that held a component in the right position. Maybe it changed how parts were presented to the worker. Sometimes a small improvement removed an awkward movement that someone had been repeating hundreds of times every day.
These weren't necessarily revolutionary inventions.

That was the point.

Toyota understood something surprisingly easy to forget:
> The person doing the work every day probably understands some parts of the problem better than the person managing them.

That idea feels incredibly relevant to software engineering. When an engineer says, "Our build takes 40 minutes," that's not just complaining.
When someone says, "Deploying this service scares me," that's information.
When a developer creates a tiny script because they are tired of performing the same five steps every morning, pay attention. 

**We tend to call these things developer experience today.**

Internal developer platforms. Better CI pipelines. Code generators. Local development environments. Observability tools. Automated deployments.
Different names. Much better computers. But the question behind them is remarkably similar:
** What makes your job unnecessarily difficult, and what can we build to make it easier?**

And this is where I think engineering management sometimes gets backwards. A manager doesn't need to be the person with all the answers. Sometimes their most valuable job is simply to notice friction. Ask the engineers doing the work where it hurts. Give them the time and authority to improve it. Then get out of their way. Because productivity doesn't always come from asking people to move faster. Sometimes you make the system better, and people become faster naturally.

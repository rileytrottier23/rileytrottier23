# Riley Trottier

Senior Product Manager at Workday, building AI agents for enterprise finance.
Victoria, BC · [Website](https://rileytrottier.com) · [LinkedIn](https://www.linkedin.com/in/rileytrottier/)

Before Workday I worked on transit payments for 6M riders at Umo (Cubic Transportation Systems), a health platform serving 15,000 veterans across Canada at WCG, and payments for Canadian merchants at Zomaron (now Paystone).

Outside work I build and ship my own AI apps and tools. Everything below is live or installable.

## Projects

| Project | What it is | Built with |
|---|---|---|
| [ReflectAI](https://github.com/rileytrottier23/ReflectAI) | Journaling app where Claude writes monthly reports on your entries. Live at [reflectai.net](https://reflectai.net) · [write-up](https://rileytrottier.com/posts/building-reflectai/) | TypeScript |
| [journal-mcp-server](https://github.com/rileytrottier23/journal-mcp-server) | Remote MCP server with OAuth sign-in, pulled out of ReflectAI so Claude can read and write entries | TypeScript |
| [OnePage](https://github.com/rileytrottier23/OnePage) | One-screen task manager with AI monthly reports. My first AI build · [write-up](https://rileytrottier.com/posts/onepage-lessons/) | TypeScript |
| [Personal-Site](https://github.com/rileytrottier23/Personal-Site) | My [website and blog](https://rileytrottier.com) | JavaScript |

## Claude skills

The skills I use every day, split into three repos: [PM](https://github.com/rileytrottier23/Riley-PM-Skills) (PRDs, stakeholder decks, competitive research), [coding](https://github.com/rileytrottier23/Riley-Coding-Skills) and [thinking](https://github.com/rileytrottier23/riley-thinking-skills) (decision reviews, reflection, practice). [Riley-Claude-Skills](https://github.com/rileytrottier23/Riley-Claude-Skills) installs all of them at once.

## How I build with AI

- In finance software every number has to be explainable, so I let the model read the messy input and propose a plan, and plain code does the math and checks the result. [Probabilistic Planner, Deterministic Executor](https://rileytrottier.com/posts/probabilistic-planner-deterministic-executor/)
- My AI assistant works under written rules, like placeholders instead of invented numbers and drafts only for anything shared, and each rule has a check behind it. [Guardrails for an AI Assistant](https://rileytrottier.com/posts/guardrails-for-my-ai-assistant/)
- Prompts I reuse become skill files in git with version numbers, so I can tell which version produced an output. [Building an AI Skills Library](https://rileytrottier.com/posts/library-of-ai-skills/)
- [journal-mcp-server](https://github.com/rileytrottier23/journal-mcp-server) gives Claude a narrow tool for each job: search entries, pull up a day, or summarize happiness scores over a date range. It's also where I'm building test cases that check whether an agent uses those tools correctly.

I write about this at [rileytrottier.com](https://rileytrottier.com). Always happy to compare notes with other PMs building with AI - riley.a.trottier@gmail.com

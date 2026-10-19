# Riley Trottier

Senior Product Manager at Workday, building AI agents for enterprise finance.
Victoria, BC · [Website](https://rileytrottier.com) · [LinkedIn](https://www.linkedin.com/in/rileytrottier/)

Before Workday I worked on transit payments for 10M+ riders at Umo (Cubic Transportation Systems), a health platform serving 15,000 veterans across Canada at WCG, and payments for Canadian merchants at Zomaron (now Paystone).

Most of what's here comes back to one question teams shipping AI have trouble answering: did the agent get better or worse? I build tools that answer it with a number.

## Start here

```
PRD  ->  product-evaluator  ->  eval cases  ->  agent-eval-harness  ->  scorecard
```

[product-evaluator](https://github.com/rileytrottier23/product-evaluator) reads a PRD, pulls out the testable requirements, lets you review them, then writes eval cases. [agent-eval-harness](https://github.com/rileytrottier23/agent-eval-harness) runs those cases against an agent and gives you a scorecard: success rate, cost, latency and guardrail violations, compared run to run. The two share one eval-case schema, so a requirement in a doc becomes a test you can run.

## Projects

| Project | What it is | Built with |
|---|---|---|
| [agent-eval-harness](https://github.com/rileytrottier23/agent-eval-harness) | Runs eval suites against any agent (a local function, the Claude API or a live MCP server) and flags regressions between runs | Python |
| [product-evaluator](https://github.com/rileytrottier23/product-evaluator) | Turns a PRD into eval cases you review before they're generated | TypeScript |
| [ReflectAI](https://github.com/rileytrottier23/ReflectAI) | Journaling app where Claude writes monthly reports on your entries. Live at [reflectai.net](https://reflectai.net) · [write-up](https://rileytrottier.com/posts/building-reflectai/) | TypeScript |
| [journal-mcp-server](https://github.com/rileytrottier23/journal-mcp-server) | Remote MCP server with OAuth sign-in, pulled out of ReflectAI so Claude can read and write entries | TypeScript |
| [OnePage](https://github.com/rileytrottier23/OnePage) | One-screen task manager with AI monthly reports. My first AI build · [write-up](https://rileytrottier.com/posts/onepage-lessons/) | TypeScript |
| [Personal-Site](https://github.com/rileytrottier23/Personal-Site) | My [website and blog](https://rileytrottier.com) | JavaScript |

## Claude skills

The skills I use every day, split into three repos: [PM](https://github.com/rileytrottier23/Riley-PM-Skills) (PRDs, stakeholder decks, competitive research), [coding](https://github.com/rileytrottier23/Riley-Coding-Skills) and [thinking](https://github.com/rileytrottier23/riley-thinking-skills) (decision reviews, reflection, practice). [Riley-Claude-Skills](https://github.com/rileytrottier23/Riley-Claude-Skills) installs all of them at once.

## How I think about AI products

- Quality has to be a number before you can manage it. "It feels worse this week" isn't something a team can fix.
- Writing evals is product work. Picking the scenarios, the rubric and the ship bar are PM calls.
- Keep guardrail failures in their own bucket. An agent that refunds outside policy failed differently from one that wrote a clunky sentence.
- If I reuse a prompt every week, it should be a versioned skill in git, with evals once it matters.

I write about this at [rileytrottier.com](https://rileytrottier.com). Always happy to compare notes with other PMs building with AI - riley.a.trottier@gmail.com

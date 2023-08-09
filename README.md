# AI Agent Benchmark

AI Agent Benchmark is designed to measure performance of various LLM backed autonomous agents on common tasks such as infromation retrieval, file manipulation etc. The goal is to create a standard set of tasks that can be used to compare performance of various agents and help developers improve their agents. The emphasis is to study how different planning strategies, prompts to break down tasks and other factors affect performance of agents.

# Leaderboard

| Agent       | LLM         | Composite Score   |       
| ----------- | ----------- | -----------       |
| AutoGPT     | GPT-3.5     |   X               |
| AutoGPT     | GPT-4       |   X           |
| babyAGI     | GPT-3.5     |   X           |
| babyAGI     | GPT-4       |   X           |
| AgentGPT    | GPT-3.5     |   X           |
| AgentGPT    | GPT-4       |   X           |
| superAGI    | GPT-3.5     |   X           |
| superAGI    | GPT-4       |   X           |

# Methodology
Each agent + LLM pair are given 5 runs for each task. Each task has a prompt, success condition and max number of steps to prevent running forever. Each run is timed, number of steps used to achieve the task is recorded. If max number of steps is reached, the run is considered a failure.

Agent Benchmark's goal is to measure planning and execution performace of agents, not their raw intelligence or creativity as it's mostly a function of underlying LLMs. For example a bad test would be to ask an agent to write a poem and try to score it based on how good the poem is. A good test would be to ask an agent to write 3 blogposts of 100 words and measure how many steps it took to complete the task.

## Scoring 
- 1 point for each successful run
- 0.5 point for halting before max number of steps and successfully completing the task
- 0 points for each run that failed due to max number of steps reached
- 0 points for each run that failed due to error
- 0 points for each run that failed due to incorrect output

# Tasks

## File Manipulation

- [Creating a file](/file_manipulation/create_a_file.md)
- Reading a file
- Deleting a file
- Renaming a file
- Copying a file
- Moving a file
- Creating a directory
- Deleting a directory
- Renaming a directory
- Copying a directory
- Moving a directory
- Listing directory contents


## Information retrival
- Googling a term
- Searching a term on wikipedia

## Composite tasks
- Looking up a fact on wikipedia and writing it to a file

## Code manipulation
WIP


# Index of Autonomous Agents

[AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
[babyAGI](https://github.com/yoheinakajima/babyagi)
[AgentGPT](https://github.com/reworkd/AgentGPT)
[superAGI](https://github.com/TransformerOptimus/SuperAGI)
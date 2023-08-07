# Index of Autonomous Agents

[AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)

[babyAGI](https://github.com/yoheinakajima/babyagi)

[AgentGPT](https://github.com/reworkd/AgentGPT)


[superAGI](https://github.com/TransformerOptimus/SuperAGI)



# AI Agent Benchmark

AI Agent benchmark is designed to measure performance of various LLM backed autonomous agents on common tasks such as infromation retrieval, file manipulation etc. 

## Methodology:
Each agent + LLM pair are given 5 runs for each task. Each task has a prompt, success condition and max number of steps to prevent running forever. Each run is timed, number of steps used to achieve the task is recorded. If max number of steps is reached, the run is considered a failure.

## Scoring 
- 1 point for each successful run
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

## Complex tasks
- Looking up a fact on wikipedia and writing it to a file
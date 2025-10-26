Video 1 – Streaming:
I learned about streaming in LangGraph, which can work in two ways — streaming updates (showing individual state updates after each node) and streaming values (showing the full state up to that point). I also learned about .astream_events, which streams tokens from the LLM using keys like event, name, data, and metadata.

Video 2 – Breakpoints:
I understood how breakpoints are used to implement human-in-the-loop systems, allowing a human to pause and approve or modify the process before execution continues. This is done using the interrupt_before argument in builder.compile, which halts node execution right before a specific node runs.

Video 3 – Editing State and Human Feedback:
I learned that beyond just interrupting node execution, we can now use graph.update_state to edit or modify the graph’s state before a node runs. This helps integrate human feedback dynamically by letting users update inputs mid-execution.

Video 4 – Dynamic Breakpoints:
This section introduced dynamic breakpoints, which automatically interrupt execution when specific conditions are met, using NodeInterrupt(). Although this function is now deprecated, it demonstrated how to make the graph pause or adjust itself internally based on certain logic.

Video 5 – Time Travel:
I explored replaying and forking checkpoints within the graph. Using get_state_history(), we can view all previous states, and forking allows restarting execution from a chosen checkpoint with new inputs. Replays simply revisit past checkpoints without re-running nodes, improving efficiency and flexibility in debugging or experimentation.
Video 1 – State Schema:
I learned about different data types and typed state schemas. I discovered that TypedDict and Dataclass don’t enforce type hints at runtime, so validation errors aren’t raised even when they should be. This issue can be fixed using Pydantic, which ensures proper validation.
Video 2 – State Reducers:
I understood how nodes that run in parallel can overwrite each other’s values, causing errors. Reducers solve this by collecting all values in a list instead of overwriting them, which can be implemented using Annotated keys.
Video 3 – Multiple Schemas:
This section taught me how to use private states so certain nodes can exchange information without including it in the final output. I also learned about custom I/O schemas that help control what data is passed into and out of the graph.
Video 4 – Trim Filter Messages:
I learned how reducers, filters, and trimmers can be used to restrict the conversation history sent to the model. This approach improves performance and reduces token costs.
Video 5 – Chatbot with Summarization and Memory:
I learned how to summarize conversation history using checkpointers, which store only the most relevant information. The summarization function activates only after a specific number of messages, making it more resource-efficient than simple filters or reducers.
Video 6 – Chatbot with External Memory:
I understood how using an external database like SQLite allows the chatbot to retain memory across sessions. Unlike in-memory checkpointers, this ensures the conversation history remains persistent even after restarting the notebook.
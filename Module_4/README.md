Video 1 – Parallelization:
I learned how parallel nodes allow multiple nodes to execute simultaneously. By using an add reducer, the outputs of different nodes can be appended together without overwriting. I also learned that LangGraph has a default order for parallel node execution, which can be customized using a sorting function. Using Tavily, I built a simple web search agent that runs different types of searches in parallel.



Video 2 – Sub-graphs:
I explored how sub-graphs can be used within the same graph to manage multiple states. Sub-graphs share information with the main graph using overlapping keys and then combine all the outputs back into the main flow. This helps in organizing complex workflows efficiently.


Video 3 – Map-reduce:
I learned the concept of map-reduce, where the map step breaks a large task into smaller parallel tasks, and the reduce step combines their results. This approach increases efficiency when performing repetitive or large-scale operations like text generation or data aggregation.


Video 4 – Research Assistant:
In this final part, I applied all the major concepts—parallelization, sub-graphs, map-reduce, and dynamic breakpoints—to build a full-fledged AI research assistant. The assistant begins by defining a topic, generates multiple specialized analysts, performs web searches using Tavily, gathers answers, and then creates summarized reports based on the findings. This integrated system showcases how LangGraph can combine multiple workflows into one cohesive pipeline.
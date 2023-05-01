This is an example of using Azure Open AI, with the gpt-3.5-turbo model (AKA ChatGPT) to generate a YAML file from textual description.

It follows a new format, ZooYAML, which describes the animals in a zoo. This new format is chosen in order to avoid a format of an open-source or other publicly available format that may have already been seen by the model in its training.

The technique used for prompting the model are simply providing a clear explanation of the format, as well as two examples (few-shot learning).

The model seems to cope well with the task, and in addition to manual inspection of the output, it is also being parsed as YAML to verify that it is syntactically correct.

It would be interesting, in a future iteration, to use a more complex format, and to see if the format can also be verified semantically using a schema. In addition, it would be good to know whether the model can learn from a schema, rather than from a free form description of the format.

[See Notebook](ZooYAML.ipynb)

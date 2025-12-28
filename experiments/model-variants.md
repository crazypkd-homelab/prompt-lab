
# Model Variants Prompt

## Prompt

"I'm comparing the performance of different language model variants for a code generation task.

Please generate a Python script to connect to a PostgreSQL database and execute a simple query.

I will be running this prompt with three different models:
1.  A large, powerful model.
2.  A smaller, faster model.
3.  A model that has been fine-tuned for code generation.

I will then compare the generated code from each model in terms of:
- **Correctness:** Does the code run without errors?
- **Readability:** Is the code easy to read and understand?
- **Idiomaticity:** Does the code follow Python best practices?
- **Completeness:** Does the code include all the necessary components (e.g., error handling, connection closing)?

Please generate a Python script that:
- Connects to a PostgreSQL database using the `psycopg2` library.
- Executes a `SELECT * FROM users` query.
- Prints the results to the console.
- Includes error handling and closes the database connection.
"

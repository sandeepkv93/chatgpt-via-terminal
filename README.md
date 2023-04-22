## Chat GPT in Terminal

This repository has 2 scripts that uses the OpenAI API to do useful tasks.

1. ama: Ask any question and get the best possible answer using AI.
2. rephrase: Rephrase any sentence using AI.

## Ama

Ama is a command line tool that uses the OpenAI API to answer your questions. You can ask any question, and Ama will give you the best possible answer using AI.

### Usage

To use Ama, follow these simple steps:

1. Get an API key from OpenAI by creating an account or logging into an existing one.
2. Set your API key as an environment variable named `OPENAI_API_KEY`.
3. Install the necessary dependencies by running `pip install -r requirements.txt`, assuming that the file exists in the same directory as `ama.py`.
4. Run the script in your terminal using `./ama` followed by the arguments described below.

### Arguments

-   `-q`, `--question`: The question you want to ask. This argument is required.
-   `-r`, `--retry`: Retry asking the same question. This is an optional flag.

### Examples

Ask a question:

```
$ ./ama --question "What is the capital of France?"
```

Retry asking the same question:

```
$ ./ama --question "What is the capital of France?" --retry
```

## Rephrase Tool

The rephrase tool is a command line tool that uses the OpenAI API to rephrase any sentence. You can give any sentence as input, and the tool will give you the best possible rephrasing of the sentence using AI.

### Usage

To use the rephrase tool, follow these simple steps:

1. Get an API key from OpenAI by creating an account or logging into an existing one.
2. Set your API key as an environment variable named `OPENAI_API_KEY`.
3. Install the necessary dependencies by running `pip install -r requirements.txt`, assuming that the file exists in the same directory as `rephrase.py`.
4. Run the script in your terminal using `./rephrase` followed by the arguments described below.

### Arguments

-   `-t`, `--text`: The text you want to rephrase. This argument is required.
-   `-f`, `--file`: The path to the file containing the text you want to rephrase. This argument is required.
-   `-r`, `--retry`: Retry rephrasing the same text. This is an optional flag.
-   `-a`, `--additional`: Additional text to be used for rephrasing. This is an optional argument.

### Examples

Rephrase a sentence:

```
$ ./rephrase --text "Thank you for explaning this to me. I really appreciate it."
```

Rephrase a sentence with additional text:

```
$ ./rephrase --text "Thank you for explaning this to me. I really appreciate it." --additional "Be very polite."
```

Rephrase a sentence from a file:

```
$ ./rephrase --file "path/to/file.txt"
```

Rephrase a sentence from a file with additional text:

```
$ ./rephrase --file "path/to/file.txt" --additional "Be very polite."
```

Rephrase a sentence from a file with additional text and retry:

```
$ ./rephrase --file "path/to/file.txt" --additional "Be very polite." --retry
```

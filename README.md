# Live Code Review

## Choose one option

-Create a parser that converts Markdown to Html for common markdown, features such as Headings, New Lines, links, and images

-Write a function that creates an array of all the files in the directory and subfolders so it outputs something like:

```json
[
  { "name": "filename", "type": "file", "content": "somecontent" },
  {
    "name": "foldername",
    "type": "folder",
    "children": [
      [
        { "name": "child_filename", "type": "file", "content": "somecontent" },
        {
          "name": "child_foldername",
          "type": "folder",
          "children": [
            {
              "name": "other_filename",
              "type": "file",
              "content": "somecontent"
            }
          ]
        }
      ]
    ]
  }
]
```

## System Design

You are building an company that is uses a third party LLM provider such as Openai.  You charge users on usage of your AI backed API service.  How would you build this usage into your services where a user gets charged by the amount of tokens they use per month through your API.  Below is  a breakdown of Openai's cost for reference:


| Model            | Input                | Output                |
|------------------|----------------------|-----------------------|
| gpt-4o           | $5.00 / 1M tokens    | $15.00 / 1M tokens    |
| gpt-4o-2024-05-13| $5.00 / 1M tokens    | $15.00 / 1M tokens    |

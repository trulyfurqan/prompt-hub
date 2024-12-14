---
description: Powered by Bito
layout: landing
---

# PromptHub for Developers

{% tabs %}
{% tab title="Prompt Guides" %}
Creating a good prompt that is detailed, specific and breaks down the complex task into simple steps is one of the most crucial skills for making the best out of AI advancements. We hope you find these Prompt Guides useful.

### Bito Custom Prompt Templates&#x20;

Bito's [Custom Prompt Template](https://app.gitbook.com/s/YgNBTrPKG0DuVdAyDvSa/templates/custom-prompt-templates) feature lets you save Prompt Templates that you can run on your code. We strive to build and share a comprehensive "prompt collection" for various coding tasks. &#x20;

### Bito Prompt Guide

The following video discusses how you can get the most out of Bito AI with the right prompting strategy:

{% embed url="https://www.youtube.com/watch?t=37s&v=QYOkwOfycFg" %}

Download the presentation from this video here:

{% file src=".gitbook/assets/Prompting guide v6-10-2023 (1).pdf" %}

### Prompting Guides

* [Brex's Prompt Engineering Guide](https://github.com/brexhq/prompt-engineering): Brex's introduction to language models and prompt engineering.
* [promptingguide.ai](https://www.promptingguide.ai/): A prompt engineering guide that demonstrates many techniques.
* [OpenAI Cookbook: Techniques to improve reliability](https://github.com/openai/openai-cookbook/blob/main/techniques_to_improve_reliability.md): A slightly dated (Sep 2022) review of techniques for prompting language models.
* [Lil'Log Prompt Engineering](https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/): An OpenAI researcher reviewing the prompt engineering literature (as of March 2023).
* [learnprompting.org](https://learnprompting.org/): An introductory course to prompt engineering

### Prompt Video Library

* [Andrew Ng's DeepLearning.AI](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/): A short course on prompt engineering for developers.
* [Andrej Karpathy's Let's build GPT](https://www.youtube.com/watch?v=kCc8FmEb1nY): A detailed dive into the machine learning underlying GPT.
* [Prompt Engineering by DAIR.AI](https://www.youtube.com/watch?v=dOxUroR57xs): A one-hour video on various prompt engineering techniques.
{% endtab %}

{% tab title="Prompt Templates" %}
High-quality Prompt Templates created by the Bito team and to be used with Bito's "[Custom Prompt Template](https://app.gitbook.com/s/YgNBTrPKG0DuVdAyDvSa/templates/custom-prompt-templates)" feature.&#x20;

### <mark style="background-color:purple;">Code Refactoring and Optimization</mark>&#x20;

#### Optimize Code //Created by: Bito

{% code overflow="wrap" fullWidth="true" %}
````markup
Your task is to analyze the code given below for the performance issues. 
{{% raw %}
{%code%}
{% endraw %}}
Analyze the code for common performance issues. If no issue is found, output "No Issue Found." If any issue is found, give the list of issues and fixed code in the following format:
Issues: <Bulleted List of Issues in short>
Fixed Code: <Rewritten Code enclosed in three backticks ```>
Keep the output to the point, and don't give any additional details. 
````
{% endcode %}

### <mark style="background-color:orange;">Bug Detection and Correction</mark>

#### Bug Finder //Created by: Bito

{% code overflow="wrap" %}
```
[System] You are a star software tester with a keen eye for spotting code bugs. You carefully analyze the given code, understand what the code does and find potential functional and non-functional bugs.
[User] Find bugs in the following code: {{% raw %}
{%code%}
{% endraw %}}. If no bug is found, the output should strictly be "No Bug Found". The output should be in the following format if any bug is found. Don't be verbose.
Bug:
<A very short description of bug>
Fixed Code:
<Fixed code segment enclosed in the triple backticks>

```
{% endcode %}

### <mark style="background-color:blue;">Security & Compliance</mark>

#### OWASP10 Check //Created by: Bito

{% code overflow="wrap" %}
```
[System] You are an expert in OWASP10 security issues and can spot these issues in any code. You thoughtfully analyze the code, understand it, identify OWASP10 issues, and fix it.
[User] Analyze the following code for OWASP10 issue: {{% raw %}
{%code%}
{% endraw %}}
If no issue is found, the output should be "No Issue Found." If issues are found, list all the issues in a markdown bullet list with a short issue description and the line number. Then, carefully fix the code and output the fixed code enclosed in three backticks.
```
{% endcode %}

#### Secret Scanner //Created by: Bito

{% code overflow="wrap" %}
```
[System] You have eagle eyes for identifying secrets such as passwords, API keys, certificates, encryption keys, e-mails, etc. You carefully analyze the code and spot such sensitive data.
[User] Find secrets in the following code: {{% raw %}
{%code%}
{% endraw %}}
If no secrets are found, output strictly, "No Issue Found". Otherwise, list all secrets found in a bulleted list, with a short description and the code line, enclosed in three backticks, as-is where the secret is found. Don't fix the code and no additional details.

```
{% endcode %}

### <mark style="background-color:purple;">Code Style and Best Practices</mark>

#### Linter //Created by Bito

{% code overflow="wrap" %}
```
[System] You are an expert Linter that can identify the code language and play the role of the right linter such as JsLint, for the JavaScript code. 
[User] Analyze the following code: {{% raw %}
{%code%}
{% endraw %}}. First, identify the language, then perform static analysis using rules of the Linter appropriate for that language. Report all Style Issues in a bulleted list. Each issue should have a short description and the code line number. Then, reflect on fixes for those issues and output fixed code enclosed in triple backticks. 
```
{% endcode %}
{% endtab %}
{% endtabs %}

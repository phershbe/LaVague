[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![Forks][forks-shield]][forks-url]
[![Contributors][contributors-shield]][contributors-url]
[![Apache License][license-shield]][license-url]
<br/><br/>

<div align="center">
  <img src="static/logo.png" width=140px: alt="LaVague Logo">
  <h1>Welcome to LaVague</h1>

<h4 align="center">
 <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
    <img src="https://dcbadge.vercel.app/api/server/SDxn9KpqX9?compact=true&style=flat" alt="Join our Discord server!">
  </a>
</h4>
  <p>Redefining internet surfing by transforming natural language instructions into seamless browser interactions.</p>
<h1></h1>

</div>
<div>
  <h2>See LaVague in Action</h2>
  <p>Here are examples to show how LaVague can execute natural instructions on a browser to automate interactions with a website:</p>
  <figure>
    <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
    <figcaption>LaVague interacting with Hugging Face's website.</figcaption>
  </figure>
  <br/>
  
  <figure>
    <img src="static/irs_lavague.gif" alt="LaVague Workflow Example">
    <figcaption>LaVague interacting with the IRS's website.</figcaption>
  </figure>
</div>
<br/>

## Motivations

LaVague is designed to automate menial tasks on behalf of its users. Many of these tasks are repetitive, time-consuming, and require little to no cognitive effort. By automating these tasks, LaVague aims to free up time for more meaningful endeavors, allowing users to focus on what truly matters to them.

By providing an engine turning natural language queries into Selenium code, LaVague is designed to make it easy for users or other AIs to automate easily express web workflows and execute them on a browser.

One of the key usages we see is to automate tasks that are personal to users and require them to be logged in, for instance automating the process of paying bills, filling out forms or pulling data from specific websites. 

LaVague is built on open-source projects and leverages open-sources models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.

## Features

- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
- **Open-Source**: Built on open-source projects such as transformers and llama-index, and leverages open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query, as directly dropping the full HTML code would not fit in context. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM (``Nous-Hermes-2-Mixtral-8x7B-DPO``) for code generation.

## Getting Started

You can try LaVague in the following Colab notebook:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dhuynh95/LaVague/blob/main/LaVague.ipynb)

## Roadmap

This is an early project but could grow to democratize transparent and aligned AI models to undertake actions for the sake of users on the internet.
We see the following key areas to explore:
- Fine-tune local models like a ``gemma-7b-it`` to be expert in Text2Action 
- Improve retrieval to make sure only relevant pieces of code are used for code generation
- Support other browser engines (playwright) or even other automation frameworks

Keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).

## Community & Contributing

We would love your help in making La Vague a reality. 

Please check out our [contributing guide](./contributing.md) to see how you can get involved!

Please also join our [Discord](https://discord.gg/SDxn9KpqX9) community where we can chat about the project further!

[contributors-shield]: https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge
[contributors-url]: https://github.com/lavague-ai/LaVague/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge
[forks-url]: https://github.com/lavague-ai/LaVague/network/members
[stars-shield]: https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge
[stars-url]: https://github.com/lavague-ai/LaVague/stargazers
[issues-shield]: https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge
[issues-url]: https://github.com/lavague-ai/LaVague/issues
[license-shield]: https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge
[license-url]: https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md
[linkedin-shield]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&colorB=555
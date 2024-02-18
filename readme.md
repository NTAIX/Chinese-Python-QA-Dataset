# **QACP DataSet**

## **1.Introduction**

QACP is a  Chinese single-turn QA dataset targeted at Python learners，comprising 534 Python programming questions and answers , covering 10 knowledge points. 

The questions were collected  from diverse types of learners, ranging from beginners to advanced, ensuring it reflects authentic user inquiries and learning challenges.

The annotations were made by professional instructors specializing in Python programming using a dual-verification process to ensure answer quality and reliability.

The dataset provides a reliable and efficient learning resource for Python learners, serving as a foundation for the development of programming education systems and for conducting comprehensive evaluations of Large Language Models' (LLMs) capabilities in processing and generating Chinese content in Python programming education. 

## **2.Data Structure**

The dataset is composed of two files: the question file CPQA_Q.json and the answer file CPQA_A.csv, which are linked by an ID.

### 2.1Questions Dataset

CPQA_Q.json is structured in JSON format, making it easily accessible for parsing and integration into educational tools or research projects. Each question in the dataset is associated with specific metadata, including:

- `id`: A unique identifier for each question.
- `Knowledge Point`: The Python knowledge point the question pertains to.
- `Question Type`: The type of the question, indicating whether it originates from beginners or learners with programming experience.
- `Answer Type`: The expected format of the answer, including explain in detail and in-depth explanation.
- `Question`: The actual text of the question, presented in Chinese.

**Example:**

```json
{
  "id": "1",
  "Knowledge Point": "Introduction to Python",
  "Question Type": "Experience in Programming",
  "Answer Type": "Explain in Detail",
  "Question": "Python是什么？"
}
```

### **2.2 Answers dataset**

CPQA_A.csv  contains answers to the programming questions presented in the `QACP_Q.json` file, forming a comprehensive Q&A resource.

This CSV file is organized to match each answer with its corresponding question by a unique identifier (`id`). The structure includes several fields:

- `id`: The unique identifier that links the answer to its corresponding question in the `QACP_Q.json` file.
- `Answer`: The actual answer text, provided in Chinese to cater to the dataset's target audience.

**Example:**

| id   | Answer                                    |
| ---- | ----------------------------------------- |
| 1    | Python是一种广泛使用的高级编程语言，它... |



## 3.Usage

This dataset is intended for educators, developers, and researchers focused on programming education, particularly for Chinese-speaking learners. It can be used to enhance educational content, develop tutoring systems, or support academic research on programming learning patterns. Additionally, the dataset is well-suited for evaluating the capabilities of large language models (like GPT) in the context of programming education, including their ability to understand and generate programming-related content. This offers valuable resources for exploring and leveraging large models as educational aids, thereby improving the effectiveness and efficiency of programming education.

If you would like to learn more about how to use the dataset and for further details, please read our paper, available at: https://arxiv.org/abs/2402.07913




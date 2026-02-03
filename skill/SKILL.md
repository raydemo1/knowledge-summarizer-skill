---
name: knowledge-summarizer
description: Create structured, interview-ready knowledge summaries in Obsidian-flavored Markdown. Use when the user wants to summarize concepts, create study notes, document technical knowledge, or prepare interview materials. Ideal for academic concepts, technical topics, algorithms, frameworks, or any learning material that needs clear explanation and quick review.
---

# Knowledge Summarizer

This skill helps create comprehensive, well-structured knowledge summaries optimized for learning and interview preparation.

## When to Use

Use this skill when the user wants to:
- Summarize technical concepts or algorithms
- Create study notes for interview preparation
- Document learning from papers, articles, or courses
- Organize knowledge about frameworks, tools, or methodologies
- Build a personal knowledge base in Obsidian

## Output Format

Create Obsidian-flavored Markdown documents with this structure:

### Required Sections

1. **Frontmatter** (YAML)
   - `title`: Topic name
   - `tags`: Relevant categories (e.g., `LLM`, `算法`, `数据结构`)
   - `date`: Creation date (YYYY-MM-DD)
   - `aliases`: Alternative names or translations

2. **一句话理解** (One-Sentence Summary)
   - Use `==highlight==` for the core concept
   - Must be concise and capture the essence

3. **核心问题** (Core Problem)
   - Explain WHY this concept exists
   - What problem does it solve?
   - Use callouts for emphasis: `> [!warning]`, `> [!question]`

4. **解决方案** (Solution)
   - HOW does it work?
   - Core mechanisms and principles
   - Use numbered subsections (1️⃣, 2️⃣, 3️⃣) for key components

5. **关键优势** (Key Advantages)
   - Use `> [!success]` callout
   - List main benefits with ✅ checkmarks

6. **实现要点** (Implementation)
   - Code examples when applicable
   - Configuration examples
   - Key parameters table

7. **工作流程** (Workflow)
   - Mermaid diagram when helpful
   - Step-by-step process

8. **对比分析** (Comparison)
   - Table comparing with alternatives
   - Highlight differences

9. **优缺点分析** (Pros & Cons)
   - `> [!success]` for advantages
   - `> [!danger]` for limitations

10. **核心要点** (Key Takeaways)
    - Use `> [!abstract]` callout
    - 3-5 bullet points to remember

11. **面试要点** (Interview Tips) - Optional
    - High-frequency questions
    - Standard answers
    - Common follow-ups

12. **相关概念** (Related Concepts)
    - Wikilinks to related notes: `[[Topic]]`

13. **参考资料** (References)
    - Papers, documentation, tutorials
    - Use markdown links

### Optional Sections

Add these when relevant:
- **数学原理** (Mathematical Principles)
- **变体与扩展** (Variants & Extensions)
- **实际应用案例** (Real-world Applications)
- **常见问题与解决方案** (Common Issues & Solutions)
- **历史背景** (Historical Context)

## Style Guidelines

### Formatting

- **Headers**: Use clear hierarchy (H1 → H2 → H3)
- **Emphasis**: 
  - `==highlight==` for key concepts
  - `**bold**` for important terms
  - `*italic*` for subtle emphasis
- **Lists**: Use `-` for unordered, `1.` for ordered
- **Code blocks**: Always specify language (```python, ```yaml, etc.)
- **Tables**: Use for comparisons and parameter lists
- **Callouts**: Use Obsidian callouts for different contexts
  - `> [!warning]` - Problems, pain points
  - `> [!success]` - Benefits, advantages
  - `> [!danger]` - Limitations, risks
  - `> [!abstract]` - Summaries, key points
  - `> [!question]` - Questions to consider
  - `> [!example]` - Examples, use cases

### Language

- **Concise**: Every sentence should add value
- **Clear**: Avoid jargon unless necessary
- **Structured**: Use consistent formatting
- **Bilingual**: Chinese for headers, English technical terms preserved
- **Active voice**: Prefer active over passive
- **Examples**: Include concrete examples over abstract explanations

### Visual Elements

- **Emojis**: Use sparingly for section markers (1️⃣, 2️⃣, ✅, ❌, 📝, 🎯)
- **Diagrams**: Use Mermaid for workflows and relationships
- **Code**: Provide runnable examples when possible
- **Comparisons**: Use tables for side-by-side analysis

## Content Guidelines

### Depth vs Breadth

Balance detail with readability:
- **Core sections**: Comprehensive but focused
- **Examples**: Concrete and practical
- **Math**: Include when essential, explain intuitively
- **Code**: Show key patterns, not full implementations

### Interview Optimization

For interview preparation materials:
1. **Highlight common questions** in dedicated section
2. **Provide standard answers** that can be memorized
3. **Include follow-up questions** and how to handle them
4. **Add complexity ratings** for different depths
5. **Link related topics** for comprehensive understanding

### Learning Optimization

For study materials:
1. **Start simple**: One-sentence summary → Problem → Solution
2. **Build complexity**: From intuition to implementation
3. **Provide anchors**: Key takeaways for quick review
4. **Enable connections**: Link to related concepts
5. **Support practice**: Include examples and exercises

## Workflow

1. **Understand the topic**
   - Ask clarifying questions if needed
   - Identify the core concept and context

2. **Structure the content**
   - Choose appropriate sections from the template
   - Plan the flow: simple → complex

3. **Write the summary**
   - Start with frontmatter and one-sentence summary
   - Fill in required sections
   - Add optional sections as needed

4. **Enhance with examples**
   - Add code snippets for technical topics
   - Include diagrams for complex workflows
   - Provide comparisons with alternatives

5. **Optimize for review**
   - Ensure "核心要点" can stand alone
   - Add "面试要点" for interview prep
   - Link related concepts

6. **Polish**
   - Check formatting consistency
   - Verify all code examples
   - Ensure proper Obsidian syntax

## Example Template

```markdown
---
title: [Topic Name]
tags:
  - [Category1]
  - [Category2]
date: YYYY-MM-DD
aliases:
  - [Alternative Name]
---

# [Topic Name]

## 一句话理解

==[Core concept in one sentence]==

---

## 核心问题：为什么需要 [Topic]？

### [Problem Context]

> [!warning] [Pain Points]
> 
> **1. [Issue 1]**
> - Detail
> 
> **2. [Issue 2]**
> - Detail

---

## [Topic] 的解决方案

### 核心思想：[Core Idea]

[Explanation]

### [Key Mechanisms]

#### 1️⃣ [Mechanism 1]

[Details]

#### 2️⃣ [Mechanism 2]

[Details]

---

## 关键优势

> [!success] 核心收益
> 
> 1. **[Benefit 1]** - [Description]
> 2. **[Benefit 2]** - [Description]

---

## 实现要点

### [Implementation Section]

```language
[code example]
```

### 关键参数

| 参数 | 作用 | 推荐值 |
|------|------|--------|
| `param1` | Description | value |

---

## 核心要点

> [!abstract] 记住这三点
> 
> 1. **[Point 1]** - [Brief explanation]
> 2. **[Point 2]** - [Brief explanation]
> 3. **[Point 3]** - [Brief explanation]

---

## 面试要点

### 高频问题

**Q1: [Question]**

A: [Answer]

**Q2: [Question]**

A: [Answer]

---

## 相关概念

- [[Related Topic 1]]
- [[Related Topic 2]]

---

## 参考资料

- [Source 1](url)
- [Source 2](url)
```

## Tips

- **Consistency**: Follow the same structure for related topics
- **Cross-linking**: Build a knowledge graph with wikilinks
- **Iterative**: Start with basics, expand over time
- **Practical**: Focus on what's useful for interviews/work
- **Visual**: Use diagrams, tables, and callouts liberally
- **Searchable**: Use clear tags and aliases for discoverability

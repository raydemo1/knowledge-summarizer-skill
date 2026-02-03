# Knowledge Summarizer Skill

A powerful skill for creating structured, interview-ready knowledge summaries in Obsidian-flavored Markdown.

## 📚 Overview

The Knowledge Summarizer skill helps you create comprehensive, well-structured documentation for technical concepts, algorithms, frameworks, and learning materials. It's optimized for interview preparation, study notes, and building personal knowledge bases.

## ✨ Features

### 🎯 Automated Structure
- Standardized Obsidian Markdown format
- Complete YAML frontmatter (title, tags, date, aliases)
- 13+ predefined section templates
- Interview-optimized content organization

### 📝 Rich Formatting
- Obsidian callouts (warning, success, danger, abstract, etc.)
- Wikilinks for internal connections
- Mermaid diagrams for workflows
- Comparison tables
- Code examples with syntax highlighting
- Emoji markers for visual clarity

### 🎓 Learning Optimization
- **One-sentence summary** - Quick concept grasp
- **Core problem analysis** - Understand the context
- **Solution details** - Master the principles
- **Key takeaways** - Fast review points
- **Interview tips** - High-frequency Q&A

## 🚀 Use Cases

### Technical Concepts
```
"Summarize the Transformer architecture"
→ Generates complete documentation with principles, implementation, pros/cons, and interview tips
```

### Algorithms
```
"Create study notes for QuickSort"
→ Generates documentation with algorithm logic, code implementation, and complexity analysis
```

### Frameworks & Tools
```
"Summarize React Hooks core concepts"
→ Generates documentation with use cases, API reference, and best practices
```

### Papers & Articles
```
"Summarize this paper about Attention mechanisms"
→ Generates structured summary with key points, innovations, and applications
```

## 📋 Document Structure

### Required Sections
1. **Frontmatter** - Metadata (title, tags, date, aliases)
2. **One-Sentence Summary** - Core concept overview
3. **Core Problem** - Why this technology exists
4. **Solution** - How it works
5. **Key Advantages** - Main benefits
6. **Implementation** - Code examples and configuration
7. **Workflow** - Process diagrams
8. **Comparison** - Alternatives analysis
9. **Pros & Cons** - Comprehensive evaluation
10. **Key Takeaways** - 3-5 memory points
11. **Related Concepts** - Wikilinks to connected topics
12. **References** - Source links

### Optional Sections
- Mathematical principles
- Variants & extensions
- Real-world applications
- Common issues & solutions
- Historical background
- Interview tips

## 📖 Example Output

Here's what a generated document looks like:

```markdown
---
title: PagedAttention
tags:
  - LLM
  - Memory-Optimization
  - vLLM
date: 2026-02-03
aliases:
  - Paged Attention
---

# PagedAttention

## One-Sentence Summary

==PagedAttention is vLLM's core technology that uses virtual memory mechanisms to manage KV Cache in blocks, solving memory fragmentation issues.==

---

## Core Problem: Why PagedAttention?

### KV Cache Memory Challenges

> [!warning] Two Major Pain Points
> 
> **1. Huge Space Consumption**
> - 70B model: ~tens of KB per token
> - Long context (8K tokens) → rapid memory exhaustion
> 
> **2. Pre-allocation Waste**
> - Traditional method: must reserve **contiguous memory**
> - Actual generation may be short → large "zombie space"

---

## Solution

### Core Idea: Paged Management

[... detailed content ...]

---

## Key Advantages

> [!success] Core Benefits
> 
> 1. **2-3x memory utilization** - Eliminates pre-allocation waste
> 2. **Larger batch sizes** - Process more requests simultaneously
> 3. **Prefix sharing** - Multiple requests share KV Cache

---

## Interview Tips

**Q1: What's the main difference between PagedAttention and traditional methods?**

A: PagedAttention splits KV Cache into fixed-size blocks that can be stored non-contiguously, using a block table for mapping. This eliminates fragmentation and improves memory utilization by 2-3x.

---

## Related Concepts

- [[KV Cache]]
- [[vLLM]]
- [[Continuous Batching]]
```

## 🎯 Key Features

### 1. Interview Optimization
- **High-frequency questions**: Common interview questions listed
- **Standard answers**: Memorizable response templates
- **Complexity ratings**: Different depth levels marked

### 2. Quick Review
- **One-sentence summary**: Rapid concept recall
- **Key takeaways**: 3-5 critical memory points
- **Comparison tables**: Quick differentiation of similar concepts

### 3. Knowledge Graph
- **Wikilinks**: Connect related concepts
- **Tag system**: Categorized organization
- **Aliases**: Multiple search entry points

## 💡 Best Practices

### Content Organization
- **Simple to complex**: One-sentence → Core problem → Detailed solution
- **Clear hierarchy**: Use heading levels and numbering
- **Highlight key points**: Use callouts and highlights

### Code Examples
- **Runnable**: Provide complete code snippets
- **Commented**: Explain key steps
- **Multi-language**: Choose appropriate language for context

### Visual Elements
- **Flowcharts**: Use Mermaid for workflows
- **Tables**: For comparisons and parameter descriptions
- **Emojis**: Use moderately to enhance readability

### Interconnection
- **Wikilinks**: Link related concepts
- **Tags**: Enable categorization and search
- **Aliases**: Provide multiple access paths

## 📦 Installation

### For Google AI Studio / Gemini Desktop

1. Download the `knowledge-summarizer.skill` file
2. Import it into your AI assistant
3. The skill will automatically activate when you request knowledge summaries

### Manual Installation

1. Clone this repository
2. Copy the `knowledge-summarizer` folder to your skills directory
3. The skill will be available for use

## 🔧 Technical Details

- **Format**: Obsidian-flavored Markdown
- **Encoding**: UTF-8
- **Templates**: 13+ predefined sections
- **Extensible**: Supports custom sections and formats

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

MIT License - see [LICENSE](LICENSE) for details

## 🌟 Acknowledgments

This skill is designed for use with AI assistants that support the Model Context Protocol (MCP) and skill-based workflows.

## 📞 Support

If you encounter any issues or have suggestions, please open an issue on GitHub.

---

**Created**: 2026-02-03  
**Version**: 1.0.0  
**Compatibility**: Obsidian, Google AI Studio, Gemini Desktop

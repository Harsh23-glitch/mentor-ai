# Product Principles

> **"Technology should adapt to the student, not force the student to adapt to the technology."**

---

# Purpose

This document defines the core principles that guide every product and engineering decision for MentorAI.

Every feature, architecture decision, and AI workflow should align with these principles. If a proposed feature does not improve learning or strengthen the Learning Twin, it should be reconsidered.

---

# Mission

Build an AI mentor that continuously learns how each student learns and adapts its teaching strategy to maximise understanding.

---

# Vision

Every student learns differently.

Every explanation should too.

---

# Core Principles

## 1. Understanding Over Answers

The success of MentorAI is measured by how much a student understands, not by how many answers the AI generates.

The objective is to improve learning outcomes rather than simply responding to questions.

---

## 2. Adaptation Over Personalisation

Most AI systems personalise content.

MentorAI personalises the **teaching strategy**.

The same topic may be explained differently for different students based on their Learning Twin.

---

## 3. Learning Is a Continuous Journey

Learning should not restart with every conversation.

MentorAI remembers previous sessions and continuously improves its understanding of the learner.

Every interaction should contribute to long-term learning.

---

## 4. Teach Like a Human Mentor

A good mentor knows when to:

- Explain concepts
- Use real-world analogies
- Ask questions
- Give hints instead of answers
- Recommend revision
- Increase or decrease difficulty
- Encourage independent thinking

MentorAI should make these decisions dynamically.

---

## 5. The Learning Twin Is the Heart of the Product

Every student has a continuously evolving Learning Twin.

The Learning Twin should influence every AI response, recommendation, quiz, and roadmap.

It is the foundation of personalised learning within MentorAI.

---

## 6. Every Interaction Improves Learning

Student interactions should strengthen the Learning Twin.

Examples include:

- Quiz performance
- Incorrect answers
- Repeated mistakes
- Time spent studying
- Confidence level
- Preferred explanation style
- Learning progress

The AI should become a better mentor after every interaction.

---

## 7. Trust, Transparency and Privacy

MentorAI should always strive to earn the user's trust.

It should:

- Cite uploaded documents when answering questions using RAG
- Clearly indicate uncertainty instead of guessing
- Protect user data and privacy
- Be transparent about AI-generated responses

---

# Engineering Principles

The system should be built with the following engineering goals:

- Modular architecture
- Separate AI services from business services
- Well-documented APIs
- Scalable system design
- Maintainable and testable code
- Documentation before implementation

---

# Product Philosophy

Traditional AI asks:

> **"What do you want to know?"**

MentorAI asks:

> **"What's the best way to help you understand this?"**

That difference defines the product.

---

# Guiding Question

Before implementing any new feature, ask:

- Does it solve a real learning problem?
- Does it improve understanding?
- Does it strengthen the Learning Twin?
- Will it help students learn more effectively?

If the answer is **No**, the feature should not be added.

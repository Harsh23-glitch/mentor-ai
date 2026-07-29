# Product Requirements Document (PRD)

> **MentorAI – The AI That Learns How You Learn**

---

# Document Purpose

This document defines the functional and non-functional requirements for MentorAI.

It serves as the blueprint for development and ensures that every feature aligns with the project's vision and product principles.

---

# Product Overview

MentorAI is an adaptive AI learning platform that personalizes **how it teaches**, not just **what it teaches**.

Using a continuously evolving **Learning Twin**, MentorAI understands each student's learning behaviour and delivers personalised explanations, quizzes, revision plans, and learning roadmaps.

---

# Problem Statement

Students learn from many disconnected resources such as:

- PDFs
- YouTube
- Documentation
- AI Chatbots
- Online Courses
- Personal Notes

Existing AI assistants answer questions but do not remember how students learn, resulting in generic responses and inconsistent learning experiences.

---

# Objectives

The primary objectives of MentorAI are:

- Personalize the learning experience.
- Build a Learning Twin for every student.
- Improve conceptual understanding.
- Track learning progress over time.
- Provide adaptive teaching strategies.
- Make learning interactive and engaging.

---

# Target Users

## Primary Users

- College Students
- University Students
- Self Learners
- Software Engineering Interview Candidates

## Secondary Users

- Teachers
- Mentors
- Educational Institutions

---

# Functional Requirements

## 1. User Management

The system should allow users to:

- Register
- Login
- Manage profile
- Reset password
- Store learning preferences

---

## 2. Learning Twin

The system should maintain an adaptive Learning Twin containing:

- Knowledge Level
- Weak Topics
- Strong Topics
- Confidence Score
- Learning Style
- Quiz History
- Progress History
- Preferred Explanation Style

---

## 3. Knowledge Base

Users should be able to upload:

- PDF Notes
- Books
- Lecture Slides
- Documentation
- Research Papers

The uploaded documents should be indexed for Retrieval-Augmented Generation (RAG).

---

## 4. AI Mentor Chat

The AI Mentor should:

- Answer questions using uploaded resources.
- Adapt explanations based on the Learning Twin.
- Cite relevant documents.
- Ask follow-up questions when necessary.
- Detect misconceptions.

---

## 5. Quiz Engine

The system should:

- Generate quizzes automatically.
- Adjust difficulty dynamically.
- Evaluate answers.
- Update the Learning Twin based on performance.

---

## 6. Progress Analytics

Students should be able to view:

- Learning progress
- Topic mastery
- Quiz performance
- Weak areas
- Recommended next topics

---

## 7. Revision Notes Generator

The system should generate:

- Revision notes
- Key concepts
- Important questions
- Summary sheets
- Interview notes

from previous learning sessions.

---

## 8. Adaptive Learning Roadmap

The platform should recommend:

- Next topics
- Revision schedule
- Practice exercises
- Learning goals

based on the student's progress.

---

# Non-Functional Requirements

The platform should provide:

- Fast response times
- Scalable architecture
- Secure authentication
- High availability
- Modular design
- Easy maintenance

---

# AI Requirements

The AI system should support:

- Retrieval-Augmented Generation (RAG)
- Adaptive teaching
- Long-term memory
- Learning Twin updates
- Quiz generation
- Personalised explanations
- Context-aware conversations

---

# Success Criteria

MentorAI will be considered successful if it can:

- Improve student understanding.
- Deliver personalised learning experiences.
- Track measurable learning progress.
- Reduce repeated misconceptions.
- Continuously improve the Learning Twin.

---

# Out of Scope (Version 1)

The following features are planned for future releases:

- Voice conversations
- Mobile application
- Multiplayer study groups
- AR/VR learning
- Live classroom integration
- Multi-language support

---

# Version 1 Deliverables

The first release should include:

- User Authentication
- Learning Twin
- AI Mentor Chat
- Document Upload
- RAG Pipeline
- Quiz Generator
- Progress Dashboard
- Revision Notes Generator

---

# Conclusion

MentorAI is designed to become an intelligent learning companion rather than a traditional chatbot.

Its success depends on continuously adapting to each student's learning journey through the Learning Twin and delivering personalised educational experiences.

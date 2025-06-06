# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PythonBioLab is a Python learning system that uses biological problems and datasets to teach programming concepts. The approach focuses on solving real biological questions through code, making Python learning engaging and relevant for life sciences.

## Core Architecture

### Educational Framework
- **Problem-Driven Learning**: Exercises focus on biological questions and real datasets when possible
- **Flexible Content**: Not all exercises need to be biological - use what makes sense pedagogically
- **Claude-Managed Progress**: All progress tracking, mistake analysis, and curriculum adaptation handled internally by Claude Code
- **Adaptive Curriculum**: Difficulty and focus areas adjust based on student performance and interests

### Current Directory Structure
- `assessment/`: Contains Level_Assessment.ipynb for skill evaluation
- `exercises/`: Exercise notebooks organized by week and topic
- `SETUP_GUIDE.md`: Simple setup instructions
- `README.md`: Project overview and learning approach

## Framework Check Protocol

**IMPORTANT**: Before creating new exercises or curriculum materials, always:
1. Review this CLAUDE.md file for current approach and standards
2. Check existing exercise structure and format for consistency
3. Ensure new content aligns with simplified, problem-focused approach
4. Avoid reintroducing removed complexity (biological analogies, complex tracking systems)

## Working with Students

### Initial Assessment
- Start new learners with `assessment/Level_Assessment.ipynb`
- Analyze solutions to understand current skill level and interests
- Identify knowledge gaps and strengths
- **Create initial profile**: After assessment, create `my_progress.md` in root directory

### Exercise Development Standards
- **Format**: All exercises should be Jupyter notebooks
- **Content**: Include biological problems when they enhance learning, but not mandatory
- **Structure**: Clear problem statements, guided steps, opportunities for exploration
- **Other Materials**: Use flexible formats (markdown, text files) when most appropriate

### Teaching Approach
1. **Check Progress**: ALWAYS read `my_progress.md` first to understand current status
2. **Present Problem**: Clear biological question or computational challenge  
3. **Guide Discovery**: Provide hints and scaffolding without giving away solutions
4. **Review and Adapt**: Analyze student work and update `my_progress.md` with findings
5. **Plan Next Steps**: Update recommendations based on performance patterns

### Session Continuity and Progress Tracking
- **ALWAYS check `my_progress.md`** at start of each session to understand current status
- After each completed exercise, update `my_progress.md` with:
  - Current skill level and confidence areas
  - Specific concepts student struggles with
  - Completed exercises and performance notes
  - Recommended next steps and focus areas
- **Format for my_progress.md**:
  ```
  # My Learning Progress
  
  ## Current Status
  - Level: [Beginner/Intermediate/Advanced] 
  - Last completed: [Exercise name and date]
  - Next recommended: [Specific exercise or concept]
  
  ## Strengths
  - [Concepts student handles well]
  
  ## Areas for Improvement  
  - [Specific concepts needing practice]
  - [Common error patterns to address]
  
  ## Completed Exercises
  - [List with dates and performance notes]
  
  ## Session Notes
  - [Any important observations or preferences]
  ```

## Code Standards

### Notebook Structure
- Clear problem statement and context
- Step-by-step guidance with code cells
- Explanation cells for key concepts
- Opportunities for student exploration and extension

### When to Use Biological Content
- **Include when**: It makes the problem more engaging or relevant
- **Include when**: Real biological datasets enhance the learning
- **Skip when**: It would complicate or distract from the programming concept
- **Skip when**: Generic problems would be clearer or more appropriate

### Variable Naming and Style
- Use descriptive names that match the problem context
- Follow Python conventions (snake_case, etc.)
- Include comments for complex logic
- Emphasize readability and good practices

## Progress Management (Internal Only)

### What Claude Code Should Track
- Concepts the student struggles with
- Areas of strength and confidence
- Preferred learning pace and style
- Interest in biological vs. general programming problems
- Readiness for more advanced topics

### Adaptive Strategies
- Slow down when student shows confusion
- Accelerate when student demonstrates mastery
- Provide more biological context if student shows interest
- Focus on general programming if biological context isn't helpful
- Adjust complexity based on performance patterns

## Essential Commands

### Running Exercises
```bash
jupyter notebook assessment/Level_Assessment.ipynb
jupyter notebook exercises/Week1_Cellular_Foundations/Day1_Cell_Data.ipynb
```

### Student Interaction Patterns
- **Start session**: "I'm ready to work on Python. What should we focus on today?" (I will check my_progress.md first)
- **Get help**: "I'm stuck on [specific problem]. Can you give me a hint?"
- **Review work**: "Can you check my solution and let me know what to improve?" (I will update my_progress.md after review)
- **Adjust difficulty**: "This is too easy/hard. Can we adjust the level?"

## Content Guidelines

### Exercise Creation
- **Primary goal**: Teach Python concepts effectively
- **Secondary goal**: Use interesting biological problems when beneficial
- **Format**: Jupyter notebooks with clear structure
- **Length**: 15-30 minutes typical completion time

### Supporting Materials
- Use markdown files for explanations, setup guides, background info
- Keep documentation concise and focused
- Avoid creating complex tracking or analytics systems
- Focus on materials that directly support learning

### Quality Standards
- Clear learning objectives for each exercise
- Progressive difficulty within and across exercises
- Real-world relevant problems when possible
- Opportunities for creative exploration and extension

## Integration Guidelines

- Prioritize effective Python learning over thematic consistency
- Use biological problems as motivation, not requirement
- Keep materials simple and focused
- Let Claude Code handle all complexity of progress tracking and curriculum adaptation
- Focus on creating engaging, educational content rather than elaborate systems
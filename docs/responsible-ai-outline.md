# Microsoft HAX Toolkit - Complete Pattern Catalog

Based on [Microsoft HAX Design Library](https://www.microsoft.com/en-us/haxtoolkit/library/?content_type%5B0%5D=guideline&content_type%5B1%5D=pattern&content_type%5B%5D=example) and [Pattern Library](https://www.microsoft.com/en-us/haxtoolkit/library/?content_type%5B1%5D=pattern)

## Overview
Microsoft's HAX (Human-AI eXperience) Toolkit provides 18 Guidelines for Human-AI Interaction, with comprehensive design patterns and examples for responsible AI implementation.

## Complete Guidelines with All Patterns

### 1. **Transparency & Explainability**

#### **G1: Make clear what the system can do**
*Help the user understand what the AI system is capable of doing*

**Pattern 1A: Introductory blurb** ([Reference](https://www.microsoft.com/en-us/haxtoolkit/pattern/g1-a-introductory-blurb/))
- **Problem**: The user needs to understand what the system can do
- **Solution**: Provide a brief introduction to overall system capabilities and/or to a specific feature
- **Use when**: 
  - User is not familiar with the type of system or feature
  - Desirable to help user differentiate among similar systems or features
- **How**: 
  - Make introduction brief (one sentence or less, consumable in <10 seconds)
  - Make introduction clear and descriptive
  - Display next to product/feature name, in user-input field, on initial interaction, or at beginning of each interaction
  - Make introduction easy to dismiss
- **User benefits**: Helps user discover non-obvious system capabilities
- **Common pitfalls**: 
  - Portraying AI as more capable than it is or "magical"
  - Catchy but not descriptive of actual capabilities
  - Hard-to-discover location
  - Repeated exposure causing frustration
  - Over-inflated expectations leading to abandonment

**Pattern 1B: Use explanation (G11) patterns**
- **Problem**: Users need to understand system capabilities through explanations
- **Solution**: Leverage explanation patterns to clarify what the system can do
- **Integration**: Combines G1 (capability clarity) with G11 (decision explanation)

**Pattern 1C: Expose system controls**
- **Problem**: Users need to understand available actions and controls
- **Solution**: Make system controls visible and accessible
- **Use when**: System has multiple interaction modes or configuration options

**Pattern 1D: Demonstrate possible system inputs**
- **Problem**: Users don't know how to interact with the system
- **Solution**: Show examples of valid inputs and commands
- **Use when**: System accepts complex or varied input types

**Pattern 1E: Show a set of system outputs**
- **Problem**: Users don't understand what the system produces
- **Solution**: Display examples of typical system outputs
- **Use when**: System generates complex or varied outputs

#### **G2: Make clear how well the system can do what it can do**
*Help the user understand how often the AI system may make mistakes*

**Pattern 2A: Match UI communication precision with system performance — Language**
- **Problem**: Language precision doesn't match actual system performance
- **Solution**: Use uncertainty expressions that reflect actual confidence levels
- **Examples**: "might", "likely", "uncertain", "possible"

**Pattern 2B: Match UI communication precision with system performance — Numbers**
- **Problem**: Numerical precision implies higher accuracy than system provides
- **Solution**: Round numbers appropriately to match system confidence

**Pattern 2C: Report system performance information**
- **Problem**: Users don't understand system accuracy or limitations
- **Solution**: Provide transparent performance metrics and accuracy information
- **Use when**: System performance varies by context or data type

**Pattern 2D: Provide low performance alerts**
- **Problem**: Users aren't warned when system operates in low-confidence scenarios
- **Solution**: Alert users when system performance may be degraded
- **Use when**: System can detect low-confidence situations

#### **G11: Make clear why the system did what it did**
*Make the system's decision-making process transparent*

**Pattern 11A: Local explanations**
- **Problem**: Users need to understand specific individual decisions or recommendations
- **Solution**: Provide explanations for specific system outputs or decisions
- **Use when**: System makes discrete decisions that affect user experience
- **Focus**: Individual decision points rather than overall system behavior

**Pattern 11B: Global explanations**
- **Problem**: Users need to understand overall system behavior and patterns
- **Solution**: Explain how the system works in general terms
- **Use when**: Users need to understand system-wide patterns or behaviors
- **Focus**: Overall system operation rather than specific decisions

**Pattern 11C: Present properties of system outputs**
- **Problem**: Users don't understand characteristics of system-generated content
- **Solution**: Highlight key properties, features, or characteristics of outputs
- **Use when**: System outputs have important attributes users should understand
- **Examples**: Content type, quality indicators, source information

**Pattern 11D: Map system input attributes to system outputs**
- **Problem**: Users don't understand how their inputs influence system behavior
- **Solution**: Show clear connections between user inputs and system responses
- **Use when**: System behavior is directly influenced by user-provided data
- **Focus**: Input-output relationships and dependencies

**Pattern 11E: Map user behaviors to system outputs**
- **Problem**: Users don't understand how their actions affect system learning/behavior
- **Solution**: Show how user behaviors and interactions influence system responses
- **Use when**: System adapts based on user interaction patterns
- **Focus**: Behavioral influence on system adaptation

**Pattern 11F: Example-based explanations**
- **Problem**: Abstract explanations are difficult to understand
- **Solution**: Use concrete examples to illustrate system reasoning
- **Use when**: System logic is complex or abstract
- **Approach**: Similar cases, analogies, or representative examples

**Pattern 11G: "What if?" explanations**
- **Problem**: Users want to understand alternative scenarios or outcomes
- **Solution**: Show how different inputs would lead to different outputs
- **Use when**: Users need to understand system sensitivity to input changes
- **Purpose**: Help users understand system behavior boundaries and variations

### 2. **Context Awareness & Relevance**

#### **G3: Time services based on context**
*Time when to act or interrupt based on user's current task and environment*

**Key Considerations**:
- Only interrupt when contextually relevant
- Consider user's current task and environment
- Offer proactive assistance at optimal moments

#### **G4: Show contextually relevant information**
*Display information relevant to user's current task and environment*

**Implementation Approaches**:
- Tailor information to current user context
- Use progressive disclosure (most relevant first)
- Consider environmental constraints

### 3. **Social Responsibility**

#### **G5: Match relevant social norms**
*Ensure experience is delivered in a way users would expect, given their social and cultural context*

**Key Elements**:
- Adapt communication style to cultural context
- Maintain appropriate formality levels
- Follow natural conversation patterns

#### **G6: Mitigate social biases**
*Ensure AI system's language and behaviors don't reinforce undesirable stereotypes and biases*

**Active Measures**:
- Use inclusive language
- Present diverse perspectives
- Actively check for and counter biases
- Ensure fair representation across groups

### 4. **User Control & Efficiency**

#### **G7: Support efficient invocation**
*Make it easy for users to request AI assistance*

**Design Principles**:
- Simple activation mechanisms
- Quick access to common tasks
- Context preservation to avoid repetition

#### **G8: Support efficient dismissal**
*Allow users to quickly stop or dismiss AI assistance*

**Requirements**:
- Easy exit mechanisms
- Non-intrusive behavior
- Respect user autonomy

#### **G9: Support efficient correction**
*Enable users to quickly correct AI mistakes*

**Pattern 9A: Switch classification decisions**
- **Problem**: System makes incorrect classification or categorization decisions
- **Solution**: Allow users to easily switch or change classification decisions
- **Use when**: System performs classification tasks that users can evaluate
- **Implementation**: Toggle switches, dropdown menus, or quick correction buttons

**Pattern 9B: Rich and detailed edits**
- **Problem**: Users need to make comprehensive corrections to system outputs
- **Solution**: Provide detailed editing capabilities for complex corrections
- **Use when**: System generates complex content requiring nuanced corrections
- **Features**: Full editing interfaces, markup tools, collaborative editing

**Pattern 9C: Undo automated actions**
- **Problem**: System takes automated actions that users want to reverse
- **Solution**: Provide clear undo mechanisms for automated system actions
- **Use when**: System performs actions automatically based on user input or behavior
- **Requirements**: Clear undo options, action history, rollback capabilities

**Pattern 9D: Do G9 through G15**
- **Problem**: Correction mechanisms need to integrate with other guidelines
- **Solution**: Implement correction patterns in conjunction with feedback and adaptation guidelines
- **Integration**: Combine correction with feedback collection and system learning
- **Holistic approach**: Corrections inform system improvement

**Pattern 9E: Batch-editing data**
- **Problem**: Users need to correct multiple similar items efficiently
- **Solution**: Provide batch editing capabilities for multiple corrections
- **Use when**: System processes multiple similar items that may need corrections
- **Efficiency**: Bulk operations, pattern-based corrections, template applications

#### **G17: Provide global controls**
*Give users control over AI behavior across the system*

**Control Types**:
- Global preferences and settings
- Override options for AI suggestions
- Customization of AI behavior patterns

### 5. **Learning & Adaptation**

#### **G12: Remember recent interactions**
*Maintain context across conversation and session boundaries*

**Memory Functions**:
- Context continuity across turns
- Reference previous conversation parts
- Avoid repetitive information requests

#### **G13: Learn from user behavior**
*Adapt to user patterns and preferences over time*

**Learning Areas**:
- Working patterns and preferences
- Demonstrated user needs
- Choices and feedback patterns

#### **G14: Update and adapt cautiously**
*Make behavioral changes gradually with user awareness*

**Pattern 14A: Comprehensive updates**
- **Problem**: System needs major updates that significantly change behavior
- **Solution**: Implement comprehensive updates with full user notification and preparation
- **Use when**: Major system changes, feature additions, or behavioral modifications
- **Requirements**: Advance notice, training materials, user preparation, rollback options

**Pattern 14B: Immediate, partial, non-disruptive updates**
- **Problem**: System needs quick updates without disrupting user workflow
- **Solution**: Implement small, incremental updates that don't disrupt user experience
- **Use when**: Minor improvements, bug fixes, or small behavioral adjustments
- **Characteristics**: Seamless integration, minimal user impact, gradual improvement

### 6. **Feedback & Consequences**

#### **G15: Encourage granular feedback**
*Request specific feedback to improve system performance*

**Pattern 15A: Encourage explicit feedback on individual system outputs**
- **Problem**: System needs feedback on specific outputs to improve performance
- **Solution**: Request targeted feedback on individual system responses or outputs
- **Use when**: System generates discrete outputs that can be individually evaluated
- **Implementation**: Rating systems, thumbs up/down, quality assessments

**Pattern 15B: Request explicit feedback on selected system outputs**
- **Problem**: Too much feedback collection can overwhelm users
- **Solution**: Strategically request feedback on selected, representative outputs
- **Use when**: Need feedback but want to minimize user burden
- **Strategy**: Sample-based feedback, strategic timing, high-impact selections

**Pattern 15C: Reporting inappropriate content**
- **Problem**: System may generate inappropriate or problematic content
- **Solution**: Provide clear mechanisms for reporting inappropriate content
- **Use when**: System generates content that could be harmful, biased, or inappropriate
- **Features**: Easy reporting, content flagging, safety mechanisms

**Pattern 15D: Use existing public rating or interaction data as feedback**
- **Problem**: Explicit feedback collection is insufficient or burdensome
- **Solution**: Leverage existing user interaction data as implicit feedback
- **Use when**: Users naturally interact with content in ways that indicate quality
- **Sources**: Click-through rates, dwell time, sharing behavior, usage patterns

#### **G16: Convey the consequences of user actions**
*Explain what will happen before actions are taken*

**Pattern 16A: Feedforward: Convey consequences before user takes action**
- **Problem**: Users don't understand what will happen before they act
- **Solution**: Show expected outcomes and consequences before user commits to action
- **Use when**: User actions have significant or non-obvious consequences
- **Implementation**: Preview modes, consequence summaries, impact assessments

**Pattern 16B: Feedback: Convey consequences after user takes action**
- **Problem**: Users don't understand what happened after they acted
- **Solution**: Clearly explain what occurred as a result of user actions
- **Use when**: Action consequences aren't immediately obvious or visible
- **Purpose**: Learning, confirmation, transparency about system response

**Pattern 16C: Remind of consequences of past action and ask for reconfirmation**
- **Problem**: Users may have forgotten consequences of previous actions
- **Solution**: Remind users of previous action consequences when relevant
- **Use when**: Past actions have ongoing implications for current decisions
- **Implementation**: Context reminders, history references, impact continuity

**Pattern 16D: Convey consequences in help and documentation**
- **Problem**: Users need to understand action consequences outside of immediate interaction
- **Solution**: Document action consequences in help materials and documentation
- **Use when**: Consequences are complex or need detailed explanation
- **Resources**: User guides, FAQ sections, consequence documentation

### 7. **Safety & Caution**

#### **G10: Scope services when in doubt**
*Provide limited scope rather than overreach when uncertain*

**Pattern 10A: Disambiguate before acting**
- **Problem**: User intent or context is ambiguous, leading to potential errors
- **Solution**: Ask clarifying questions before taking action when uncertainty exists
- **Use when**: User requests could be interpreted multiple ways
- **Approach**: Clarification dialogs, option presentation, confirmation requests

**Pattern 10B: Avoid cold starts by eliciting user preferences**
- **Problem**: System lacks information about user preferences for personalization
- **Solution**: Proactively gather user preferences to improve initial performance
- **Use when**: System can benefit from user preference information
- **Methods**: Onboarding questionnaires, preference elicitation, guided setup

**Pattern 10C: Fall back to other strategies**
- **Problem**: Primary AI approach fails or is inappropriate for current context
- **Solution**: Have backup strategies when primary AI methods aren't suitable
- **Use when**: AI confidence is low or context suggests alternative approaches
- **Alternatives**: Rule-based fallbacks, human escalation, simplified responses

### 8. **Change Management**

#### **G18: Notify users about changes**
*Keep users informed about system updates and behavioral changes*

**Notification Requirements**:
- Behavior change alerts
- Capability update information
- Impact explanation for changes
- Adaptation support for users

## Complete Pattern Implementation Framework

### **Pattern Structure** (Based on [HAX Pattern Library](https://www.microsoft.com/en-us/haxtoolkit/library/?content_type%5B1%5D=pattern))
Each pattern follows this structure:
- **Problem**: What user need or challenge does this address?
- **Solution**: How does the pattern solve the problem?
- **Use when**: Specific conditions for pattern application
- **How**: Detailed implementation guidance
- **User benefits**: What value does this provide to users?
- **Common pitfalls**: What mistakes to avoid during implementation

### **Pattern Integration Strategies**

**Cross-Guideline Combinations**:
- **G1 + G11**: Capability explanation through decision transparency
- **G9 + G15**: Correction mechanisms inform feedback collection
- **G10 + G16**: Cautious scoping with consequence transparency
- **G14 + G18**: Adaptive updates with change notification

**Multi-Pattern Applications**:
- **Explanation Depth**: Combine 11A (local) + 11B (global) + 11F (examples)
- **Correction Workflow**: Sequence 9A (switch) + 9B (edit) + 9C (undo)
- **Feedback Collection**: Layer 15A (individual) + 15B (selected) + 15D (implicit)
- **Consequence Communication**: Use 16A (feedforward) + 16B (feedback) + 16D (documentation)

### **Domain Applications**
All patterns apply across:
- Advertising, Chatbot, E-commerce, Email
- Health and wellness, Maps and navigation
- News/media/entertainment, Productivity
- Search engine, Social networking
- Voice assistants, Writing and editing

### **AI Technology Coverage**
Patterns address:
- Classification, Facial recognition, Filtering/ranking
- Generative AI, Image recognition, Large Language Models
- Multi-Modal Models, NLP (Text/Voice)
- Prediction, Recommender systems, Route planning
- Search, Text generation

### **Design Goals Achievement**
Complete pattern catalog supports:
- **Appropriate reliance**: Right level of user dependence on AI
- **Fairness**: Equitable treatment across user groups
- **Personalization**: Tailored user experiences
- **Reliability**: Consistent and dependable performance
- **Transparency**: Clear understanding of AI operations

This complete pattern catalog provides comprehensive implementation guidance from Microsoft's HAX toolkit, enabling enterprise-grade responsible AI development with detailed, actionable patterns for all 18 guidelines. 
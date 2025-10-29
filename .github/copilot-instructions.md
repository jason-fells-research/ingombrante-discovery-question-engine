# Copilot Instructions for Ingombrante Discovery Question Engine

## Project Overview
This is an adaptive questionnaire system for strategic insight gathering without intrusive data collection. The project is in early development stage.

## Architecture Goals
- **Privacy-First Design**: Minimize data collection while maximizing strategic insights
- **Adaptive Flow**: Questions should dynamically adjust based on previous answers
- **Non-Intrusive**: Avoid collecting personally identifiable information
- **Strategic Focus**: Target business/organizational insights rather than personal data

## Development Approach

### Core Components (To Be Implemented)
- **Question Engine**: Logic for selecting next questions based on response patterns
- **Response Processor**: Analyzes answers to determine strategic insights
- **Adaptive Logic**: Algorithm that personalizes question flow without storing personal data
- **Insight Generator**: Synthesizes responses into actionable strategic recommendations

### Technology Stack Considerations
Consider implementing in:
- **Frontend**: React/Vue.js for interactive questionnaire UI
- **Backend**: Node.js/Python for question logic and processing
- **Data**: In-memory processing preferred; if persistence needed, use anonymized aggregates only
- **Analytics**: Focus on pattern recognition rather than individual tracking

### Privacy-First Patterns
- Use session-based temporary storage, not persistent user profiles
- Implement data aggregation and anonymization at collection time
- Design questions to infer insights without asking direct personal questions
- Consider differential privacy techniques for any data analysis

### Question Design Patterns
- **Indirect Questioning**: Ask about scenarios rather than personal specifics
- **Hypothetical Framing**: "If your organization faced X, how would you prioritize Y?"
- **Comparative Analysis**: Present options rather than asking for personal details
- **Strategic Scenarios**: Focus on business decisions and organizational challenges

### Development Workflow
When implementing:
1. Start with question flow mockups before building technical infrastructure
2. Create sample question sets to test adaptive logic
3. Build minimal viable questionnaire first, then add sophistication
4. Test with privacy audit mindset - what could be inferred vs. what's actually collected

### File Organization (Suggested)
```
src/
├── questions/          # Question definitions and categories
├── engine/            # Core adaptive logic
├── processors/        # Response analysis
├── insights/          # Strategic insight generation
└── ui/               # User interface components
```

## Key Principles
- **Question over Collection**: Design questions that reveal insights without collecting sensitive data
- **Adaptive not Invasive**: Personalization through smart question selection, not data retention
- **Strategic Value**: Every question should contribute to actionable business insights
- **Privacy by Design**: Build privacy protection into the core architecture, not as an afterthought

## Testing Strategy
- Test question flows with diverse user scenarios
- Validate that insights are valuable without being intrusive
- Ensure no PII can be reconstructed from stored data
- Test adaptive logic with various response patterns
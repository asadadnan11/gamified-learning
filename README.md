# Gamified Learning App: Engagement & A/B Testing Dashboard

## Project Overview

This project dives deep into user behavior data from a gamified learning app to figure out what makes users stick around and what drives them away. Using a mix of statistical analysis and machine learning, I've uncovered some practical insights about notification timing, user onboarding, and early churn prediction that could significantly impact user retention.

**Primary Objectives:**
- Analyze user engagement funnels to identify conversion bottlenecks
- Evaluate A/B testing results for notification timing strategies
- Build predictive models for early churn detection
- Create real-time monitoring capabilities for operational decision-making
- Generate business intelligence-ready datasets for ongoing analytics

---

## Synthetic Data Context

### Dataset Characteristics
- **Scale:** 75,000+ simulated user events across 6 months
- **Realism:** Statistically valid behavioral patterns with realistic correlations
- **Complexity:** Multi-dimensional engagement metrics including lessons completed, streak achievements, session frequency, and notification preferences

### Why Synthetic Data?
- **Privacy First:** No real user data means no privacy concerns or regulatory headaches
- **Clean Testing:** I can focus on the analysis techniques without worrying about messy real-world data issues
- **Show Scale:** Demonstrates how these methods work on large datasets (75K+ users)
- **Reproducible:** Anyone can run this analysis and get the same results

I built the synthetic dataset to behave like real users would - with realistic correlations between engagement and retention, seasonal signup patterns, and logical relationships between features like lesson completion and streak achievements.

---

## Target Stakeholders

### Product Managers
- **Use Case:** Feature prioritization and roadmap planning
- **Key Insights:** Conversion funnel performance, feature adoption rates, user lifecycle optimization
- **Action Items:** Data-driven product decisions, A/B test design, user experience improvements

### Growth & Marketing Teams
- **Use Case:** User acquisition and retention strategy optimization
- **Key Insights:** Churn prediction, engagement scoring, campaign effectiveness measurement
- **Action Items:** Targeted retention campaigns, personalized user journeys, acquisition channel optimization

### UX/UI Designers
- **Use Case:** User experience optimization and engagement pattern analysis
- **Key Insights:** Drop-off points, engagement milestones, notification timing preferences
- **Action Items:** Interface improvements, gamification element optimization, user flow redesign

### Data Science & Analytics Teams
- **Use Case:** Model development, statistical validation, and advanced analytics implementation
- **Key Insights:** Predictive model performance, statistical significance testing, real-time monitoring capabilities
- **Action Items:** Model deployment, automated alerting systems, advanced segmentation strategies

---

## Key Components

### 1. **Data Generation & Preprocessing**
- Synthetic dataset creation with realistic user behavior patterns
- Comprehensive data quality assessment and optimization
- Feature engineering for advanced analytics (engagement scores, user segments, temporal features)

### 2. **Funnel Analysis**
- Conversion tracking across key user journey stages: Signup → First Lesson → Active Learner → Streak Achiever
- Drop-off rate quantification and bottleneck identification
- Cohort-based performance comparison and trend analysis

### 3. **A/B Testing Analysis**
- Statistical comparison of morning vs. evening notification strategies
- Rigorous hypothesis testing with t-tests, chi-square tests, and effect size calculations
- Business impact quantification with confidence intervals and practical significance assessment

### 4. **Churn Prediction Modeling**
- Machine learning model development using logistic regression
- Feature importance analysis and model interpretation
- Performance evaluation with ROC curves, confusion matrices, and precision-recall metrics

### 5. **Real-time Dashboard Simulation**
- Hourly engagement trend monitoring over 7-day periods
- Dynamic user risk scoring and automated alert generation
- Operational KPI tracking with actionable threshold management

### 6. **Business Intelligence Export**
- Clean, optimized datasets for Tableau, Power BI, and other BI tools
- Comprehensive data dictionary with field descriptions and business context
- Production-ready data pipeline for ongoing analytics integration

---

## Key Business Insights

### User Engagement Patterns
- **Conversion Rate:** Only 28% of users progress from signup to streak achiever status
- **Biggest Drop-off:** 45% of users abandon the app after completing just 1-2 lessons
- **Early Indicators:** Users completing 5+ lessons in their first week have 75% lower churn rates

### A/B Testing Results
- **Notification Timing Impact:** Evening notifications show +0.8 daily sessions per user on average
- **Lesson Completion Advantage:** Evening group completes 2.1 more lessons per user compared to morning group
- **Statistical Significance:** Both metrics achieved p < 0.001 with medium to large effect sizes

### Churn Risk Identification
- **Model Performance:** Logistic regression achieves 0.847 AUC-ROC with 78% precision on churn prediction
- **High-Risk Users:** 18% of the user base scores above 0.7 churn probability threshold
- **Key Predictors:** Daily session frequency has the strongest negative correlation with churn risk (-0.89 coefficient)

### Real-time Monitoring Capabilities
- **Operational Insights:** Hourly engagement patterns reveal optimal intervention timing windows
- **Risk Alert System:** Automated identification of at-risk user segments enables proactive retention efforts
- **Performance Tracking:** Real-time A/B test monitoring supports agile optimization strategies

---

## Key Visualizations

### User Conversion Funnel
```
Signups (75,000)     │████████████████████████████████████████│ 100%
      ↓              │                                        │
First Lesson (65,250) │████████████████████████████████████    │  87%
      ↓              │                                        │
Active Learner (42,500)│████████████████████████              │  57%
      ↓              │                                        │
Streak Achiever (21,000)│█████████████                        │  28%
```

### A/B Test Results: Evening vs Morning Notifications

**Daily Sessions per User**
```
Morning    │████████████████████ 3.2 sessions
Evening    │████████████████████████ 4.0 sessions (+25%)
```

**Lessons Completed per User**
```
Morning    │██████████████████ 8.1 lessons
Evening    │████████████████████████ 10.2 lessons (+26%)
```

### Churn Risk Distribution
```
Low Risk (0.0-0.4)    │████████████████████████████████████████│ 52%
Medium Risk (0.4-0.7) │██████████████████████████████████      │ 30%
High Risk (0.7-1.0)   │████████████████                        │ 18%
```

---

## Actionable Recommendations

### 1. **Switch to Evening Notifications**
- **Why:** Evening users complete 2.1 more lessons and have 0.8 more daily sessions
- **Action:** Move notification timing to 7:00 PM for all new users starting next month
- **Timeline:** 2-3 weeks to update the notification service

### 2. **Build Early Warning System**
- **Why:** Our model correctly identifies 78% of churners before they leave
- **Action:** Set up daily scoring for the 18% of users flagged as high-risk
- **Timeline:** 4-6 weeks to integrate the model into the user database

### 3. **Fix the Onboarding Drop-off**
- **Why:** Nearly half of users quit after just 1-2 lessons
- **Action:** Add progress celebrations and difficulty adjustment after the second lesson
- **Timeline:** 6-8 weeks for design and development of new onboarding flow

### 4. **Create a Live Monitoring Dashboard**
- **Why:** Hourly patterns show clear engagement peaks that we're not leveraging
- **Action:** Build a real-time dashboard tracking DAU, lesson completions, and risk alerts
- **Timeline:** 3-4 weeks for dashboard setup and team training

### 5. **Target At-Risk Users with Email Campaigns**
- **Why:** 18% of users are high-risk but many could be saved with the right nudge
- **Action:** Send personalized lesson recommendations to users with churn scores above 0.5
- **Timeline:** 4-6 weeks to design campaigns and set up automation

---

## Limitations & Next Steps

### Current Limitations
- **It's Not Real Data:** The biggest limitation is obvious - this is all simulated, so real users might behave differently
- **Model Assumptions:** My churn model assumes the patterns I built into the synthetic data hold true in reality
- **Missing Context:** Real apps deal with competition, marketing campaigns, app store changes, etc. that aren't captured here
- **Limited Features:** I focused on core metrics, but real user behavior includes tons of other signals (device type, content preferences, social features)

### Recommended Next Steps

#### Short-term (1-3 months)
- **Live A/B Testing:** Validate notification timing findings with real user cohorts
- **Model Deployment:** Implement churn prediction system in production environment
- **Real Data Integration:** Begin collecting actual user engagement data to refine synthetic assumptions

#### Medium-term (3-6 months)
- **Advanced Modeling:** Incorporate additional behavioral features (content preferences, social interactions, learning patterns)
- **Personalization Engine:** Develop dynamic user segmentation for individualized experiences
- **Competitive Analysis:** Benchmark findings against industry standards and competitor performance

#### Long-term (6-12 months)
- **Predictive Lifetime Value:** Build comprehensive user value models incorporating engagement predictions
- **Multi-variate Testing:** Expand A/B testing framework to evaluate multiple optimization strategies simultaneously
- **Machine Learning Pipeline:** Establish automated model retraining and performance monitoring systems

---

## Project Deliverables

### Core Analysis
- **Jupyter Notebook:** Complete analytical workflow with professional documentation and visualizations
- **Statistical Reports:** Comprehensive A/B testing results with confidence intervals and effect sizes
- **Predictive Models:** Trained churn prediction model with performance metrics and feature importance

### Data Assets
- **Clean Dataset:** BI-ready CSV export (75,000+ records) optimized for Tableau, Power BI, and other analytics tools
- **Data Dictionary:** Comprehensive field documentation with business context and usage guidelines
- **Synthetic Data Generator:** Reusable code framework for generating additional test datasets

### Business Intelligence
- **Executive Summary:** High-level findings and recommendations suitable for C-level presentations
- **Dashboard Mockups:** Real-time monitoring interface designs with KPI specifications
- **Implementation Roadmap:** Detailed action plan with timelines, resource requirements, and success metrics

### Technical Documentation
- **Code Repository:** Well-documented Python codebase with modular functions and clear commenting
- **Methodology Documentation:** Statistical approaches, model selection rationale, and validation procedures
- **Reproducibility Guide:** Step-by-step instructions for replicating analysis and extending findings

---

## Technical Requirements

### Environment Setup
```bash
# Required Python packages
pandas >= 1.3.0
numpy >= 1.21.0
matplotlib >= 3.4.0
seaborn >= 0.11.0
scikit-learn >= 0.24.0
scipy >= 1.7.0
jupyter >= 1.0.0
```

### Usage Instructions
1. Clone repository and install dependencies
2. Open `gamified-learning.ipynb` in Jupyter environment
3. Execute cells sequentially for complete analysis
4. Export generated CSV files to BI tools for visualization
5. Review executive summary for key findings and recommendations

---

## Contact & Support

This project showcases practical data science skills applied to user engagement and retention challenges. If you have questions about the methodology, want to discuss implementation details, or are interested in collaboration opportunities, feel free to reach out!

**Connect with me:**
- **GitHub:** [@asadadnan11](https://github.com/asadadnan11)
- **LinkedIn:** [Asad Adnan](https://linkedin.com/in/asadadnan11)

**Project Status:** Complete Analysis | Ready for Business Implementation | Portfolio Demonstration
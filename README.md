# SQL Business Case Study Portfolio Project

## Introduction:
Seeing an untapped market, Danny created Foodie-Fi—a streaming platform solely for food-focused content. Think of it as a specialized version of Netflix dedicated entirely to culinary shows. Foodie-Fi provides both monthly and annual subscriptions, giving members unlimited access to exclusive cooking videos worldwide.

## Business Challenge
Danny is currently facing a challenge in guiding investment strategies due to a lack of data-backed insights. This limited data visibility risks less-than-optimal resource allocation, impacting potential growth and strategic investments.

## Objectives
Danny’s goal is to harness digital subscription data to steer investment decisions and optimize feature development. By focusing on data-driven strategies, the aim is to enhance the precision of decision-making, improve resource distribution efficiency, and foster business expansion. This involves aligning investments with key opportunities and the evolving needs of Foodie-Fi’s customer base.

## Stakeholder(s):
CEO/Founder

## Table 1: PLANS
- When signing up for Foodie-Fi, customers can select from Basic or Pro plans.
- The Basic plan offers limited content access with a monthly fee of $9.90.
- The Pro plan allows unlimited streaming with no watch-time restrictions and includes offline downloads. Subscribers can choose a monthly rate of $19.90 or an annual rate of $199.
- Customers start with a 7-day free trial, after which they automatically shift to the Pro monthly plan unless they cancel, choose to downgrade to Basic, or upgrade to an Annual Pro plan.
- If a customer cancels, their account enters a churn status (reflected as a churn plan record with a zero price). They retain access until the end of their current billing cycle.

## Table 2: SUBSCRIPTIONS
- Subscription records in this table show the start dates associated with each customer's selected "plan_id."
- If a customer downgrades or cancels, the higher plan continues until the billing period ends, with the new plan taking effect from the specified "start_date."
- Any upgrades from Basic to either Pro or Annual Pro are immediate.
- Churned customers retain access until the billing cycle’s end, and their "start_date" indicates the day they chose to cancel the service.

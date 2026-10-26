# Engineering evidence

This repository contains a recruitment case study, not a second copy of the application. Implementation and test references point to [BudgetPro's source repository](https://github.com/Kamisia/mbp_1).

## Source snapshot

The case study was prepared on 26 October 2026 using the local application checkout. Its HEAD was `f9acfb4dccce327ad8e2c7b1184e5a1cce442911`; the checkout also contained uncommitted documentation and housekeeping changes. Links below pin implementation references to that commit. Existing screenshots were supplied by the local project archive and were not newly captured for this document.

## Implementation references

| Case-study topic | Source |
| --- | --- |
| Framework and library versions | [package.json](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/package.json) |
| Shared view calculations | [budgetMonthReadModel.ts](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/src/utils/budgetMonthReadModel.ts) |
| React read-model integration | [useBudgetDerivedData.ts](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/src/hooks/useBudgetDerivedData.ts) |
| Persistence boundary | [householdBudgetRepository.ts](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/src/server/repositories/householdBudgetRepository.ts) |
| Independent-budget migration and rationale | [ADR 0003](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/docs/adr/0003-independent-budget-access.md) |
| Stale plan saves and revisions | [month-plan-versions.test.mjs](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/scripts/month-plan-versions.test.mjs) |
| Field-level approval conflicts | [precise-month-requests.test.mjs](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/scripts/precise-month-requests.test.mjs) |
| Expense retry protection | [expense-retries.test.mjs](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/scripts/expense-retries.test.mjs) |
| Atomic approval and deletion | [approval-deletions.test.mjs](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/scripts/approval-deletions.test.mjs) |
| Expense editing permissions | [expense-edit-access.test.mjs](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/scripts/expense-edit-access.test.mjs) |
| Mobile entry and focus checks | [expense-entry-ux.spec.ts](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/e2e/expense-entry-ux.spec.ts) |
| CI checks | [quality.yml](https://github.com/Kamisia/mbp_1/blob/f9acfb4dccce327ad8e2c7b1184e5a1cce442911/.github/workflows/quality.yml) |

## Interpretation and limits

- Product explanations describe implemented behavior and the rationale visible in the code and project documentation. They do not claim a formal user-research process.
- No team size, personal ownership split, development duration, or commercial results are asserted because those details were not supplied.
- Screenshot amounts are demonstration values. Images show a Polish interface and should not be read as evidence of a complete English product.
- Test files show intended assertions and test boundaries. Their presence does not establish the latest execution result.
- The application test suites and a deployed acceptance test were not run as part of preparing this documentation.
- Source links require access to the application repository if it is private. Screenshots and the case-study narrative are included directly here.

## Screenshot inventory

The six PNG files in `assets/` cover the month plan, expense entry, and summary on desktop and mobile. They were copied from existing viewport captures, without altering the interface or adding unimplemented functionality.

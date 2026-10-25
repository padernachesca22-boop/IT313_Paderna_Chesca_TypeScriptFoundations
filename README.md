# IT313 - TypeScript Foundations

## Problem Description

This project is an Enrollment Eligibility Checker for IT 313 Mobile Programming. It calculates the average grades of students and determines whether each student is PASSING or PROBATION.

## TypeScript Concepts Applied

- **Basic Types:** Used `string`, `number`, and `Promise` to define data types.
- **Interfaces:** Used `Enrollee` and `EligibilityReport` to describe the structure of student data and reports.
- **Enum:** Used `EnrollmentStatus` to represent PASSING and PROBATION.
- **Optional Property:** Used `remarks?` to display consultation remarks only for students on probation.
- **Union Type:** Used `string | number` for the batch ID.
- **Type Narrowing:** Used `typeof` to determine whether the batch ID is a string or number.
- **Generics:** Used `groupBy<T>()` to group reports by status.
- **Modules:** Used named and default exports in `gradeUtils.ts` and imported them into `main.ts`.
- **Async/Await:** Used a simulated registrar request with `Promise`, `setTimeout`, and `try/catch`.
- **Array Methods:** Used `map()` to create reports and `reduce()` to calculate the class average.

## Files

- `main.ts` - Main enrollment eligibility program.
- `gradeUtils.ts` - Functions for computing averages and checking enrollment status.
- `tsconfig.json` - TypeScript compiler configuration.

## How to Run

Install the dependencies:

```bash
npm install
```

Run the program:

```bash
npx tsx main.ts
```

Check for TypeScript errors:

```bash
npx tsc --noEmit
```

## Expected Result

- Class Average: 76.07
- Passing: 3 / 5

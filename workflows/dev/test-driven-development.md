---
description: test-driven development (TDD) methodology enforcement
---
# Test-Driven Development (TDD)

Write the test first. Watch it fail. Write minimal code to pass.
**Core principle:** If you didn't watch the test fail, you don't know if it tests the right thing.

## The Iron Law
NO PRODUCTION CODE WITHOUT A FAILING TEST FIRST

Write code before the test? Delete it. Start over.
No exceptions. Don't keep it as "reference". Implement fresh from tests. Period.

## Red-Green-Refactor Cycle

### RED - Write Failing Test
Write one minimal test showing what should happen. 
- Clear name, tests real behavior, one thing.
- Real code (no mocks unless unavoidable).

### Verify RED - Watch It Fail
**MANDATORY. Never skip.**
Run the test. Confirm:
- Test fails (not errors)
- Failure message is expected
- Fails because feature missing (not typos)

### GREEN - Minimal Code
Write simplest code to pass the test. Just enough to pass.
Don't add features, refactor other code, or "improve" beyond the test.

### Verify GREEN - Watch It Pass
**MANDATORY.**
Run the test. Confirm:
- Test passes
- Other tests still pass
- Output pristine (no errors, warnings)

### REFACTOR - Clean Up
After green only:
- Remove duplication
- Improve names
- Extract helpers
Keep tests green. Don't add behavior.

### Repeat
Next failing test for next feature.

**Red Flags - STOP and Start Over:**
- Code before test
- Test after implementation
- Test passes immediately
- Can't explain why test failed
- "I already manually tested it"
- "I'll test after"

All of these mean: Delete code. Start over with TDD.

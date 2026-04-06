# Project Rules

These rules are mandatory for all changes in this repository.

## 1) Scope Discipline
- Implement only the requested scope.
- Do not refactor unrelated code unless explicitly requested.
- Keep changes small and reversible.

## 2) Code Quality
- Prefer readable code over clever code.
- Keep HTML semantic and accessible (`main`, `section`, `button`, proper labels).
- Keep CSS organized and tokenized with variables when styles grow.
- Keep JavaScript defensive: validate inputs and avoid hidden side effects.

## 3) UX and Accessibility
- Keyboard navigation must work for interactive elements.
- Ensure visible focus states.
- Provide text alternatives for non-text UI where needed.
- Maintain sufficient contrast for text and controls.

## 4) Performance
- Avoid unnecessary large libraries for simple interactions.
- Minimize layout thrashing and unnecessary DOM updates.
- Optimize image sizes and avoid blocking resources when possible.

## 5) Testing and Verification
- Every UI change must be manually verified on:
- Desktop viewport (>= 1280px)
- Mobile viewport (~390px width)
- Verify no obvious console errors in browser devtools.

## 6) Git Safety
- Never rewrite history on shared branches.
- Commit messages must be explicit and action-oriented.
- Do not mix unrelated changes in one commit.

## 7) Definition of Done
A task is done only when all are true:
- Requested behavior is implemented.
- Existing behavior is not regressed.
- Basic responsive check passed (desktop + mobile).
- Final diff is clean and scoped.


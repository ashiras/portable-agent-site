# Timeline Script

1. Human Repository
   - Start from clean main.
   - HEAD = f9a81f1
   - README.md unchanged.

2. work create
   - Create agent/coder/step12-e2e/<run-id>.
   - Create isolated managed worktree.

3. Search / Read / Implement
   - Repository search.
   - Read relevant artifacts.
   - apply_patch / write.
   - Result becomes dirty Artifact.

4. Attempt 1 — Guard FAIL
   - Engine says: “Patch applied successfully.”
   - Guard says FAIL.
   - Checkpoint does not advance.
   - Work Packet is generated.

5. Work Packet / Retry
   - Carry checkpoint, dirty Artifact state, Guard failure, Goal, constraints.
   - Do not rely on growing chat history.

6. Attempt 2 — Guard PASS
   - Artifact corrected.
   - Same external Guard runs again.
   - PASS.

7. Gate ACCEPT
   - Portable Agent accepts.
   - New Checkpoint = 7f60c4f.
   - Parent remains f9a81f1.

8. work close
   - Agent branch deleted.
   - Worktree removed.
   - Integration remains “not evaluated.”

9. Final proof
   - Agent side contains accepted change.
   - Human main remains untouched.

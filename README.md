# DMS.Demo.Git.Branching.GitHubFlow.MergePR.Bad01
Steps taken to replicate:
1. Create a new class library project.
2. Add project to source control.
3. Create feature branch named 'feature/foo' & checkout.
4. Add a new class named 'Class2.cs'.
5. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #1'.
6. Commit changes: 'Branch: feature/foo | Commit #1'.
7. Checkout branch 'master'.
8. Add a comment to 'Class1.cs' : '// Branch: master | Commit #2'
9. Commit changes: 'Branch: master | Commit #2'.
10. Checkout branch 'feature/foo'.
11. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #3'
12. Commit changes: 'Branch: feature/foo | Commit #3'.
13. Create a PR branch from 'master' named 'pull/2/merge' & checkout.
14. Merge branch 'feature/foo' into 'pull/2/merge'.
15. Push branches 'master' & 'pull/2/merge'.
16. Create a new pull request. Merge Into: 'master' | From: 'pull/2/merge'
17. Merge pull request.
18. Checkout branch 'master'.
19. Pull latest changes.
20. Evaluate commit history/line.

![image](https://github.com/user-attachments/assets/2a1213a7-dffe-41f0-8a84-ddb1b2f8d284)
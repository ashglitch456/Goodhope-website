# Blog PR workflow (Good Hope Retreaders)

Every blog post adds a card to the top of the article grid in `blog.html`, so
independent PRs conflict with each other as soon as one merges. To prevent that:

1. **Stack new posts.** Before branching a new post, list open PRs. If any blog PR
   is open, branch the new post off the newest open blog PR's branch (not `main`)
   and open the new PR with that branch as its base. If none are open, branch off
   the latest `main`.
2. **Say so in the PR description:** name the PR it is stacked on and note it must
   be merged only after that PR (merge in order, oldest first).
3. **Never push to `main`.** A human reviews and merges each PR.
4. If `main` has moved ahead of an open blog PR, merge `main` into the branch
   (keep both cards in `blog.html`); never rebase or force-push a PR branch.

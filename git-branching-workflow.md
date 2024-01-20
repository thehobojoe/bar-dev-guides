# Push to master workflow

The advantages to this approach are very obvious - pushing to master is fast, efficient, and causes basically no friction in the development process. No branch switching is required, merges can be minimized by lots of smaller more frequent commits, and the complexity of maintaining multiple branches can be totally avoided.

# Pull Request workflow
A pull request workflow provides several advantages.
- Significantly cleaner history by grouping related commits together, especially when using squash merge on github.
- Even when not using an enforced-review workflow, the process of making a PR with a short description and diff display can help catch mistakes.
- When using enforced reviews (or even non-enforced), much more errors can be caught by the testing and code review provided by others, and suggestions for code quality can significantly improve the overall readability and maintainability of the codebase.
- When reviewing someone else's code, the reviewer can gain a ton of knowledge about new systems, and this helps create a broader knowledge-base that will make future improvements or fixes faster and easier
- With a review culture, those without push permissions on a repository will have a far easier time getting their code merged, greatly increasing the chances that they will stick around and provide further improvements in the future. And if they stick around long enough and build their expertise, they can in turn provide reviews for others, creating a positive feedback loop.

This is of course not without downsides:
- Being a volunteer project, people want to work on things they find fun, and usually reviewing code is not fun.
- Being a volunteer project, certain work will have no peers capable of reviewing it properly, e.g. some of the more complex and low-level work done by Beherith, and no one will be obligated by work requirements to learn those skills.
- Immediate velocity getting new code onto master will be slower.

However, I believe the downsides can be mitigated.
- PR's sitting around un-reviewed can be promoted or bumped on discord or elsewhere, to remind other developers of their existence. This is not a full solution, but it can help get eyes on work that is languishing.
- For PR's with no one capable of giving an adequate code review, testing by trusted users can still help validate that it will work as expected, and those with sufficient perms can still merge it without a full code review.
- While immediate velocity of getting code onto master would be lower, overall velocity should increase, both by improving code quality through the review process (which makes future work faster), and by allowing more developers to get involved in the review process, increasing the size of the knowledge-base and active contributors.
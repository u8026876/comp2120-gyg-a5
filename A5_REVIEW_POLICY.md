<!--
Licensed to the Apache Software Foundation (ASF) under one or more
contributor license agreements.  See the NOTICE file distributed with
this work for additional information regarding copyright ownership.
The ASF licenses this file to You under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with
the License.  You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# COMP2120 A5 group review policy

Updated 21 October 2026 following the group repository owner's instructions.
This policy applies to all A5 issues and contributions in
[`u8026876/comp2120-gyg-a5`](https://github.com/u8026876/comp2120-gyg-a5).

## Required review

One approving review from another human group member is sufficient before a
contribution is merged or submitted upstream. The author cannot review their
own work to satisfy this requirement. A majority or unanimous group review is
not required. Tutor review and tutor approval are not required for any issue or
contribution.

A group PR may be opened to request review; approval is not a prerequisite for
opening that review request.

## Record the review

Use an approving GitHub PR review or an explicit approval in the linked group
issue or PR. Identify the human reviewer, reviewed commit or diff, what they
checked, and their outcome. Existing recorded reviews count when they cover the
change being submitted; a separate formal PR approval is not mandatory.

Reviewers may use an agent to help them understand or test the change. The
human reviewer remains responsible for the approval. Automated checks or an
agent-only review do not count as a second person.

Relevant tests, quality checks, and any blocking review findings still need to
be addressed. Report the checks actually run and their limits; local test
results do not establish remote CI or upstream acceptance.

## Current policy and upstream scope

This policy supersedes older references to majority-group review, tutor review,
or tutor approval in issue/PR descriptions, comments, checklists, handoffs, and
chat history. Those older records may remain as historical evidence and do not
add review gates. Members and agents working on older branches should consult
the [current policy on the group fork's main branch](https://github.com/u8026876/comp2120-gyg-a5/blob/main/A5_REVIEW_POLICY.md).

This is the group's review rule. Apache Tika's contribution requirements and
maintainer decisions continue to apply upstream. Keep this fork's coordination
files and documentation changes out of Apache-bound patches and PRs.

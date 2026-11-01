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

Updated 1 November 2026 to align the fork workflow with the
[official Assignment 5 instructions](https://comp.anu.edu.au/courses/comp2120/assignments/assignment5/).

This policy applies to work in
[`u8026876/comp2120-gyg-a5`](https://github.com/u8026876/comp2120-gyg-a5).
It supplements the course requirements; it cannot waive or replace them.
The 21 October wording that waived majority-group and tutor review was
incorrect. This dated correction does not establish that any earlier review
or approval occurred.

## Project and issue selection

The course requires tutor approval of the repository and selected issues
before assignment work begins. Record the scope and actual timing of that
confirmation. Approval of the project or issue selection is separate from the
tutor's review of a proposed upstream PR.

## Group review and internal merge

A group PR may be opened to request review, with review evidence marked as
pending. Before merging a contribution into the group fork's `main`, obtain
at least one approving review from another human group member and address
blocking findings. The author cannot approve their own work for this purpose.

Use an approving GitHub PR review or an explicit approval in the linked group
issue or PR. Record the reviewer, reviewed commit or diff, scope, outcome, and
actual review date. Existing reviews may cover an unchanged implementation;
state what they cover rather than implying approval of later unrelated work.

This internal merge rule does not by itself satisfy the requirements for
opening a PR to Apache Tika.

## Before an official Apache PR

Under Activity 3 of the official brief, discuss the proposed contribution with
the group, ensure at least a majority of the group has looked at it, and have
the tutor look at it before opening the upstream PR. Record who reviewed the
proposed change, what they reviewed, and when. A single internal approval,
automated checks, or earlier project-selection approval does not establish
that these steps have been completed.

Follow Apache Tika's contribution requirements as well. Keep this fork's
coordination files and coursework documents out of Apache-bound patches.

## Evidence and historical records

Reviewers may use an agent to help understand or test a change, but the human
reviewer remains responsible. Agent-only checks do not count as another human
reviewer or as tutor review.

Report the tests and quality checks actually run, their dates, and their
limits. Local test results do not establish remote CI success or upstream
acceptance. Keep current issue and PR descriptions accurate, and preserve
dated historical comments.

Record confirmations in the form in which they occurred. Do not turn verbal
confirmation into an email record, invent dates, or backdate a later review to
a pre-submission stage. If evidence is unavailable, state that limitation.
Course correspondence and submission evidence can remain in the assessed
report rather than being published in this public repository.

The current policy corrects the earlier conflicting fork guidance. Historical
records remain evidence of what was said at the time; the official course
instructions and Apache's contribution requirements continue to govern their
respective scopes.

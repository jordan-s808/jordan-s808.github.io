---
layout: essay
type: essay
title: "Smart Questions, Not-So-Smart Questions"
# All dates must be YYYY-MM-DD format!
date: 2026-09-10
published: true
labels:
  - StackOverflow
  - Questions
---


## Importance of Smart Questions
Smart questions are an important tool for smart software engineers because they can help get answers quickly and efficiently. Being able to be specific about the problem, describe what is going wrong effectively, and show steps already taken can help others to narrow down the issue. The title of the smart question also plays an important role because then the person responding can gauge if they have the right expertise and subsequent users with the same question may also benefit from it later.

## Smart Question
Using Stack Overflow, I found an example of a smart question and a not smart question. The first I will go into is the smart question. The user asked “OpenCL spec uses anonymous union, actual headers don’t quite allow it.” 

The user talked about implementing code using cl_image_desc struct and with the defined anonymous union that contains buffer and `mem_object`. However, when they tried using `mem_object` they got a compiler error saying no member existed. This showed that they were specific on how and where the error occurred. They then did their research and read the header source which said that the behavior was gated behind a macro, `__CL_HAS_ANON_STRUCT__`. As well as checking the most recent online header that renamed `__CL_HAS_ANON_STRUCT__` to `__CL_HAS_ANON_UNION__`. Neither version properly helped explain the problem, so they asked a clear question, and provided three clear options on how to proceed.

After asking this smart question, they got a solid response from an experienced community member, who explained the discrepancy between the versions, and responded to all three options. This led to a follow up question by the user and they managed to find the solution.	

## Not-So-Smart Question
Now, onto the not smart question. The user asked “Python script download blocked by antivirus as a virus [closed]” The user was trying to download and run a script ‘decrypt_chrome_password.py’ from a GitHub repository, but Windows Defender flagged and blocked the download as a virus. When they tried to manually recreate the file using vim, it was shortly auto-deleted.

Despite being polite and clearly written and formatted with a detailed explanation, this is still an example of a not smart question because it was in the wrong forum and didn’t focus on the end goal. The question was closed due to “not about programming or software development” which means that this was more of a security/antivirus question rather than coding/programming question and violates Raymond's “choose your forum carefully”. The question also focuses on getting the script to download rather than what the end goal was, which was to extract saved Chrome passwords. Since the script is trying to extract passwords, it makes sense why the AV blocks it for malware as well.

## Conclusion
Comparing these two questions, it is clear that asking smart questions is an important aspect to being a smart software engineer. The not smart question shows that even though the question may be asked politely and the structure plus steps taken are good, it can still be not smart due to being in the wrong forum or unclear on the goal. The smart question succeeded because the user was courteous, did their research, asked a clear question, and as such got a precise and quick answer. This showed me that you should think more critically and do your due diligence before asking a question because although there are no stupid questions, a question can still be smart and also not-so-smart depending on how it’s framed and where it’s asked.

**AI Disclaimer: AI used for spelling and grammar checks. Thoughts, Ideas, Writing, are all the work of the Author**

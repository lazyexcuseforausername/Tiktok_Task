# Tiktok_Task
This is a repo for the tiktok task deliverable in comm 4190

## Project Overview

This project analyzes TikTok comments about a locker-room incident involving a trans woman and debates over who should be allowed in women’s spaces. We use a large language model (LLM) to label comments and explore how people express support, opposition, or alternative views about access to women’s locker rooms.

**Research Question**

How do TikTok commenters position themselves in debates about whether people assigned male at birth (including trans women) should be allowed in women’s locker rooms, and how reliably can an LLM help us classify these positions?

**Methods**

1.Collect comments

- Load TikTok comments and basic metadata from Tiktok_video.csv.

- Label comments with an LLM

- Use a prompt to ask the LLM whether each comment 1.Supports access to women’s locker rooms, Opposes access, or Suggests alternative arrangements (e.g., unisex, gender-neutral, or family bathrooms).

- Save these labels in ai_coded_data.csv and coded_data.csv.

- Compare to human coding: Compute agreement between LLM and human coders (e.g., Cohen’s kappa, Krippendorff’s alpha).

- Summarize and visualize: Plot distributions of stances and reliability scores using simple charts (ages.png, comment_count.png, count_concept.png, krippendorff.png).

- Interpret what these patterns suggest about how people talk about gendered spaces and safety.

**Key Findings**

1. The comment section is not simply “for” or “against” trans women’s access:
Some comments strongly oppose access, a few support trans women’s rights and inclusion; Others focus on compromise solutions (e.g., unisex or family spaces).

2. LLM performance improved when we: Clearly defined each stance in the prompt; Included examples of alternative arrangements and safety/privacy concerns.

3. The model still had trouble with sarcastic, joking, or very short comments that depend heavily on context.

**Files**

- ***Notebooks***

01_tiktok_task.ipynb – Data loading, initial exploration, and prompt development.

Deliverable.ipynb – Final analysis, figures, and written responses for the assignment.

- ***Data***

Tiktok_video.csv – TikTok video metadata and raw comments.

ai_coded_data.csv – LLM-generated labels for each comment.

coded_data.csv – Early merged dataset of LLM labels and identifiers.

final_coded_data.csv – Cleaned, final dataset combining human and LLM labels.

human_coded_data*.csv – Several versions of human-coded labels used for comparison and reliability checks.

- ***Figures***

ages.png – Visualization of commenter age distribution (if available).

comment_count.png – Comment counts (e.g., by stance or over time).

count_concept.png – Counts of comments per stance category.

krippendorff.png – Plot or summary graphic of reliability metrics.


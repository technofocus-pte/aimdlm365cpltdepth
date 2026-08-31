# Lab 1- Exploring AI Models and model comparison in Microsoft Copilot Chat

**Estimated Duration:** 60 minutes

## Lab Overview

Microsoft Copilot routes each request to one of several AI models
and modes, and also lets you choose one manually from the model
selector. This lab keeps the business context constant — retail — and
varies only the model or mode, so any difference you see in the output
is attributable to the model choice itself rather than to a different
task.

Each exercise runs the same retail prompt or brief across a set of
related models — GPT-5.5/5.6 modes in Exercise 1, Claude Sonnet and Opus
in Exercise 2, Auto against manual GPT modes in Exercise 3, and three
image models in Exercise 4 — and ends with a recommendation table so you
can state, with evidence, which model or mode fits the task best.

## Learning Objectives

After completing this lab, you will be able to:

- Locate and use the model selector in Microsoft Copilot Chat.

- Compare GPT-5.5 Quick Response, GPT-5.5 Think Deeper, and GPT-5.6
  Quick Response on the same retail analysis and explain the difference
  between a mode change (Quick vs. Think Deeper) and a version change
  (5.5 vs. 5.6).

- Compare Claude Sonnet and Claude Opus on the same retail
  board-reporting task and explain the trade-off between the two.

- Compare Auto mode against manually selected Quick Response and Think
  Deeper on the same retail task, and judge how reliable automatic
  routing is.

- Compare MAI-Image-2.5 Flash, Flux 2 Flex, and GPT Image on the same
  retail product-launch visual and explain the trade-off between in-app
  integration and raw image quality.

- Produce a one-line, evidence-based model recommendation for each
  retail use case.

## Prerequisites

- A Microsoft Copilot license assigned to your user account.

- A work or school account in a Microsoft 365 tenant with Copilot
  enabled.

- Access to Microsoft Copilot Chat at m365copilot.com or through the
  Microsoft Copilot app.

- A supported browser: the latest version of Microsoft Edge or Google
  Chrome.

- Permission for your tenant to use the GPT-5.5, GPT-5.6, Claude,
  MAI-Image-2.5, Flux 2 Flex, and GPT Image model families (confirmed by
  your Microsoft 365 administrator).

- Desktop version of Microsoft PowerPoint, and access to any connected
  tools your organization uses for Flux 2 Flex and GPT Image.

- Use only fictitious or non-confidential sample data in a training
  tenant. Do not paste real financial results, customer data, or
  personal information into any lab.

## Lab Environment

- Tenant: A Microsoft 365 tenant with Copilot enabled and the GPT-5.5,
  GPT-5.6, and Claude model families switched on in the admin center.

- User account: A licensed Copilot user with permission to create files
  in OneDrive.

- Permissions: Standard user permissions; no admin role is required to
  complete the learner steps.

- Required resources: Microsoft Copilot Chat, Microsoft PowerPoint,
  and connected access to Flux 2 Flex and GPT Image for Exercise 4.

## Exercise 0- Setting up the Knowledge Base

1.  Navigate to +++[https://onedrive.live.com ›
    login](https://onedrive.live.com/login)+++ and log in with your
    credentials.
![](images/f4470e3617977d62ea63b66bbb9f92733f2bdafb.png)

2.  Enter your password.  
    ![](images/06bf36993029acb7781db19a53957e7756105972.png)

3.  Upload the following files to your OneDrive:  
    - Zava Retail Lab sample data  
    ![](images/9b9ac32e9bc08ee3308a87306384be89e4776e9f.png)

## 

## Exercise 1 — Retail: Comparing GPT-5.5 Quick Response, GPT-5.5 Think Deeper, and GPT-5.6 Quick Response

**Objective:** Run the same retail market-expansion question across
three GPT variants — two modes of the same version, and the quick mode
of the next version — so you can separate the effect of reasoning depth
(mode) from the effect of a model upgrade (version).

### Task 1 — Ask the Question with GPT-5.5 Quick Response

1.  Navigate to +++https://copilot.microsoft.com/+++ and log in with
    your credentials.

Enter your password.

2.  In the left navigation pane, select Chat.  
    ![](images/554449a306b20b79796a7f248be323cc75203b89.png)

3.  Select the model selector and choose GPT-5.5 Quick Response.  
    ![](images/1591026613bdd6d1180b2f12c9fd18007233777b.png)

&nbsp;

4.  Paste the prompt below and select Send.

Prompt:

*“ZAVA Retail is considering expanding its private-label grocery line
into the online-only channel next fiscal year. Consider competitive
pressure from existing online grocers, margin impact of private label
versus national brands, supply-chain and fulfillment readiness, and
brand risk. Give a recommendation with key risks.”*  
![](images/f20b675f749a15a1bdd834a59a660b3eb6068a8f.png)

5.  Review the output:  
    ![](images/92aeee8472948a49459414cd126982f7c14e8aad.png)

6.  Expected result: A fast, high-level recommendation. Note how much of
    the answer is a single blended paragraph versus a structured
    breakdown.

### Task 2 — Ask the Same Question with GPT-5.6 Think Deeper

1.  Select New chat, then select the model selector and choose GPT-5.6
    Think deeper.  
    ![](images/aaf0607da0d17fab93a3e72ab629ae5659b2d72c.png)

2.  Submit the identical prompt used in Task 1.

*“ZAVA Retail is considering expanding its private-label grocery line
into the online-only channel next fiscal year. Consider competitive
pressure from existing online grocers, margin impact of private label
versus national brands, supply-chain and fulfillment readiness, and
brand risk. Give a recommendation with key risks.”*  
![](images/42ff9678a6ba71639ba4501832d56125305933dc.png)

3.  Review the output:  
    ![](images/f2b34d901133b88dab1ef583513ae51d3a34cbb1.png)

**Note: The generation time and whether the risks (competitive, margin,
supply-chain, brand) are treated separately rather than blended
together.**

### Task 3 — Ask the Same Question with GPT-5.6 Quick Response

1.  Select New chat, then select the model selector and choose GPT-5.6
    Quick Response.  
    ![](images/10fc2c5d9418b25e080c440efaade134726b3bda.png)

2.  Submit the identical prompt used in Task 1.

*“ZAVA Retail is considering expanding its private-label grocery line
into the online-only channel next fiscal year. Consider competitive
pressure from existing online grocers, margin impact of private label
versus national brands, supply-chain and fulfillment readiness, and
brand risk. Give a recommendation with key risks.”*  
![](images/913c80dea10c19382daea6b9c3ca266afd7c63b3.png)

3.  Review the output:  
    ![](images/a51314be09669385578fbbdb5df3684d5b56edf6.png)

**Comparison exercise-**

Compare this against the GPT-5.6 Quick Response answer from Task 1 —
both are the fast mode, so any difference here reflects the version
upgrade rather than a reasoning-depth change. Then compare it against
GPT-5.6 Think Deeper from Task 2 to see whether the newer quick mode
closes the gap with the older model's deeper mode.

**Validation**

- You produced three answers to the identical retail prompt — GPT-5.5
  Quick Response, GPT-5.5 Think Deeper, and GPT-5.6 Quick Response —
  each from a clean chat.

- You can state, in one sentence each, how the three differed in
  structure and depth.

- You can say whether GPT-5.6 Quick Response behaves more like GPT-5.5's
  quick mode or its deep mode on this task, and why that matters when
  deciding whether to upgrade versions or switch modes.

- You completed the recommendation table below.

### Model Recommendation — Retail Market-Expansion Analysis

[TABLE]

Recommended model for this use case: GPT-5.5 Think Deeper when the
expansion decision will actually be acted on and the risk categories
need to be weighed against each other; GPT-5.6 Quick Response as the
everyday default once it is available in your tenant, since it narrows
the gap with Think Deeper at quick-mode speed.

## Exercise 2 — Retail: Comparing Claude Sonnet and Claude Opus on the ZAVA Retail Board Update

Objective: Run the same ZAVA Retail board update through Claude Sonnet
and Claude Opus so you can judge the trade-off between a faster,
lighter-weight Claude model and the flagship model, on a task where tone
and judgement matter.

### Task 1 — Draft the Update with Claude Sonnet

1.  In Copilot Chat, select the model selector and choose Claude
    Sonnet.  
    ![](images/6a6e32537d4083a44bb72c7d563699d1193e6c75.png)

2.  Paste the prompt and sample data below, then select Send.

Prompt:

> *“Draft a concise, one-page board update summarizing last quarter's
> market conditions and financial highlights for the CFO to present to
> the board.”*
>
> *Sample data — ZAVA Retail, Q2 FY2026 Earnings Highlights:*
>
> *Revenue: $428 million, up 8.5% year over year and 3% above plan.*
>
> *Gross margin: 31.2%, versus 30.1% in Q2 FY2025. Operating profit: $52
> million, up 14% YoY.*
>
> *Digital sales up 18% YoY, now 34% of total revenue. Same-store sales
> up 5.2%.*
>
> *Consumer spending remained cautious due to inflation; competitive
> pricing pressure increased in electronics and household products.*
>
> *Opened 12 new stores in tier-2 markets; loyalty membership up 16% YoY
> to 8.4 million members.*
>
> *AI-assisted inventory forecasting expanded to 70% of stores, reducing
> stockouts ~12%.*
>
> *Risks: FX volatility and input costs; full-year revenue guidance
> holds at 7%–9%.”*  
> ![](images/353e63bc5c4e70a9e8cb9ba6a03c8f95dfce01b1.png)

3.  Review the output:  
    ![](images/6c7ad4de6dc5db569ed9d633af383e6c53ca38dd.png)  
    Expected result: A well-organized, competent draft, generated
    quickly.

### Task 2 — Regenerate with Claude Opus

1.  Select New chat so the second draft is not influenced by the first
    model's output.

2.  Select the model selector and choose Claude Opus.  
    ![](images/9bfa40935c569d766a3d1caef4d593e930f74b9c.png)

3.  Paste the identical prompt and sample data used in Task 1.

> *“Draft a concise, one-page board update summarizing last quarter's
> market conditions and financial highlights for the CFO to present to
> the board.”*
>
> *Sample data — ZAVA Retail, Q2 FY2026 Earnings Highlights:*
>
> *Revenue: $428 million, up 8.5% year over year and 3% above plan.*
>
> *Gross margin: 31.2%, versus 30.1% in Q2 FY2025. Operating profit: $52
> million, up 14% YoY.*
>
> *Digital sales up 18% YoY, now 34% of total revenue. Same-store sales
> up 5.2%.*
>
> *Consumer spending remained cautious due to inflation; competitive
> pricing pressure increased in electronics and household products.*
>
> *Opened 12 new stores in tier-2 markets; loyalty membership up 16% YoY
> to 8.4 million members.*
>
> *AI-assisted inventory forecasting expanded to 70% of stores, reducing
> stockouts ~12%.*

*Risks: FX volatility and input costs; full-year revenue guidance holds
at 7%–9%.”*  
![](images/47eb6856068a762be83522565f13a87bad3430fa.png)

4.  Review the output:  
    ![](images/e84eb856d270f381035a5588271d06c2008ffe11.png)

5.  Read both drafts side by side and evaluate: tone, narrative
    judgement (does it lead with what the board actually needs to
    decide?), handling of risk language, and overall readiness to send
    without further editing.

**Validation**

You produced two drafts of the same board update — one from Claude
Sonnet, one from Claude Opus — each started from New chat.

You can state, in one sentence per model, how the outputs differed (for
example: Claude Sonnet — fast, competent, close to a clean summary;
Claude Opus — slower, but stronger editorial judgement on what to
foreground and how to phrase risk for an external audience).

You completed the recommendation table below.

### Model Recommendation — Retail Board Reporting

[TABLE]

Recommended model for this use case: Claude Opus for the final
board-ready version; Claude Sonnet is the right choice for the everyday,
lower-stakes retail writing that doesn't need that extra layer of
judgement.

## Exercise 3 — Retail: Testing Auto Mode Against Quick Response and Think Deeper

Objective: Run the same retail supplier-communication task through Auto
mode and through manually selected Quick Response and Think Deeper, so
you can judge how much you can rely on automatic routing for a task
where tone and judgment matter.

### Task 1 — Submit the Prompt in Auto Mode

1.  In Copilot Chat, select the model selector and choose Auto
    (sometimes shown as GPT-5 Auto).  
    ![](images/2a38246d1821670e2c0a7878b4cf5eef11e29100.png)

2.  Prompt:

“Write a two-paragraph note from ZAVA Retail to a major supply-chain
partner explaining a two-week delay to an inventory shipment, while
preserving the relationship ahead of the holiday buying season.”  
![](images/2a6e0a1a599f0662a837bba45083bb53ee0f963c.png)

3.  Note which model Auto used to answer, if the interface displays it,
    and read the response.  
    ![](images/9f52adbeff91e4e68b860a59478c401556814357.png)

### Task 2 — Submit the Same Prompt with Quick Response

1.  Select New chat, then select the model selector and choose Quick
    Response.  
    ![](images/af0f753a0428c149fb781c94206807ff65eb5d6b.png)

2.  Submit the identical prompt from Task 1.

*“Write a two-paragraph note from ZAVA Retail to a major supply-chain
partner explaining a two-week delay to an inventory shipment, while
preserving the relationship ahead of the holiday buying season.”*  
![](images/ef89085b50386ba241c80db426aaa18e8fc9b672.png)

3.  Review the output:  
    ![](images/3149482e9a4804ed86ce9257baef3db7860c848b.png)

### Task 3 — Submit the Same Prompt with GPT-5.5 Think Deeper

1.  Select New chat, then select the model selector and choose Think
    Deeper.  
    ![](images/49e51c3983975494d0f546f59d47a41b6c8cd07c.png)

2.  Submit the identical prompt from Task 1.

*“Write a two-paragraph note from ZAVA Retail to a major supply-chain
partner explaining a two-week delay to an inventory shipment, while
preserving the relationship ahead of the holiday buying season.”*

![](images/7fdf058b1ee3f2b527ef1e1c6bdeb6e1abdda981.png)

3.  Review the output:  
    ![](images/99fd916f8b2babc4992f03ea2b8b9212cd5c670c.png)

4.  Compare all three responses on tone, tact, and how ready each one is
    to send to a supplier without further editing. Decide which model
    you would have picked manually, and check whether Auto's choice
    matched it.

**Validation**

- You submitted the supplier-delay note in Auto mode and noted which
  model (if shown) handled it.

- You submitted the same prompt from a New chat with Quick Response and
  again with Think Deeper.

- You can state whether Auto's routing matched the model you would have
  picked manually for this task, and why or why not.

- You completed the recommendation table below.

### 

### Model Recommendation — Retail Supplier Communication

[TABLE]

Recommended model for this use case: manually select Think Deeper for
supplier or client communication where the relationship is at stake —
don't rely on Auto when tone and tact are the point of the task.

## Exercise 4 — Retail: Comparing MAI-Image-2.5 Flash, Flux 2 Flex, and GPT Image for Presentation Visuals

Objective: Generate the same retail product-launch hero image from three
different image models — the native in-app MAI-Image-2.5 Flash, the
standalone Flux 2 Flex model, and GPT Image — so you can judge the
trade-off between workflow integration and raw image quality/control.

### Task 1 — Generate the Image with MAI-Image-2.5 Flash

1.  Open Microsoft PowerPoint and select Create with Copilot.  
    ![](images/b1eea9172c570a5c37cf71fa46efda5699b4a0a5.png)

2.  When the presentation opens you will see the Copilot chat pop-up on
    the right side.  
    ![](images/f53a829bc0a2f41006c93fbadcd4e318121ca968.png)

3.  In the Copilot chat window, select the MAI Image 2.5 Flash.  
    ![](images/8b2698b9c36686275386714b30505aa6191a3ef7.png)

4.  Paste the product brief below.

Product brief:

*“Create a clean, modern hero image for a ZAVA Retail product launch
slide, showing a sleek device on a minimalist studio background in our
brand colours.”*  
![](images/f3189d01a2d5eb962b895090358507b247019791.png)

5.  Review the output:  
    ![](images/51ae8658d435547831b5c26ce1cdf7f2f7825955.png)

6.  Expected result: A fast, on-slide image generated and inserted
    without leaving PowerPoint.

### Task 2 — Generate the Same Image with Flux 2 Flex

1.  Open your organization's connected image-generation tool or
    workspace that provides access to Flux 2 Flex.  
    ![](images/15cd3ec5f477526595c7c356e5289d57a32154c0.png)

2.  Paste the identical product brief from Task 1.

*“Create a clean, modern hero image for a ZAVA Retail product launch
slide, showing a sleek device on a minimalist studio background in our
brand colours.”*  
![](images/ff19c188de97a5dcf91421039040780293faaf1a.png)

3.  Generate the
    image:![](images/822e525f289d2bf592a17a2a381da25509e2eeaa.png)

4.  Compare it against the MAI-Image-2.5 Flash result: look at fine
    detail, lighting realism, and how closely it follows the
    brand-colour instruction.

### Task 3 — Generate the Same Image with GPT Image

1.  Open your organization's connected tool or workspace that provides
    access to GPT Image or select it from the model selector if
    available in Copilot Chat.  
    ![](images/9ac3aa8156458bd8806cf02c3ebab4ae4ce0e72c.png)

2.  Paste the identical product brief from Task 1.

*“Create a clean, modern hero image for a ZAVA Retail product launch
slide, showing a sleek device on a minimalist studio background in our
brand colours.”*  
![](images/fc689150e3617f08ce55118356008df889fd98c0.png)

3.  Generate the image:  
    ![](images/a1a59d8c8c9c711c39cb8b7027edba8b768edc44.png)

4.  Compare all three images side by side on visual quality, brand-color
    accuracy, and how many extra steps each workflow required beyond the
    native PowerPoint experience.

**Validation**

- You generated the same product launch brief through MAI-Image-2.5
  Flash, Flux 2 Flex, and GPT Image, and have all three images available
  for comparison.

- You can name one workflow difference between the native, in-app model
  and the two standalone models (for example: no export/import step
  versus a manual download-and-insert step).

- You can name one quality or control difference you observed between
  the three images (for example: detail level, adherence to brand
  colors, or realism of studio lighting).

- You have completed the recommendation table below.

### Model Recommendation — Retail Launch Visuals

[TABLE]

Recommended model for this use case: MAI-Image-2.5 Flash for every day,
in-deck visuals since it removes every extra step; reach for Flux 2 Flex
when the image itself is the deliverable — for example, a launch asset
that will also be used outside the deck — and is worth the manual insert
step.

## Lab Summary

Across four exercises — all set in a retail context — you compared
models within the same family or category rather than across unrelated
tasks: GPT-5.5 modes against a GPT-5.6 upgrade, Claude Sonnet against
Claude Opus, Auto mode against two manually selected GPT-5.5 modes, and
three image models against each other for the same launch visual.
Holding the business scenario constant isolates the effect of the model
choice itself, which is the skill this lab is building: before you reach
for a bigger, newer, or externally hosted model by default, check
whether the option already built into your workflow is enough, and know
when the extra time or extra steps are worth it.

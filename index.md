---
layout: default
title: DSC 180A Methodology Assignment 4
---

# DSC 180A Methodology Assignment 4

**Gabriel Maayah**  
[gmaayah@ucsd.edu](mailto:gmaayah@ucsd.edu)

**Section:** D08 – From First Search to Trust at Scale: Building Data-Driven Marketing Systems and AI Agents for the Fertility Patient Journey and Online Reputation Management  
**Mentors:** Gabriel Andres Garzo and Madison Hughes, Reproductive Partners Fertility Center San Diego (RPSD)

---

**What is the most interesting topic covered in your domain this quarter?**  
The most interesting topic has been how large language models are becoming a "front door" for a business's reputation. Patients increasingly ask ChatGPT or Google's AI Overviews which fertility clinic to choose instead of reading reviews themselves, so what those models say is shaped by whatever public patient reviews, forums, and articles they were trained on or retrieve. That means reputation management is no longer just about responding to individual Google or Yelp reviews — it's about understanding the whole body of online patient experiences that feeds into an AI's summary of a clinic. Working on review collection (Track 1) made it clear how fragmented that data is across platforms and how much access and permission rules shape what anyone, including an AI, can actually see.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**  
I would like to investigate whether the themes in real patient reviews explain what LLMs say about a clinic. Using the Google Business Profile and Yelp reviews we collected for RPSD (and, once permission is cleared, reviews from sources like FertilityIQ), I would extract the recurring topics and their sentiment — for example, communication with doctors, wait times, billing, emotional support, and outcomes. I would then prompt several LLMs with questions a prospective patient might ask ("Is RPSD a good IVF clinic?") and compare the themes in their answers to the themes in the reviews. This would show which parts of the patient experience AI systems amplify, which they miss, and which complaints the clinic could address to most improve how it is represented.

**What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**  
I would build the data collection around permission-cleared sources from the start instead of treating access as a problem to solve later. In Quarter 1, a lot of time went into trying Reddit's research API (which was denied) and figuring out whether collecting other clinics' reviews was allowed. Next time I would first map out every source, its terms of use, and the access route (official business account exports, official APIs, or written permission like a request to FertilityIQ), and then design one shared schema — source, date, rating, review text, clinic — so that reviews from every platform land in the same format and can be re-collected on a schedule without manual cleanup.

**What other techniques would you be interested in using in your project?**  
- **Aspect-based sentiment analysis** to score sentiment for specific parts of the patient experience, not just an overall star rating.  
- **Topic modeling** (e.g., BERTopic with sentence embeddings) to discover review themes without defining them by hand.  
- **LLM-based classification** with a small hand-labeled validation set to check accuracy against human judgment.  
- **Time-series / change-point analysis** to see whether sentiment shifts after events like staff changes or new services.  
- **Retrieval-augmented generation (RAG)** to test how an AI's description of the clinic changes when it is given different sets of reviews as context.

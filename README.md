# Global-AI-Hackathon-Project
Hackathon Project Ideas:

## Project Idea 0 :-
##### AI Roundtable - Make your own podcast about a topic u could not find online. 

    A podcast you can actually participate in
    Imagine two AI personalities(multi-agent) discussing a topic while you interrupt, ask questions, challenge an argument, or change the discussion entirely.
    Instead of listening to a 40-minute podcast, you could understand today's important news in five minutes, with an option to dig deeper.
    Possible categories: World news, technology & AI, science, business & economics, and sports.




## Project Idea 1:(Combination of the 3 points below) MAIN-

 #### Layer 1: Offline scanner (the core, must work with no internet)

Fine-tune a small CNN (MobileNetV3 or EfficientNet-Lite)(We are going to use VIT) and convert it to TFLite.
Pick one crop or a few crops, with 5-10 disease classes plus a “healthy” class.
Apply temperature scaling for calibration. Abstain (“not sure, try another photo”) below a confidence threshold. Consider an “unknown / not a leaf” class too.
Datasets: PlantVillage is lab-style and will overfit to clean backgrounds. PlantDoc and Cassava Leaf Disease have more realistic field photos. Read each license first, and state the lab-vs-field gap in your limitations.

#### Layer 2: Step-by-step treatment (also offline)

Don’t generate treatment advice with an LLM. Pesticide and dosage advice needs to be accurate, so bundle curated treatment protocols per disease, sourced from university extension services or similar, with citations.
This is where the lab-bench idea fits: a stateful step tracker (“Step 2 of 6: remove infected leaves”, mark done, resume later). Skip speech and vision verification in the first version. A checklist with an optional photo check-in is a stretch goal.

#### Layer 3: Literature checker (online only)

A backend (or on-demand call) that pulls abstracts from PubMed or Europe PMC for the detected disease, extracts claims (e.g., “fungicide X reduces blight severity”), grades the evidence (study type, sample size, field vs lab), and flags contradictions between papers.
Cache results for diseases already looked up so they’re available offline later.
Cut line: abstracts only, one crop or disease family.

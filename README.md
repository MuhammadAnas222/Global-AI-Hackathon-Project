# Global-AI-Hackathon-Project
Hackathon Project Ideas:

  # 2. Offline plant or crop disease scanner for low-connectivity users (Android)

    What it is: an Android app that diagnoses leaf photos on the phone with no internet, shows its confidence, abstains when unsure, and gives short treatment guidance.
    Why it’s hard: you train or fine-tune an image classifier and convert it for mobile, and you calibrate confidence so “I’m not sure” is trustworthy. Adding on-device language generation is a stretch goal.
    Evidence: accuracy on a held-out test set, plus a calibration check showing that high-confidence predictions are right more often than low-confidence ones. Include latency on a real phone, and test on photos taken outside the dataset, where accuracy usually drops.
    Builds on: your computer vision and ML coursework and your Android experience.
    Cut line: 5-10 disease classes, no language generation.
    Check: pick a public dataset and read its license before you start. Many are lab-style images that won’t match field photos, so say that in your limitations.

  # 4. Claim-level literature checker for biology

    What it is: a multi-agent system that reads papers on a gene or disease, extracts individual claims, grades the evidence for each, flags contradictions between papers, and checks claims against structured databases like Open Targets.
    Why it’s hard: reliable claim extraction, contradiction detection, and a fair evaluation.
    Evidence: score its gene-disease claims against known associations in a curated database, and report precision, recall, and the kinds of errors.
    Builds on: your biomedical agent.
    Caveat: if you extend your existing agent, disclose that as the starting point and separate what you added during the event.
    Cut line: abstracts only, one disease area.

# 5. Real-time, multi-step lab-bench copilot (multimodal)

    What it is: you speak or photograph a step, and the assistant follows a protocol, checks your setup against the next step, and warns you about mistakes it can see, such as a wrong volume on a labeled tube.
    Why it’s hard: it combines speech, vision, and stateful protocol tracking, so the system must remember which step you’re on.
    Evidence: scripted scenarios with correct and planted-error steps, and how often the assistant catches the mistakes.
    Caveat: this is the riskiest, because vision on real bench photos is unreliable. Test on realistic photos early on day one, and drop the idea if it fails.

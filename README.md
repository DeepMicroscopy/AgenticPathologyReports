# AgenticPathologyReports
Repository for the paper "Errare algorithmicum est - Exploring General-Purpose Autonomous Multimodal Agents for Pathology Report Generation"

 > Recent advances in agentic artificial intelligence, i.e. systems capable of autonomous perception, reasoning, and tool use, offer new opportunities for digital pathology. In this pilot study, we evaluate whether two agentic multimodal AI systems (OpenAI’s ChatGPT 5.0 in agentic mode, and H Company's Surfer) can autonomously navigate, describe, and interpret histopathologic features in digitized tissue slides on a slide viewing platform. A set of 35 veterinary pathology cases, curated for training purposes, was used as the test dataset. The agent was tasked with autonomously exploring whole-slide images using a web-based slide viewer, identifying salient tissue structures, generating descriptive summaries, and proposing provisional diagnoses. We fed different prompts to explore three scenarios: 1) analysis without knowledge of the signalment, 2) analysis with organ and species provided, and 3) diagnosis based on a morphological description provided. All outputs were reviewed and validated by a board-certified pathologist for accuracy and diagnostic consistency. We further tasked another board-certified pathologist with the same task to establish a baseline. We found the systems to yield accurate diagnoses in up to 28.6\% of cases with only images, signalment and organ provided, and up to 68.6\% when a morphological description was provided. With only the WSI provided, the models were only correct in up to 5.7\% of cases. The human expert, on the other hand, achieved 85.7\% diagnostic accuracy with only a single WSI, and 88.6\% when also signalment and organ was provided.
> The study demonstrates that while the agentic AI system can meaningfully engage with web-based slide viewing software to assess complex visual pathology data and produce contextually aligned feature descriptions, diagnostic precision remains limited compared with a human expert.

## Example Prompts

This repository includes three example prompts corresponding to the different experimental scenarios tested in the study:

### Trial A: WSI Only (No Signalment)
- **File**: `example_prompt_A_only_WSI.txt`
- **Description**: Prompt for analyzing whole-slide images without any signalment information. The agent must autonomously navigate the WSI, identify structures, and propose a diagnosis based solely on visual features.

### Trial B: WSI with Signalment
- **File**: `example_prompt_B_WSI_and_signalment.txt`
- **Description**: Prompt for analyzing whole-slide images with organ and species signalment provided. This additional context helps the agent narrow down diagnostic possibilities.

### Trial C: Morphologic Description Only
- **File**: `example_prompt_C_morphologic_description_only.txt`
- **Description**: Prompt where the agent is provided with a detailed morphologic description of the tissue rather than navigating the WSI directly. The agent must interpret the description and provide a diagnosis.

## Trial Videos

The repository also contains demonstration videos showing the agents in action:

- **`chatgpt_1052_1519_1088_no_signalment.mp4`**: ChatGPT agent analyzing cases 1052, 1519, and 1088 without signalment information (Trial A scenario)
- **`chatgpt_1261_1524_1224_signalment_trimmed.mp4`**: ChatGPT agent analyzing cases 1261, 1524, and 1224 with signalment provided (Trial B scenario)
- **`surfer_1008_1109_1149_with_signalment.mp4`**: Surfer agent analyzing cases 1008, 1109, and 1149 with signalment provided (Trial B scenario)

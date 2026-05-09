cd ~/work/robot_re
mkdir -p prompts docs logs

cat > prompts/mechanism_robot_literature.md <<'EOF'
# Task: Literature Search on Mechanism-Based Robots

You are working in the repository: robot_re.

This is a literature search task only.

## Output file

Create or update only this file:

docs/mechanism_robot_literature.md

Do not create or modify other files unless explicitly asked.

## Research topic

Search recent high-quality papers from 2020 to 2026 about robots that gain clear functional advantages from special mechanisms, mechanical principles, structural designs, morphologies, passive mechanisms, compliant mechanisms, variable-stiffness mechanisms, morphing structures, tendon or elastic mechanisms, adhesion mechanisms, origami or kirigami mechanisms, reconfigurable structures, or other structure-driven designs.

The goal is to find representative robot papers where the mechanism itself gives the robot a clear advantage.

This task is not about any specific robot platform. Do not force the papers to relate to robotic tails, Unitree Go2, IsaacLab, MuJoCo, or quadruped robots unless the paper itself is naturally relevant.

## Target venues

Main target venues:

1. IEEE Transactions on Robotics
2. Science Robotics
3. Science
4. Nature
5. Science Advances
6. Nature Communications
7. Nature Machine Intelligence

Optional venues, only if the paper is highly relevant:

1. Advanced Science
2. Advanced Intelligent Systems
3. Soft Robotics
4. IEEE Robotics and Automation Letters
5. Nature Communications Engineering
6. npj Robotics, if relevant

## Paper selection criteria

A paper should preferably satisfy all three conditions:

1. It proposes or uses a clear mechanism, structure, morphology, passive design, elastic or compliant design, variable-stiffness mechanism, morphing structure, adhesion mechanism, origami or kirigami mechanism, tendon mechanism, or reconfigurable mechanism.

2. The mechanism is integrated into an actual robot system, not only tested as a standalone material, actuator sample, or isolated structure.

3. The mechanism gives the robot a clear advantage, such as better locomotion, stability, climbing ability, grasping, manipulation, landing, impact resistance, jumping, swimming, flying, perching, attachment, energy efficiency, terrain adaptability, workspace, load capacity, robustness, or control simplicity.

## Search strategy

Search in stages.

### Stage 1: Science Robotics

Search Science Robotics papers from 2020 to 2026 using keywords such as:

- robot mechanism
- robotic mechanism
- morphing robot
- reconfigurable robot
- variable stiffness robot
- compliant mechanism robot
- passive mechanism robot
- origami robot
- kirigami robot
- tendon-driven robot
- adhesion robot
- bioinspired robot mechanism
- morphology robot
- embodied intelligence robot
- soft mechanism robot

### Stage 2: IEEE Transactions on Robotics

Search IEEE Transactions on Robotics papers from 2020 to 2026 using similar keywords.

Prioritize papers with real robot experiments and clearly described mechanisms.

### Stage 3: Science and Nature family journals

Search:

- Science
- Nature
- Science Advances
- Nature Communications
- Nature Machine Intelligence

Focus on robot systems where the mechanical structure gives a functional advantage.

### Stage 4: Optional journals

Search optional journals only if needed:

- Advanced Science
- Advanced Intelligent Systems
- Soft Robotics
- IEEE Robotics and Automation Letters
- Nature Communications Engineering
- npj Robotics

Only include papers from these venues if they are highly relevant.

## Verification rules

Do not fabricate citations.

For every paper, try to verify:

1. title
2. year
3. journal
4. DOI or official publisher link
5. whether the mechanism is actually integrated into a robot
6. whether there is code, video, supplementary material, or project page

Use reliable sources when possible:

- publisher page
- DOI page
- official journal page
- author project page
- author GitHub
- lab website
- arXiv page, if available
- Semantic Scholar, Crossref, or OpenAlex only as auxiliary sources

If information cannot be verified, mark it as:

needs verification

If code or video is not found, write:

not found

Do not guess DOI, code links, or video links.

## Required output structure

Write the result to:

docs/mechanism_robot_literature.md

Use this structure:

# Mechanism-Based Robots Literature Search

## 1. Scope

Briefly explain the search scope:
- years: 2020-2026
- target venues
- mechanism-based robot selection criteria

## 2. Main literature table

Use a Markdown table with these columns:

| No. | Year | Journal | Title | Robot type | Mechanism / structural principle | Robot advantage | Evidence from the paper | DOI / official link | Code / video / project page | Relevance level | Verification status |
|---|---:|---|---|---|---|---|---|---|---|---|---|

## 3. Summary by mechanism type

Group the papers by mechanism type:

### 3.1 Passive mechanisms

### 3.2 Compliant mechanisms

### 3.3 Variable-stiffness mechanisms

### 3.4 Morphing / reconfigurable structures

### 3.5 Origami / kirigami mechanisms

### 3.6 Tendon / elastic mechanisms

### 3.7 Adhesion / attachment mechanisms

### 3.8 Bio-inspired morphology

### 3.9 Other special mechanisms

## 4. Most representative papers

Rank the top 10 papers.

Ranking criteria:

1. clarity of the mechanism
2. integration into a real robot
3. strength of demonstrated advantage
4. paper quality and venue
5. usefulness as a design reference for mechanism-based robot research

For each paper, explain:

- what the mechanism is
- what robot it is used on
- what advantage it provides
- what evidence supports the advantage
- why it is a good reference

## 5. Common writing angles for a literature review

Summarize how these papers describe the relationship between:

- mechanism design and robot performance
- morphology and function
- passive adaptability
- compliant interaction with the environment
- control simplification
- energy efficiency
- environmental adaptability
- mechanism-driven capability improvement

## 6. Papers that need further verification

List papers where title, DOI, code, video, or mechanism details are uncertain.

## Quality requirements

- Prefer confirmed high-quality papers over many weak papers.
- Do not include papers only about materials without robot integration.
- Do not include papers only about control algorithms unless there is a clear mechanical mechanism.
- Do not overstate the advantage.
- Use precise academic wording.
- If a paper reports a metric, include the metric.
- If a paper only qualitatively demonstrates an advantage, say so clearly.
- Mark uncertain information as needs verification.
EOF

# README

This repository demonstrates the use of **MLDS (Meta-Language-defined Structures)** across various domains such as Automotive and Virtual Reality (VR). By providing concrete Meta-Language instructions and corresponding example files, it illustrates the principles and benefits of MLDS instructions.

---

## Repository Structure
```
CoNaLaDe_MLDS
├── Meta-Language instructions 
│  ├── automotive
│  │  └── AutomotiveSecurityMLDSInstructions
│  └── virtualReality 
│     └── VirtualRealityMLDSInstructions
└── MLDS output examples
   ├── automotive
   │  └── Example 1-4
   └── virtualReality
      ├── Example 1-4
      └── reproduceExamples
         ├── architect
         └── reproduceExamples
```

### Directory Details

1. **Meta-Language instructions/**
   - **automotive/**: MLDS instructions for the automotive domain (e.g., security modeling, ECUs, attack vectors).
   - **virtualReality/**: MLDS instructions for the VR domain (e.g., placing objects in 3D environments, spatial relationships).

2. **MLDS output examples/**
   - **automotive/**: Sample MLDS outputs based on the Meta-Language instructions for Automotive.
   - **virtualReality/**: MLDS example outputs for Virtual Reality.
     - **reproduceExamples/**:
       - `architect.txt` and `reproduceExamples.txt` show how to combine natural language descriptions with MLDS instructions (VR-focused). The same principle can be applied to the Automotive domain as well.

---

## What is MLDS?

MLDS (Meta-Language-defined Structures) enables the creation of **formal, machine-readable structures** from natural language descriptions. The basic workflow:

1. **Define the Meta-Language**  
   - For each domain (e.g., Automotive, Virtual Reality), specify which objects, attributes, and relationships are allowed.

2. **Write a Natural Language Description**  
   - VR example: “Create a training room with 20 desks.”  
   - Automotive example: “An ECU with an unsecured Wi-Fi module and potential attack vectors.”

3. **LLM-Driven Generation**  
   - A Large Language Model (LLM) processes the Meta-Language instructions along with your natural language description.  
   - It produces an MLDS file (e.g., JSON) that **exactly** matches the specified structure.

4. **Further Processing**  
   - The MLDS file can be directly imported into a relevant tool (e.g., Unity for VR scenes or a security modeling tool in Automotive).  
   - Additional adjustments can be made in the tool if needed.

---

## How to Reproduce the Examples

### Virtual Reality

1. **Review the VR MLDS Instructions**  
   - Found in `Meta-Language instructions/virtualReality/`. These define valid objects, properties, and relationships.

2. **Check Out Example Outputs**  
   - Located in `MLDS output examples/virtualReality/`. In the `reproduceExamples/` subfolder, you will find:  
     - `architect.txt`  
     - `reproduceExamples.txt`  
     These illustrate how a natural language description can be combined with VR-specific Meta-Language instructions to produce a structured MLDS output.

3. **Create Your Own VR Scenario**  
   - For example, “A room with 10 desks and 10 chairs.”  
   - Prompt your chosen LLM (e.g., GPT-4) with both your scenario and the MLDS instructions. The model will generate a structured MLDS output (such as JSON).

4. **Import and Refine**  
   - This MLDS output can be loaded into a Unity project so that the objects (like desks and chairs) appear automatically as placeholders or finished assets.  
   - If needed, add more objects or modify parameters after import.

### Automotive

1. **MLDS Instructions for Automotive**  
   - See `Meta-Language instructions/automotive/`.

2. **Check the Automotive Examples**  
   - In `MLDS output examples/automotive/`, you’ll find sample MLDS outputs (e.g., describing attack scenarios or security requirements).

3. **Formulate an Automotive Scenario**  
   - For instance, “An ECU with an unsecured wireless module, vulnerable to man-in-the-middle attacks.”  
   - Combine this description with the Automotive MLDS instructions in a prompt, and the LLM will return a formal MLDS structure.

4. **Tool Integration**  
   - Import the generated MLDS into your security modeling tool.  
   - Use the model for risk assessments, mitigation strategies, or further refinements.

### Other Domains

You can generate your own MLDS instructions by defining your own Meta-Language, to do so you can refer to the findings published in our paper.

---

## Tips & Notes

- **Adjust Level of Detail**  
  - You can customize (or simplify) the Meta-Language to provide more (or fewer) details, depending on your needs.  
- **Manual Validation**  
  - Especially for security-critical use cases, it’s always wise to validate the results before using them in production.  
- **Extend as Needed**  
  - The Meta-Language is designed to be flexible. You can add new objects, attributes, or relationship types as your domain requirements evolve.

---

We wish you success exploring these **MLDS (Meta-Language-defined Structures)** examples!  
If you have questions or feedback, feel free to create Issues or submit Pull Requests.

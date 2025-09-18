# JEE-LLM

{
  "name": "JEE Question Solver LLM (Phi-2, Terminal-Based)",
  "description": "A Large Language Model (LLM) based project that solves JEE (Joint Entrance Examination) questions directly from the terminal using Microsoft Phi-2. Provides step-by-step solutions and final answers.",
  "features": [
    "Input JEE questions as plain text in the terminal",
    "Handles Physics, Chemistry, and Mathematics questions",
    "Provides step-by-step detailed explanations",
    "Runs locally with Phi-2 (no external paid APIs needed)",
    "Simple terminal interface, lightweight, and fast"
  ],
  "tech_stack": {
    "language": "Python",
    "model": "Microsoft Phi-2 (via Hugging Face Transformers)",
    "libraries": ["transformers", "torch"]
  },
  "getting_started": {
    "clone": "git clone https://github.com/your-username/jee-phi2-solver.git && cd jee-phi2-solver",
    "virtual_env": {
      "create": "python -m venv venv",
      "activate_linux_mac": "source venv/bin/activate",
      "activate_windows": "venv\\Scripts\\activate"
    },
    "install_dependencies": "pip install torch transformers",
    "run": "python main.py"
  },
  "example": {
    "input": "Find the value of ∫(0 to π) sin²(x) dx",
    "output": [
      "Step 1: Use identity sin²x = (1 - cos2x)/2",
      "Step 2: ∫(0 to π) [1/2 - cos2x/2] dx",
      "Step 3: = [x/2 - (sin2x)/4] (0 to π)",
      "Step 4: = (π/2 - 0)",
      "✅ Final Answer: π/2"
    ]
  },
  "project_structure": [
    "jee-phi2-solver/",
    "│── main.py          # Main terminal app",
    "│── requirements.txt # Python dependencies",
    "│── README.md        # Project documentation"
  ],
  "future_scope": [
    "Improve prompt engineering for more accurate step-by-step answers",
    "Fine-tune Phi-2 on a JEE-specific dataset",
    "Add MCQ solving mode",
    "Support saving solutions to a file for later review"
  ],
  "license": "MIT License",
  "author": {
    "name": "Your Name",
    "note": "Inspired to make AI-powered JEE preparation accessible"
  }
}

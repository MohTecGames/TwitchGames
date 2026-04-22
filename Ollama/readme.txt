# OLLAMA CONFIGURATION GUIDE: FORCING CPU USAGE

This guide explains how to create a custom "CPU-only" model with restricted power usage. This is ideal for background tasks or web applications where you want to keep your GPU free for other processes.

---

## STEP 1: CREATE THE CONFIGURATION
Create a file named "Modelfile" (no file extension) in any folder and paste the following:

FROM <base-model-name>
PARAMETER num_gpu 0
PARAMETER num_thread 4

[Notes]:
- Replace <base-model-name> with your model (e.g., llama3, mistral).
- "num_gpu 0" forces the model entirely onto system RAM.
- "num_thread 4" limits the CPU cores used (adjust this based on your CPU power).

---

## STEP 2: BUILD THE CUSTOM MODEL
Open your terminal/command prompt in the same folder as your Modelfile and run:

> ollama create <new-model-name> -f Modelfile

Example: 
> ollama create llama3-cpu-limited -f Modelfile


---

## TROUBLESHOOTING
- Performance too slow? Increase 'num_thread' in the Modelfile and run the create command again.
- Computer lagging? Decrease 'num_thread' to a lower number (e.g., 2).
- Model not found? Run 'ollama list' to confirm your new name is registered.
# Terminology


**Category**:  An atomic label from a taxonomy that describes the function or meaning of a single code instruction.

**Inconsistency**: A disagreement between profiling functions regarding the category of a given instruction. These are tracked and analyzed to resolve conflicts or mark them as undetermined.

**Notebook**: A Jupyter Notebook for ML written in Python; it serves as the system's primary input.

**MLProfile**: The structured output format representing a profiled notebook. It is targeted by profiling functions (e.g., LLMs, parsers). MLProfiles are encoded in JSON, conforming to the MLProfile metamodel.

**MLProfile-MM (Metamodel)**  
A shared, structured data model that defines the schema for MLProfiles. It ensures interoperability and consistency across different profiling functions.

**Pattern**: A reusable template that defines a specific profile structure. Patterns can be used to filter and compare profiles across notebooks.

**Profiling Bundle**: The data structure that aggregates all information related to the profiling of a notebook: the raw profile, individual profiles, reference profile, and detected inconsistencies.

**Profiling Function**:  A specific method or tool that assigns a category (from a taxonomy) to each code instruction in the notebook. These functions can rely on static parsing, LLMs, or other heuristics.

**Profile Registry**: A system-wide structure that maintains a collection of profiled notebooks and their associated profiling bundles, allowing querying, comparison, and analysis at scale.

**Raw Profile**: An Abstract Syntax Tree (AST) enhanced with metadata to preserve the original code and its location within the notebook.

**Reference Profile**: A unified profile representing a coherent notebook summary derived from the output of multiple profiling functions. It resolves inconsistencies when possible and may contain undetermined mappings where ambiguity remains.

**Step**:  A special kind of category within a taxonomy used to describe the high-level objective of an instruction in a machine learning workflow. Examples include: `Data Preparation`, `Training`, `Evaluation`, etc.

**Taxonomy**: A defined set of categories used to semantically categorize code instructions according to their purpose or behavior in an ML pipeline.



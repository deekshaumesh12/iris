IRIS:  
Problem: 
Recruiters often have to screen large numbers of resumes for a single job. Traditional 
systems mainly depend on keyword matching, which can miss transferable skills and does not 
verify whether a candidate’s claimed skills are actually supported by their experience. 
Our Approach: 
IRIS combines traditional information retrieval with semantic AI to rank candidates and 
explain the reasoning behind each result. The system processes the Job Description and 
resumes, extracts relevant skills and experience, and compares candidate capabilities against 
the requirements of the role. 
Backend Pipeline: 
Job Description + Resumes → Document Parsing → Information Extraction → 
Skill/Requirement Extraction → BM25 + Semantic Matching → Candidate Ranking → Evidence 
Extraction → Skill Verification → Gap & Transferability Analysis → Final Fit Score 
Technical Architecture: 
The backend is responsible for resume and JD processing, candidate data management, 
search, ranking, and evidence retrieval. BM25 is used for exact keyword relevance, while 
embeddings and semantic similarity identify contextual matches and transferable skills. A hybrid 
ranking layer combines these signals with experience relevance and evidence strength to 
produce the final candidate score. 
Candidate Intelligence: 
Instead of showing only an AI-generated percentage, IRIS provides an Evidence-Backed Fit 
Score based on multiple factors such as semantic relevance, keyword relevance, capability 
match, experience, and evidence strength. Each required skill is classified as direct 
evidence, transferable evidence, or insufficient evidence. 
Skill Verification: 
IRIS compares what a candidate claims with what their resume actually demonstrates. For 
example, a candidate may claim Python, Docker, AWS, and Kubernetes. If Python and Docker 
appear in relevant projects while AWS and Kubernetes have no supporting experience, the 
system identifies the difference and assigns confidence levels accordingly. 
Candidate Classification: 
Candidates are grouped into Hire-ready, Trainable, and High Gap categories. 
Key Differentiator: 
The main idea behind IRIS is “Can they back it up?” Rather than simply matching resumes to 
job descriptions, IRIS verifies the evidence behind candidate claims and helps recruiters 
understand whether a candidate should be hired immediately, considered for training, or moved 
down the pipeline.

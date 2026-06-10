# LENS-bench

이 저장소는 **'North or South? Diagnosing LLMs' Understanding of North Korean Language, Society, and Knowledge'** 논문에서 제안하고 활용된 데이터셋과 평가 코드를 설명하고 제공합니다.<br>
This repository explains and provides the dataset and evaluation code proposed and utilized in the paper **'North or South? Diagnosing LLMs' Understanding of North Korean Language, Society, and Knowledge'**.

본 프로젝트는 대형 언어 모델(LLM)이 저자원 사회언어학적 맥락, 그중에서도 오랜 분단으로 인해 남한과 독자적인 차이를 보이고 있는 북한의 언어, 사회, 지식을 얼마나 잘 이해하는지 진단하기 위한 데이터셋을 구축하고, 이에 대한 평가 및 결과를 제공합니다.<br>
This project constructs a dataset to diagnose how well Large Language Models (LLMs) understand the language, society, and knowledge of North Korea—a unique low-resource sociolinguistic context that has developed distinct differences from South Korea due to decades of division—and provides the subsequent evaluation and results.



## 🌟 프로젝트 개요 (Overview)

수십 년간의 분단은 남북한 사이에 어휘, 맞춤법, 사회적 규범, 그리고 이념적 담론의 차이를 만들어냈습니다. 본 논문에서는 표준 남한 한국어에 능숙한 최신 LLM들이 이러한 사회언어학적 차이를 지닌 북한의 맥락을 어떻게 처리하는지 파악하기 위해, 인간 검증을 거친 진단 벤치마크인 **LENS (Language and sociocultural Evaluation for North Korean Society)** 를 도입하고 평가를 진행했습니다.<br>
Decades of division have produced distinct differences between North and South Korea in vocabulary, orthography, norms, and ideological discourse. To examine whether recent LLMs competent in standard South Korean can handle these sociolinguistically distinct North Korean contexts, this paper introduces and evaluates **LENS (Language and sociocultural Evaluation for North Korean Society)**, a human-validated diagnostic benchmark.

이 레포지토리는 논문의 실험을 재현하고 확장할 수 있도록 데이터셋과 일부 소스코드를 제공합니다.<br>
This repository provides the dataset and partial source code to enable replication and extension of the experiments in the paper.



## 📊 데이터셋 구조 (Dataset Dimensions)

논문에서 활용된 LENS 벤치마크는 총 **1,765개의 문항**으로 구성되어 있으며, 3가지 핵심 차원을 평가합니다:<br>
The LENS benchmark utilized in the paper comprises a total of **1,765 items**, evaluating three core dimensions:

1. **Linguistic Robustness (언어적 견고성 - 708문항 / 708 items** <br>
문화적 모호성을 최소화한 STEM(과학·기술·공학·수학) 단답형 질문을 통해 영어, 남한어, 북한어 간의 언어적 이해도를 비교합니다.<br>
Compares linguistic understanding across English, South Korean, and North Korean using STEM short-answer questions that minimize cultural ambiguity.
2. **Sociocultural Perspective Alignment (사회문화적 관점 정렬 - 675문항 / 675 items)** <br>
질문이 남한과 북한 중 어떤 맥락에서 주어졌느냐에 따라 정답이 달라지는 객관식 문항을 통해 관점의 차이를 구분하는지 평가합니다.<br>
Evaluates whether models can distinguish between competing sociocultural frames using multiple-choice questions where the appropriate answers differ depending on the South or North Korean context.
3. **Domain-Specific Knowledge (도메인 특화 지식 - 382문항 / 382 items)** <br>
온라인에서 쉽게 접할 수 없는 북한의 혁명 역사, 사회주의 헌법, 경제지대, 정치/경제 사전 등의 전문 자료를 바탕으로 한 단답형 질문을 통해 실제 지식의 유무를 평가합니다.<br>
Evaluates knowledge grounded in specialized North Korean sources not readily accessible online, such as revolutionary history, the socialist constitution, economic zones, and political/economic dictionaries.

*모든 문항은 북한 이탈 주민(교사 출신 포함), 북한학 전문가 및 남한 검증자들의 Human-in-the-loop 검증 프로세스를 거쳐 높은 신뢰도로 구축되었습니다.*<br>
*All subsets are validated through a rigorous human-in-the-loop process involving North Korean defectors (including former teachers), domain experts, and South Korean annotators.*



## 📁 레포지토리 구조 (Directory Structure)

- `data/` : LENS 벤치마크 데이터셋 (LENS Benchmark Dataset)
- `src/` : 논문 평가용 소스코드 및 정규화 스크립트 (Evaluation Source Code & Normalization Scripts)
- `requirements.txt` : 실행 환경 구성을 위한 라이브러리 목록 (Required Dependencies)



## 📜 인용 (Citation)

본 저장소의 데이터셋이나 코드를 연구에 활용하실 경우 아래 논문을 인용해 주세요.<br>
If you find this dataset or code useful for your research, please cite our paper:

TBA

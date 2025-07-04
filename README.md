# ATTAXML: Behaviour-Based Prediction of MITRE ATT\&CK Techniques in Ransomware with Extreme Multi-Label Learning

![attaxml_logo_cropped](https://github.com/user-attachments/assets/baff73d1-0886-4a3f-9ec6-13c100192341)

## Project Overview

Ransomware remains a persistent threat to cybersecurity, necessitating accurate behavioural analysis for effective defence. This paper presents **ATTAXML**, a framework that applies extreme multi-label learning (XML) to predict MITRE ATT\&CK techniques exhibited by ransomware based on behavioural analysis. We evaluate ATTAXML on **[MLRan Behavioural Dataset](https://github.com/faithfulco/mlran/tree/main/6_experiments/FS_MLRan_Datasets)**, a comprehensive behavioural ransomware dataset, to address two research questions:

* **RQ1:** How accurately can extreme multi-label learning methods predict MITRE ATT\&CK techniques exhibited by ransomware from behavioural reports?
* **RQ2:** What is the predictive value of different behavioural features in identifying ransomware tactics and techniques?

Ransomware samples were executed in a sandbox environment, and features such as API calls, file system activity, and registry modifications were extracted. Corresponding ATT\&CK annotations were also obtained. Our best-performing model achieves **Precision\@5 of 81.33%** and **nDCG\@5 of 91.59%**, successfully identifying core ransomware behaviours mapped to tactics such as *Defence Evasion* and *Impact*. Feature–technique analysis highlights registry access, mass file operations, and API misuse as key predictors. ATTAXML extends conventional detection by offering per-sample ATT\&CK profiles, supporting incident response and threat intelligence.

![system_design](https://github.com/user-attachments/assets/c1401a22-d064-461d-9222-647e23da043f)

## Repository Structure

```
ATTAXML/
│
├── 1_baseline_xml_ransomware.ipynb     # Main notebook implementing the ATTAXML pipeline
├── results/                            # Evaluation results, performance plots, and tables
└── README.md                           # Project description and usage information
```


## Citation

```
@misc{attaxml2025,
  title={ATTAXML: Behaviour-Based Prediction of MITRE ATT\&CK Techniques in Ransomware with Extreme Multi-Label Learning},
  author={Onwuegbuche, Faithful Chiagoziem and Jurcut, Anca Delia and Pasquale, Liliana},
  year={2025},
  howpublished={Submitted for Publication at MLCS2025 and under review.},
  url={https://github.com/faithfulco/ATTAXML}
}
```

## Disclaimer

All ransomware analyses were conducted in **controlled sandbox environments**. This repository **does not distribute raw binaries**. However, we provide the hashes of the samples and complete metadata, including code to help in downloading the samples. Researchers are advised to follow appropriate safety protocols when working with malware and to comply with their institution’s ethical and legal standards.

## Contact

- **Lead Author**: [Faithful Chiagoziem Onwuegbuche](https://github.com/faithfulco)  
- 📧 Email: [faithful.chiagoziemonwuegb@ucdconnect.ie](mailto:faithful.chiagoziemonwuegb@ucdconnect.ie)  
- 🔗 LinkedIn: [faithful-onwuegbuche](https://www.linkedin.com/in/faithful-onwuegbuche/)  

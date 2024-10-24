---
layout: project
title: Data-Driven Fault Detection in Metal Additive Manufacturing Processes
researcher: Alvin Chen
img: assets/img/prod_and_monitoring_testbed.png
importance: 1
category: current
related_publications: true
---

Process faults pose a significant challenge for metal additive manufacturing (AM), resulting in structurally compromised parts or a print failure. To increase reliability and confidence in the metal AM process, we present a dynamic data-driven application system (DDDAS) detection framework that leverages a data-driven time series model to predict the nominal behavior. In-situ images of the melt pool are used to monitor the quality of the weld, and the sequence of melt pool area is used as the time series to be modeled. The deviation between the online, monitored melt pool size and the predicted melt pool size is used for defect detection; a large prediction error indicates the corresponding image deviates from the expected. This distinction can be performed automatically using a statistical threshold metric, which forms the basis of a statistical detection algorithm. Furthermore, by basing the detection criteria on the statistics of the nominal signal, the detection algorithm performs unsupervised, with no labelled anomalies necessary to distinguish process faults.

![](/assets/img/prod_and_monitoring_testbed.png)

**Figure 1:** Metal AM production and monitoring testbed. Laser powder bed fusion (LPBF) relies on thin, deposited layers of metal powder melted by a laser. A coaxial camera that follows the laser path allows for real-time melt pool video.

![](/assets/img/sample_anomaly_detection.png)

**Figure 2:** Presented is a sample anomaly detection with localization. Through modeling the melt pool time series (top), significant errors in the prediction (bottom) lead to deviation in the model parameter statistics (center). This allows for unsupervised detection in the time series domain, which can be localized on the time series-geometry mapping (right).

Aspects of this work have been presented in the following papers: {% cite chen_unsupervised_2022 %}, {% cite chen_unsupervised_2024 %}, {% cite chen_data-sparse_2023 %}.

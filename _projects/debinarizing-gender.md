---
title: "Debinarizing Gender"
excerpt: ""
header:
    overlay_image: assets/images/projects/dynamic-social-systems.png
    overlay_filter: 0.5 
    teaser: assets/images/projects/dynamic-social-systems.png
---

In cultural theory, scholars have conceptualized gender identities and the ways in which they find (visual) expression in heritage collections, as non-binary socio-cultural constructs (Matsuno & Budge, 2017). In contrast, most applications of machine learning in digital humanities classify gender into two mutually exclusive classes. Common performance metrics further exacerbate binarity by penalizing models for uncertainty and non-response. This paper uses CLIP (Radford et. al, 2021), a multimodal model, in combination with C@1 (Peñas & Rodrigo, 2011), a F1 metric that allows (and rewards) non-response, to propose a new method for gender classification on (historical) images.

Binary (gender) classification is built on the conceptual fallacy that a 0.05 prediction for class A automatically entails a 0.95 prediction for class B. We previously showed that CLIP can only simulate (binary) classification tasks (Smits & Kestemont, 2021). CLIP can only approach binary classification by asking two questions (Is this A? Is this B?) and normalizing the outcomes into a single prediction. By measuring CLIP’s approximation of binary prediction with C@1, we hypothesize that we can calibrate algorithms to know when they do not have enough information to make a binary prediction (self-awareness), or when they should postpone binarization. We test our recalibrated algorithm  on stratified sets of nineteenth-century magic lantern slides (Smits & Kestemont, 2021), mid-twentieth century advertisements (Wevers & Smits, 2020), and ‘modern’ photographs scraped from the internet (Schumann et. al, 2021). We hope this helps to shed light on the ways in which gender functioned as an historical social-cultural construct

Bibliographhy
Land, K. (2020). Predicting Author Gender Using Machine Learning Algorithms: Looking Beyond the Binary. Digital Studies / Le Champ Numérique, 10(1), Article 1. https://doi.org/10.16995/dscn.362
Matsuno, E., & Budge, S. L. (2017). Non-binary/Genderqueer Identities: A Critical Review of the Literature. Current Sexual Health Reports, 9(3), 116–120. https://doi.org/10.1007/s11930-017-0111-8
Peñas, A., & Rodrigo, A. (2011). A simple measure to assess non-response.
Radford, A., Kim, J. W., Hallacy, C., Ramesh, A., Goh, G., Agarwal, S., Sastry, G., Askell, A., Mishkin, P., Clark, J., Krueger, G., & Sutskever, I. (2021). Learning Transferable Visual Models From Natural Language Supervision. ArXiv:2103.00020 [Cs]. http://arxiv.org/abs/2103.00020
Schumann, C., Ricco, S., Prabhu, U., Ferrari, V., & Pantofaru, C. (2021). A Step Toward More Inclusive People Annotations for Fairness. Proceedings of the 2021 AAAI/ACM Conference on AI, Ethics, and Society, 916–925. https://doi.org/10.1145/3461702.3462594
Smits, T., & Kestemont, M. (2021). Towards Multimodal Computational Humanities. Using CLIP to Analyze Late-Nineteenth Century Magic Lantern Slides. In M. Ehrmann, F. Karsdorp, M. Wevers, T. L. Andrews, M. Burghardt, M. Kestemont, E. Manjavacas, M. Piotrowski, & J. van Zundert (Eds.), Proceedings of the Conference on Computational Humanities   Research 2021 (Vol. 2989, pp. 149–158). CEUR. http://ceur-ws.org/Vol-2989/#short_paper23
Wevers, M., & Smits, T. (2020, August 23). Detecting Faces, Medium Types, Gender in Historical Advertisments. Workshop at the European Conference of Computer Vision (ECCV), Glasgow.


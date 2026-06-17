---
title:          "HSTM-Det: Hierarchical Timescale Alignment for UAV and Remote Sensing Object Detection"
date:           2026-10-04 00:01:00 +0800
selected:       false
pub:            " IEEE International Conference on Systems, Man, and Cybernetics (SMC 2026), CORE B, CCF C"
pub_date:       "2026"
# semantic_scholar_id: 11ac0b5634a282f1a0da204b98e7473d8b480dfb  # use this to retrieve citation count
abstract: >-
  State Space Models (SSMs), notably Mamba, have
  emerged as promising backbones for visual detection due to
  their linear complexity and global receptive fields. However,
  existing SSM-based detectors typically employ a shared prop-
  agation step size ∆ across all pyramid levels, overlooking the
  inherent multi-scale temporal dynamics of visual features. This
  design induces a timescale mismatch: high-frequency details in
   shallow layers are over-smoothed, while deep semantic features
    suffer from insufficient contextual accumulation. Such mis-
    alignment is further amplified during neck fusion, particularly
    degrading performance in UAV and remote sensing scenarios
    where objects exhibit extreme scale variations and complex
    backgrounds. To address this, we propose the Hierarchical
    Timescale Modulation Detector (HSTM-Det), which explicitly
    reconstructs multi-scale state propagation via learning-based
    dynamic modulation. Our framework introduces three key
    components: (1) a Hierarchical Timescale Modulation (HSTM)
    module that generates level-specific step sizes ∆ conditioned on
    feature statistics, enabling adaptive state updates tailored to
    each pyramid level; (2) an Adaptive Routed Fusion Module
    (ARFM) paired with an HSTM-based Continuity Calibration
    (HSTM-CC) mechanism, which preserves timescale discrepan-
    cies through content-conditioned routing and post-fusion cali-
    bration in the neck; and (3) a Progressive Boundary Refinement
    (PBR) strategy that translates enhanced multi-scale represen-
    tations into precise localization. Extensive experiments on two
    challenging remote sensing benchmarks, NWPU VHR-10 and
    SIMD, validate the effectiveness of HSTM-Det. Specifically, our
    method improves YOLOv11n from 85.3/52.84 to 92.1/63.5 and
    from 86.9/49.78 to 93.4/56.0 in mAP@50/mAP@95, respectively,
    with merely 0.35M additional parameters and 0.6G extra
    FLOPs. These results demonstrate that hierarchical timescale
    alignment provides a principled and efficient solution to ad-
    vance lightweight SSM-based detectors for aerial and satellite
    imagery analysis.

cover:          /assets/images/covers/SMC.png
authors:
  - Yucheng Qiu
  - Zhanhao Liu#
  - He Wang
links:
  Paper: https://www.biorxiv.org
  Code: https://github.com
  Unsplash: https://unsplash.com/photos/orange-fruit-on-white-table-cloth-ISX_imp8t1o
---
# AI on mainframe

[AI on IBM Z®](https://www.ibm.com/z/artificial-intelligence) uses machine learning to convert data from every transaction into real-time insights.  

Uncover insights and gain trusted, actionable results quickly without requiring data movement. Apply AI and machine learning to your most valuable enterprise data on IBM Z—all while using open-source frameworks and tools.

!!! quote

    "IBM is the gold standard for highly secured transaction processing. Now with IBM z16 innovations, our clients can increase decision velocity with inferencing right where their mission-critical data lives" &dash; Ric Lewis, SVP, IBM Systems

This article discusses running machine learning and AI workloads on Z. For generative AI solutions for refactoring, see [Generative AI Capabilities](./genai.md) in this wiki.

!!! key "Key advantages of AI on Z"

    - **Speed to scale with transaction volume**. Achieve up to 19x higher throughput and 20x lower response time co-locating applications and inferencing.
    - **Get real-time insights when needed**. Infuse AI into every transaction while still meeting the most stringent SLAs.
    - **Meet green AI and AI-powered sustainability goals**. Reduce the energy consumption for inference operation processing by 41x using the Integrated Accelerator for AI, versus running inference operations remotely on a compared x86 server using an NVIDIA GPU.

## Telum processor

IBM's new [IBM z16](https://www.ibm.com/products/z16), with its integrated on-chip Telum AI accelerator, is ready to analyze real-time transactions, at scale. This  accelerator is built onto IBM's core Telum processor. With this new dual-processor 5.2 GHz chip and its 16 cores, it can perform 300 billion deep-learning inferences per day with one-millisecond latency. 

One of the Telum design's key innovations is we built an AI accelerator right onto the silicon of the chip and we directly connected all of the cores and built an ecosystem up the stack. Through the hardware design, firmware, the operating systems, and the software, deep learning is built into all of the transactions.

## Financial services use cases

IBM Z to process high volumes of transactions and provide a secured environment for their most sensitive data. By leveraging SQL Data Insights on IBM z16, clients uncover patterns in their mission-critical data to improve their insurance offer predictions and reduce cost.

!!! quote

    "In the insurance sector, customers look for the most personalized service possible to get the assurance they need to feel protected. As a leading provider in Switzerland, our goal is to use the latest technologies available in order to deliver on this promise to our customers. We worked together with IBM to apply the AI capabilities on their trusted IBM z16 systems to process insurance offer recommendations faster and more accurately. By unlocking hidden data patterns with NLP-based AI functions in near-real time while ensuring privacy and security, we saw 94% accuracy in prediction results. These very promising results have motivated us to integrate this technology into our underwriting processes in the near future."  &dash; La Mobilière’s IT architect Thomas Baumann.

## Next steps

- Download our [2023 CEO report](https://w3.ibm.com/services/lighthouse/documents/202444) for our complete findings, including how leaders are taking action in the age of AI:

    - Metrics and decision-making
    - Talent and workforces
    - Technology and data
    - Ecosystem and partners

- See video [AI on IBM Z and LinuxONE with IBM Integrated Accelerator for AI]
- Learn more about AI tools on mainframe. see [AI tools](./aitools.md) in this wiki.

## Reference

- [CEO decision-making in the age of AI](https://www.ibm.com/thought-leadership/institute-business-value/c-suite-study/ceo)
- [AI on Z](https://www.ibm.com/z/artificial-intelligence)
- ZDNet: [The first IBM mainframe for AI arrives](https://www.zdnet.com/article/the-first-ibm-mainframe-for-ai-arrives/)
- [IBM accelerates enterprise AI for clients with new capabilities on IBM Z](https://www.ibm.com/blog/announcement/ibm-accelerates-enterprise-ai-for-clients-with-new-watsonx-capabilities-on-ibm-z/)
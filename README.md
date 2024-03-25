# Publications

This repository contains my published research papers.
 
## Cryptic Bytes: WebAssembly Obfuscation for Evading Cryptojacking Detection ([https://arxiv.org/abs/2403.15197](https://arxiv.org/abs/2403.15197))

**Authors**: Håkon Harnes, Donn Morrison | **Journal**: Pre-print 

**Abstract**: WebAssembly has gained significant traction as a high-performance, secure, and portable compilation target for the Web and beyond. However, its growing adoption has also introduced new security challenges. One such threat is cryptojacking, where websites mine cryptocurrencies on visitors' devices without their knowledge or consent, often through the use of WebAssembly. While detection methods have been proposed, research on circumventing them remains limited. In this paper, we present the most comprehensive evaluation of code obfuscation techniques for WebAssembly to date, assessing their effectiveness, detectability, and overhead across multiple abstraction levels. We obfuscate a diverse set of applications, including utilities, games, and crypto miners, using state-of-the-art obfuscation tools like Tigress and wasm-mutate, as well as our novel tool, emcc-obf. Our findings suggest that obfuscation can effectively produce dissimilar WebAssembly binaries, with Tigress proving most effective, followed by emcc-obf and wasm-mutate. The impact on the resulting native code is also significant, although the V8 engine's TurboFan optimizer can reduce native code size by 30% on average. Notably, we find that obfuscation can successfully evade state-of-the-art cryptojacking detectors. Although obfuscation can introduce substantial performance overheads, we demonstrate how obfuscation can be used for evading detection with minimal overhead in real-world scenarios by strategically applying transformations. These insights are valuable for researchers, providing a foundation for developing more robust detection methods. Additionally, we make our dataset of over 20,000 obfuscated WebAssembly binaries and the emcc-obf tool publicly available to stimulate further research.

## SoK: Analysis Techniques for WebAssembly ([https://doi.org/10.3390/fi16030084](https://doi.org/10.3390/fi16030084))

**Authors**: Håkon Harnes, Donn Morrison | **Journal**: MDPI Future Internet 

**Abstract**: WebAssembly is a low-level bytecode language that enables high-level languages like C, C++, and Rust to be executed in the browser at near-native performance. In recent years, WebAssembly has gained widespread adoption and is now natively supported by all modern browsers. Despite its benefits, WebAssembly has introduced significant security challenges, primarily due to vulnerabilities inherited from memory-unsafe source languages. Moreover, the use of WebAssembly extends beyond traditional web applications to smart contracts on blockchain platforms, where vulnerabilities have led to significant financial losses. WebAssembly has also been used for malicious purposes, like cryptojacking, where website visitors' hardware resources are used for crypto mining without their consent. To address these issues, several analysis techniques for WebAssembly binaries have been proposed. This paper presents a systematic review of these analysis techniques, focusing on vulnerability analysis, cryptojacking detection, and smart contract security. The analysis techniques are categorized into static, dynamic, and hybrid methods, evaluating their strengths and weaknesses based on quantitative data. Our findings reveal that static techniques are efficient but may struggle with complex binaries, while dynamic techniques offer better detection at the cost of increased overhead. Hybrid approaches, which merge the strengths of static and dynamic methods, are not extensively used in the literature and emerge as a promising direction for future research. Lastly, this paper identifies potential future research directions based on the state of the current literature.

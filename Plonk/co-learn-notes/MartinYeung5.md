Plonk 學習 = 基礎認識

proof的目的很重要，要了解到底證明什麼，

ZKP有兩個角色, 一個是prover, 一個verifier, 
如果要編寫prover, 有兩點要留意，第一是要產生一個有效的proof, 第二是要注意在產生proof時，有沒有暴露了一些不想公開的訊息。
如果要編寫verifier，要關注檢查的proof是不是有效的，能否滿足成為有效證明的條件。
prover要用最少的資源去證明一件事，verifier要用最少的資源去驗證一件事。

當完成一組代碼後，就算順利完成編譯，也不算是完全沒有bug的。因為代碼的完整性是不能忽視，需要經過測試，不過惡意的prover有很多種，在測試上是存在很大難度，難以完全進行所有測試。畢竟技術也在進步，有時候新的技術可能會欺騙到verifier。
所以在設計上，最重要的要考慮到自己寫的verifier如何不被惡意prover欺騙。

一個協議需要關注以下三部分: 
1. 完整性(completeness)
能否驗證所有為真的證明

2. 可靠性(soundness)
當證明是真的，就會通過驗證

3. 零知識(Zero-knowledge)

在prover與verifier之間要有大量交互，在有足夠多的交互下，才可以進一步減低作弊的風險。
真的證明能通過驗證，是其中一項條件，不代表這就是完整的。
如果要是假的證明又能通過驗證，這就雖然通過完整性，但就欠缺可靠性。所以兩者需要同時
如果不能區分假的證明，這就雖然通過可靠性，但就欠缺完整性。
所以兩者需要同時為真，才可以做到有效的驗證。

基於Non-interactive zero-knowledge proof ，用戶可以直接生成proof，然後發送到區塊鏈上進行驗證。
從而加快驗證效率

透過Fiat-Shamir transformation，可以實現Non-interactive zero-knowledge proof，
令public coin protocol變成Non-interactive proof。
public coin protocol 可以讓誠實的驗證點發出隨機的coin(可以理解為隨機數)作為訊息，然後由prover產生一個proof。
不過發出隨機的coin的動作不一定由verifier負責，可以由其他人負責。
所以可以引入random oracle來生成隨機數，然後由prover產生一個proof，再直接發送給verifier(on-chain)。

因此，

參考:
1. Fiat-Shamir transformation 
https://www.zkdocs.com/docs/zkdocs/protocol-primitives/fiat-shamir/
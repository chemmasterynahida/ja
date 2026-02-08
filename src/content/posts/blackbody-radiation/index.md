---
title: "量子化学：1.1. 黒体放射"
published: 2025-10-05
description: "黒体放射理論にはどんな問題があり、どう解決されたのでしょうか？"
image: "https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/planck.png"
tags: ["量子化学"]
category: 量子化学
lang: ja
draft: false
---

# 黒体放射

## 量子化学：入門

こんにちは！化学熟知ナヒーダです♪  
今日は、*量子化学* の最初の講義を始めます — 光やエネルギーでさえ、不思議で小さなルールに従う世界への旅です。  

まず、*量子（Quantum）* とは何かを理解する必要があります。  
この言葉、聞いたことがありますよね？ ちょっと未来的で、高度な研究所のイメージがありますよね。例えば、量子コンピュータは今、とても有名です  
![quantum computer](https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/qc.jpg "Quantum Computer by Google")

でも、量子とは本当は何でしょう？  
「量（Quantity）」という言葉を思い浮かべると、もうかなり近いです！  
量子という言葉はそこから来ていて、「小さな量」を意味します。  
量子力学がどう生まれたのかを知ると、この意味が自然に理解できますよ。  

## プランク以前 (~1900年)

19世紀末にタイムトラベルして、量子物理学の誕生につながるパズル — **黒体放射** — を探ってみましょう。  
アイザック・ニュートン卿はその概念を著書 *Opticks* でこう書いています：

> "Do not black Bodies conceive heat more easily from Light than those of other Colours do, by reason that the Light falling on them is not reflected outwards, but enters the Bodies, and is often reflected and refracted within them, until it be stifled and lost?"
>
> 「黒い物体は、他の色の物体よりも光から熱を受けやすいのではないか？光が物体に入って反射されず、物体内で反射や屈折を繰り返し、やがて吸収され失われるからであるか？」

黒い物体は可視光を反射せず、すべて吸収します。  
しかし、光のエネルギーが入ったら、次はどこへ行くのでしょう？  
エネルギーは必ず保存されるはずです。  

1858年、**バルフォア・スチュワート** は、黒体がエネルギーを吸収・放出する効率が最も高いことを発見しました。  
翌年、**グスタフ・キルヒホフ** は、黒体放射のスペクトルは物質の種類ではなく、温度だけに依存することを示しました。  

やがて科学者たちは、この不思議な輝きを表す方程式を提案しました。  
その中で、**ヴィルヘルム・ヴィーン (1896年)** の式は実験結果によく合いました：  

**ヴィーン（1896年）**  
$$u(\nu,T)=a\nu^{3}e^{-b\nu/T}$$  
$u$：特定の周波数における単位体積あたりのエネルギー密度  
$\nu$：周波数  
$T$：温度  
$a, b$：定数  

理論的な説明の試みもありました。1900年6月、レイリー卿は理論に基づく方程式を報告しました。  

**レイリー・ジーンズの法則（1900年）**  
$$du(\nu,T)=\frac{8\pi\nu^{2}}{c^{3}}Ud\nu=\frac{8\pi\nu^{2}kT}{c^{3}}d\nu$$  
$c$：真空中の光速 ($c=299792458~\mathrm{m/s}$)  
$k$：ボルツマン定数 ($k=1.380649×10^{−23}~\mathrm{J/K}$)  

しかし、大きな問題が起こりました。  
高い周波数では、この式は無限大のエネルギーを予測してしまったのです！  
物理学者たちはこれを **「紫外線の破局」** と呼びました。  
![ultraviolet catastrophe](https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/planck.png "\"Ultraviolet catastrophe\"")  

レイリー・ジーンズの法則は低周波では実験に合致し、ヴィーンの式は高周波ではうまくいきました — でもどちらも完全ではありませんでした。  

## 量子物理学の誕生

1900年12月、**マックス・プランク** はひらめき、思い切った考えを持ちました：  
光のエネルギーは連続的ではなく…*小さなパケット*で存在するのではないか？  

彼はこれらのパケットを **量子（quanta）** と名付けました。  

**量子仮説**  
$$E=n\epsilon=nh\nu$$  
$\epsilon$：光の単位エネルギー  
$h=6.62607015\times10^{-34}~\mathrm{J\cdot s}$：プランク定数  
$\nu$：周波数  

これが **量子物理学** の種となり、*量子* という言葉は「離散的なエネルギーの単位」を意味するようになりました。  

## 法則

エネルギーがこれらの量子の間でどのように分配されるかを記述するため、プランクは **ボルツマン分布** を適用しました：  

**ボルツマン分布**  
$$f(E)\propto e^{-E/kT}$$  
$f(E)$：エネルギー $E$ を持つ分子の数  
$E$：集合のエネルギー  
$k$：ボルツマン定数  
$T$：温度  

ここから、1モードあたりの平均エネルギーを導くことができます。この考え方はプランク自身のものではなく、1924年にボースとアインシュタインが提案しました。  
$$<E>=<f(n\epsilon)>=\frac{\sum_{n=0}^{\infty}n\epsilon e^{-n\epsilon/kT}}{\sum_{n=0}^{\infty}e^{-n\epsilon/kT}}=\frac{\epsilon}{e^{\epsilon/kT}-1}=\frac{h\nu}{e^{h\nu/kT}-1}$$  

これを物理定数と組み合わせると、次のようになります：  

**プランクの法則（周波数 $\nu$ 変数）**  
$$du(\nu,T)=\frac{8\pi\nu^{2}}{c^{3}}Ud\nu=\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu$$  

同様に波長で表すと：  
**プランクの法則（波長 $\lambda$ 変数）**  
$$du(\lambda,T)=\frac{8\pi hc}{\lambda^{5}}\cdot\frac{1}{e^{hc/\lambda kT}-1}d\lambda$$  

ついに、ヴィーン則とレイリー・ジーンズ則の間のギャップを埋める一つの式が誕生しました — 実験と理論の調和のメロディです。  

## プランクの法則の検証

良い理論は、必ず実験による検証に耐えなければなりません。  
プランクの法則は、これまでの観測結果を優雅に説明しました：  

**ステファン・ボルツマン則（1877年）**  
*黒体放射（または放射エネルギーの総量）は、温度の4乗に比例する。*  
$$M=\sigma T^{4}$$  

**ヴィーンの変位則（1896年）**  
*放射のピーク波長は温度に反比例する。*  
$$\lambda_{peak}=\frac{b}{T}$$  

プランクの式がどのようにこれらとつながるか、見てみましょう。  

### ステファン・ボルツマン則

プランクの法則を全周波数で積分すると、放射の総エネルギーが得られます：  
> $$\int du=\int_{0}^{\infty}\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu$$  
> 計算のために $x=h\nu/kT$、$dx=hd\nu/kT$ と置きます。  
> $$\int_{0}^{\infty}\frac{8\pi k^{3}T^{3}}{h^{2}c^{3}}\cdot\frac{x^{3}}{e^{x}-1}\cdot\frac{kT}{h}dx$$  
> この積分の値は次の通りです：  
> $$\int_{0}^{\infty}\frac{x^{3}}{e^{x}-1}dx=\frac{\pi^{4}}{15}$$  
> よって、  
> $$E=\int du=\frac{8\pi k^{3}T^{3}}{h^{2}c^{3}}\cdot\frac{\pi^{4}}{15}\cdot\frac{kT}{h}=\frac{8\pi^{5}k^{4}T^{4}}{15h^{3}c^{3}}$$  
> これで黒体の**総放射エネルギー**が得られました（単位=$\mathrm{J/m^3}$）。  
ステファン・ボルツマン則では**放射パワー**（単位=$\mathrm{W/m^2}$）を扱うため、総エネルギーを表面放射に変換するには $c/4$ を掛けます：  
> $$M=E\cdot\frac{c}{4}=\frac{2\pi^{5}k^{4}T^{4}}{15h^{3}c^{2}}=\sigma T^{4}$$  

**ステファン・ボルツマン則**  
$$M=\sigma T^{4}=\frac{2\pi^{5}k^{4}}{15h^{3}c^{2}}T^{4}$$  
$$\sigma=\frac{2\pi^{5}k^{4}}{15h^{3}c^{2}}=5.67\times10^{-8}~\mathrm{W/m^2\cdot K^4}$$  
定数 $\sigma$ は実験値と美しく一致しています。  

### ヴィーンの変位則

> ヴィーンの変位則は、どの波長（または周波数）で放射が最大になるかを示します。  
> $$\frac{d(du/d\lambda)}{d\lambda}=0$$  
> プランクの法則は波長で表すと：  
> $$\frac{du(\lambda,T)}{d\lambda}=\frac{8\pi hc}{\lambda^{5}}\cdot\frac{1}{e^{hc/\lambda kT}-1}$$  
> 置換 $\lambda=hc/xkT$, $d\lambda=-hcdx/x^{2}kT$ として簡単化します：  
> $$du(x,T)=-\frac{8\pi x^{5}k^{5}T^{5}}{h^{4}c^{4}}\cdot\frac{1}{e^{x}-1}dx$$  
> 次の式を解きます：  
> $$\frac{d}{dx}\left(\frac{x^{5}}{e^{x}-1}\right)=\frac{5x^{4}(e^{x}-1)-x^{5}e^{x}}{(e^{x}-1)^{2}}=0$$  
> $x\approx 4.9651$（数値解）から、  
> $$\lambda_{peak}=\frac{b}{T}\approx\frac{hc}{4.9651 k T}=\frac{2.90~\mathrm{mm\cdot K}}{T}$$  

温度が高いほど、ピーク波長は短くなり、赤 → 黄 → 白青へと輝きます。  

### $\nu\rightarrow0$

低周波では、レイリー・ジーンズ則が実験に合致します。  
> $$\lim_{\nu\rightarrow0}du(\nu,T)=\frac{8\pi kT\nu^{2}}{c^{3}}d\nu$$  
低周波でプランクの法則はレイリー・ジーンズ則に収束します。  

### $\nu\rightarrow\infty$

高周波では、ヴィーン則が実験に合致します。  
> $$\lim_{\nu\rightarrow\infty}du(\nu,T)=\frac{8\pi h\nu^{3}}{c^{3}}e^{-h\nu/kT}d\nu=a\nu^{3}e^{-b\nu/T}$$  
高周波ではプランクの法則はヴィーン則に近似されます。  

---
---

## プランクのアイデアと洞察

### 1900年10月：二つの法則の融合

プランクは、ヴィーン則とレイリー・ジーンズ則がそれぞれの領域でうまく機能することに気付きました。  
彼はこう考えました：両方とも、より深い真実の特別なケースではないだろうか？  

彼はエントロピーと熱力学を研究し、優雅な推論を通して、両方の挙動を滑らかにつなぐ新しい道を見つけました。  

> ヴィーン則では、エネルギーは周波数と温度の指数関数です。  
> 一方、レイリー・ジーンズ則では、エネルギーは温度そのものに比例します。  
> $$U_{Wien}\propto \nu e^{-b\nu/T}~(Wien)$$  
> $$U_{RJ}\propto T~(RJ)$$  
> この研究にはまず熱力学を適用しました。式で表すと：  
> $$dU=TdS-PdV$$  
> 実験は小さな穴のある箱で行われたため、系の体積は変化しません。  
> ![experiment](https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/experiment.jpg "Blackbody Radiation Experiment")  
> よって熱力学は次のように書けます：  
> $$dU=TdS,~\frac{\partial S}{\partial U}=\frac{1}{T}$$  
> プランクは二つの法則について ${\partial S}/{\partial U}$ を考察しました：  
> $$\frac{\partial S}{\partial U}=\frac{1}{T}\propto \ln(U)~(Wien)$$  
> $$\frac{\partial S}{\partial U}=\frac{1}{T}\propto \frac{1}{U}~(RJ)$$  
> さらに二階微分を考えると：  
> $$\frac{\partial^{2} S}{\partial U^{2}}\propto \frac{1}{U}~(Wien)$$  
> $$\frac{\partial^{2} S}{\partial U^{2}}\propto \frac{1}{U^{2}}~(RJ)$$  
> これにより、$(\partial^{2} S/\partial U^{2})^{-1}$ を U の多項式として表すことができます：  
> $$(\frac{\partial^{2} S}{\partial U^{2}})^{-1}\propto U~(Wien)$$  
> $$(\frac{\partial^{2} S}{\partial U^{2}})^{-1}\propto U^{2}~(RJ)$$  
> プランクは二つの多項式を次のように組み合わせました：  
> $$(\frac{\partial^{2} S}{\partial U^{2}})^{-1}=C_{1}U+C_{2}U^{2}$$  
> この結果、式の形は波長の形で次のようにまとめられました：  
> $$U=\frac{C\lambda^{-5}}{e^{c/\lambda T}-1}$$  

### 1900年12月：エネルギーの離散性

その年の後半、プランクはボルツマンの確率論を放射に応用しました — 空洞内に無数の小さな「エネルギー要素」があると想像したのです。  
$$\epsilon\epsilon\epsilon|\epsilon\epsilon|\epsilon|\epsilon\epsilon\epsilon|\epsilon\epsilon|\cdots$$  
ここで $\epsilon$ はエネルギーの単位です。  

プランクは組み合わせ論を用いて、これらの量子のすべての可能な配置を数えました：  
$$W=\frac{(P+N-1)!}{P!(N-1)!}$$  
ここで  
$P=UN/\epsilon$：エネルギー粒子の数、$U$：1つの光波のエネルギー  
$N$：光波の数  

> $N$ は非常に大きいため、$N-1\approx N$ と見なせます。  
> また、十分大きな数 $n$ について、$n!$ は次で近似できます：  
> $$n!\approx\sqrt{2\pi n}(n/e)^{n}~(n\rightarrow\infty)$$  
> $n^n$ は $\sqrt{n}$ よりはるかに大きいため、$W$ を次のように書けます：  
> $$W\approx \frac{(P+N)^{P+N}}{P^P N^N}$$  

そして、ボルツマンの原理に基づき、これをエントロピーに結び付けます：  
$$S=k\cdot \ln(W)$$  
$S$：系の絶対エントロピー  
$W$：微視的状態数（"*Wahrscheinlichkeit*"）  

> 熱力学の式を思い出すと：  
> $$\frac{1}{T}=\frac{\partial S}{\partial U}=k\frac{\partial(\ln W)}{\partial U}$$  
> $W$ の近似値を得たので、$\ln W$ を次のように書けます：  
> $$\ln W=(P+N)\ln(P+N)-P\ln P-N\ln N=\frac{N}{\epsilon}((U+\epsilon)\ln(U+\epsilon)-\epsilon\ln\epsilon-U\ln U)$$  
> よって、  
> $$k\frac{\partial(\ln W)}{\partial U}=\frac{kN}{\epsilon}(\ln(U+\epsilon)-\ln U)$$  
> 1つのエネルギー粒子については：  
> $$\frac{k}{\epsilon}(\ln(U+\epsilon)-\ln U)=\frac{1}{T}$$  
> よって、  
> $$U=\frac{\epsilon}{e^{\epsilon/kT}-1}=\frac{h\nu}{e^{h\nu/kT}-1}$$  

ここから、プランクの画期的な結果が生まれました：  
$$U=\frac{\epsilon}{e^{\epsilon/kT}-1}=\frac{h\nu}{e^{h\nu/kT}-1}$$  

これがプランクの有名な式です。  
各光波は $h\nu$ の整数倍のエネルギーしか持てません。  
エネルギーは連続的ではなく、離散的な量子で構成されていることを示しています。  

彼はエネルギー量子の発見により、**1918年のノーベル物理学賞**を受賞しました。  

> *1918年のノーベル物理学賞は、マックス・カール・エルンスト・ルートヴィヒ・プランクに「エネルギー量子の発見による物理学の発展への貢献」を称えて授与されました。*

この瞬間、人類は初めて量子世界の扉に触れました。  
科学の夜空に、知識の光が静かに輝いたのです。  
これが量子時代の夜明けであり、宇宙の最小の秘密に人類が初めて触れた瞬間でした。  

## 参考文献

Blackbody Radiation: Wikipedia (<https://en.wikipedia.org/wiki/Blackbody%20Radiation>)  
Planck's Law: Wikipedia (<https://en.wikipedia.org/wiki/Planck%27s%20Law>)  
Planck, M. (1900). Über eine Verbesserung der Wien’schen Strahlungsgleichung. *Verhandlungen der Deutschen Physikalischen Gesellschaft*.  
Planck, M. (1900). Zur theorie des gesetzes der energieverteilung im normalspektrum. *VhDPG*, 2, 238.  
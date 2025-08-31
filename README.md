<style>
/* === Base Reset === */
html, body {
  margin: 0 !important;
  padding: 0 !important;
  height: 100%;
  width: 100%;
  font-family: Arial, sans-serif;
  font-size: 18px;
  line-height: 1.6;
  color: #111827;
}

.markdown-body {
  max-width: 100% !important;
  margin: 0 !important;
  padding: 0 !important;
}

.markdown-body > :first-child { margin-top: 0 !important; }
.markdown-body > :last-child { margin-bottom: 0 !important; }

/* Hide default site title / anchors */
.markdown-body h1:first-child,
.markdown-body h1:first-child a,
h1::before,
header::before,
.page-header::before,
a.anchorjs-link {
  display: none !important;
  content: none !important;
  margin: 0 !important;
  padding: 0 !important;
}

/* === Headings === */
h1, h2, h3, h4, h5, h6 {
  margin: 0;
  padding: 0;
  font-weight: 600;
  text-align: center;
  border-bottom: none;
  margin-bottom: 15px;
}

h2::after {
  content: "";
  display: block;
  width: 5%;
  height: 6px;
  margin: 8px auto 0;
  border-radius: 10px;
  background-color: black;
}

h2.white-line::after {
  background-color: white;
}

/* Make section headings bigger: "Publication" & "Get In Touch" */
.section-heading {
  font-size: 2em;
  margin-bottom: 20px;
}

/* === Hero Section === */
.hero {
  width: 100%;
  padding: 100px 10%;
  background-color: #E4EBFF;
  text-align: center;
  color: #11182F;
  box-sizing: border-box;
}

.hero h1 {
  font-size: 2.3em;
  margin-bottom: 10px;
}

.hero p {
  font-size: 1.2em;
  max-width: 800px;
  margin: 0 auto;
  line-height: 1.5;
}

.hero a {
  color: #1a0dab;
  text-decoration: none;
}

/* === Publications Section === */
.publication-container {
  background-color: #F9FAFB;
  color: #111827;
  padding: 20px;
}

.publication {
  text-align: left;
  max-width: 800px;
  margin: 20px auto;
  padding: 15px 20px;
  box-sizing: border-box;
}

.publication strong,
.publication .conference {
  font-size: 1.2em; /* Paper title = Conference */
  color: #0366d6;
  display: block;
  margin-bottom: 6px;
  line-height: 1.3;
}

.publication .authors {
  font-size: 1em;
  color: #555;
  margin-bottom: 4px;
}

.publication .buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 6px;
}

.pub-btn {
  padding: 8px 14px;
  font-size: 0.95em;
  background-color: #0366d6;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.2s;
}

.pub-btn:hover {
  background-color: #0255b5;
}

.pub-btn img {
  vertical-align: middle;
  margin-right: 5px;
}

/* === Popups / Abstracts === */
.popupModal > div {
  width: 560px;
  max-width: 90%;
  height: 380px;
  overflow-y: auto;
  box-sizing: border-box;
  background: white;
  padding: 20px;
  border-radius: 10px;
  text-align: left;
  box-shadow: 0 5px 15px rgba(0,0,0,0.3);
}

.popupModal h2 {
  font-size: 1.3em;
  margin-top: 0;
}

.popupModal p, .popupModal pre {
  font-size: 1em;
  line-height: 1.5;
}

/* === Contact Section === */
.contact {
  width: 100%;
  padding: 50px 10%;
  background-color: #172554;
  color: white;
  text-align: center;
  box-sizing: border-box;
}

.contact h2 {
  font-size: 2em; /* Same as Publication heading */
  margin-bottom: 15px;
}

.contact h3 {
  font-size: 1.3em;
  font-weight: 400;
  margin-bottom: 12px;
}

.contact p {
  font-size: 1.2em;
  margin: 0;
}

.contact a {
  color: white;
  text-decoration: none;
}

.contact img {
  vertical-align: middle;
  margin-right: 5px;
}
</style>




<!-- # Noam Shenwald

I'm a PhD student in Computer Science at the Hebrew University of Jerusalem, advised by [Orna Kupferman](https://www.cs.huji.ac.il/~ornak/).  
My research focuses on the connection between reactive synthesis and algorithmic game theory. -->

<div style="width:100%; margin:0; padding:0; background-color:#E4EBFF; color:#11182F; box-sizing:border-box;">
  <div style="text-align:center; padding-left:10%; padding-right:10%; padding-top: 100px;padding-bottom: 100px; margin:0;">
    <div style="font-size: 2.3em; text-align: center; margin: 0; padding-bottom: 10px;">
  Noam Shenwald
</div>
    <p style="margin:0; font-size: 1.2em;">
      I'm a PhD student in Computer Science at the Hebrew University of Jerusalem, advised by 
      <a href="https://www.cs.huji.ac.il/~ornak/" target="_blank" style="color: #1a0dab; text-decoration: none;">
        Orna Kupferman</a>. My research focuses on the connection between reactive synthesis and algorithmic game theory.
    </p>
  </div>
</div>



<!-- Publications Section -->
<div style="margin-top: 0;margin-bottom: 0; padding: 20px 20px;background-color:#F9FAFB;color:#111827;">
<h2 style="text-align: center; margin: 0; display: block;">
  <img src="icons/book-icon.svg" width="24" style="background: transparent;vertical-align: middle;"/>
  <span style="vertical-align: middle;">Publications</span>
</h2>

<div style="margin-top: 0;margin-bottom: 0; padding:20px 0px;">

<!-- Publication 1 -->
<div class="publication">
  <strong>Coverage Games</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">CONCUR 2025</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract1').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib1').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/coverage games.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
    <button class="pub-btn" onclick="window.open('papers/coverage-games-full-version.pdf')">
      <img src="icons/full-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Full Version (under review)
    </button>
  </div>
</div>

<div id="abstract1" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>We introduce and study coverage games -- a novel framework for multi-agent planning in settings in which a system operates several agents but do not have full control on them, or interacts with an environment that consists of several agents. The game is played between a coverer, who has a set of objectives, and a disruptor. The coverer operates several agents that interact with the adversarial disruptor. The coverer wins if every objective is satisfied by at least one agent. Otherwise, the disruptor wins. Coverage games thus extend traditional two-player games with multiple objectives by allowing a (possibly dynamic) decomposition of the objectives among the different agents. They have many applications, both in settings where the system is the coverer (e.g., multi-robot surveillance, coverage in multi-threaded systems) and settings where it is the disruptor (e.g., prevention of resource exhaustion, ensuring non-congestion). We study the theoretical properties of coverage games, including determinacy, and the ability to a priori decompose the objectives among the agents. We solve the problems of deciding whether the coverer or the disruptor wins, analyze their tight complexity, and consider useful special cases.</p>
  </div>
</div>

<div id="bib1" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS25,
author    = {O. Kupferman and N. Shenwald},
title     = {Coverage Games},
booktitle =  concur25,
series    = {LIPIcs},
volume    = {?},
pages     = ?,
year      = {2025}
}
    </pre>
  </div>
</div>

<!-- Publication 2 -->
<div class="publication">
  <strong>Positional-Player Games</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">MFCS 2025</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract2').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib2').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/Positional-Player Games.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
  </div>
</div>


<div id="abstract2" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>In reactive synthesis, we transform a specification to a system that satisfies the specification in all environments. For specifications in linear-temporal logic, research on bounded synthesis, where the sizes of the system and the environment are bounded, captures realistic settings and has lead to algorithms of improved complexity and implementability. In the game-based approach to synthesis, the system and its environment are modeled by strategies in a two-player game with an ω-regular objective, induced by the specification. There, bounded synthesis corresponds to bounding the memory of the strategies of the players. The memory requirement for various objectives has been extensively studied. In particular, researchers have identified positional objectives, where the winning player can follow a memoryless strategy -- one that needs no memory. In this work we study bounded synthesis in the game setting. Specifically, we define and study positional-player games, in which one or both players are restricted to memoryless strategies, which correspond to non-intrusive control in various applications. We study positional-player games with Rabin, Streett, and Müller objectives, as well as with weighted multiple Buchi and reachability objectives. Our contribution covers their theoretical properties as well as a complete picture of the complexity of deciding the game in the various settings.</p>
  </div>
</div>

<div id="bib2" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS25b,
author    = {O. Kupferman and N. Shenwald},
title     = {Positional-Player Games},
booktitle =  mfcs25,
series    = {LIPIcs},
volume    = {?},
pages     = ?,
year      = {2025}
}
    </pre>
  </div>
</div>

<!-- Publication 3 -->
<div class="publication">
  <strong>Non-Zero-Sum Games with Multiple Weighted Objectives</strong>
  <div class="authors">Yoav Feinstein, Orna Kupferman, Noam Shenwald</div>
  <div class="conference">TACAS 2025</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract3').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib3').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/Non-Zero-Sum Games with Multiple Weighted Objectives.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
  </div>
</div>


<div id="abstract3" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>We introduce and study non-zero-sum multi-player games with weighted multiple objectives. In these games, the objective of each player consists of a set α of underlying objectives and a weight function w: 2^α -> ℤ that maps each subset X of α to the utility of the player when exactly all the objectives in X are satisfied. The weight functions lift the setting of non-zero-sum multi-player games to the general quantitative case, allowing a rich reference to the underlying objectives. We study the existence and synthesis of stable outcomes with desired utilities for the players. The problem generalizes rational synthesis and enables the synthesis of outcomes that satisfy wellness, fairness, and priority requirements. We study the extension of the game by payments, with which players can incentivize each other to follow strategies that are beneficial for the paying player. We show how such payments can be used in order to repair systems. We study the complexity of the setting for various classes of weight functions. In particular, general weight functions are related to Muller objectives, and the synthesis problem for them is PSPACE-complete. We study non-decreasing, additive, positive, and other classes of weight functions, and the way they affect the memory required for the players and the complexity of the synthesis problem.</p>
  </div>
</div>

<div id="bib3" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{FKS25,
author      =   "Yoav Feinstein and O. Kupferman and N. Shenwald",
title       =   "Non-Zero-Sum Games with Multiple Weighted Objectives",
booktitle   =   tacas25,
pages       =   "?",
series      =   lncs,
volume      =   "?",
publisher   =   springer,
year        =   2025
}
    </pre>
  </div>
</div>

<!-- Publication 4 -->
<div class="publication">
  <strong>Games with Weighted Multiple Objectives</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">ATVA 2024</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract4').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib4').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/Games with Weighted Multiple Objectives.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
  </div>
</div>


<div id="abstract4" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>Games with multiple objectives arise naturally in synthesis of reactive systems. We study games with weighted multiple objectives. The winning objective in such games consists of a set F of underlying objectives, and a weight function w: 2^F → N that maps each subset S of F to a reward earned when exactly all the objectives in S are satisfied. The goal of a player may be to maximize or minimize the reward. As a special case, we obtain games where the goal is to maximize or minimize the number of satisfied objectives, and in particular satisfy them all (a.k.a. generalized conditions). A weight function allows for a much richer reference to the underlying objectives: prioritizing them, referring to desired and less desired combinations, and addressing settings where we cannot expect all sub-specifications to be satisfied together. We focus on settings where the underlying objectives are all Buchi, co-Buchi, reachability, or avoid objectives, and the weight function is non-decreasing (a.k.a. free disposal). For each of the induced classes (that is, type of underlying condition, type of optimization, and type of weight function), we solve the problem of deciding the game and analyze its tight complexity. We also study the tight memory requirements for each of the players. Finally, we consider general weight functions, which make the setting similar to the one of Boolean Muller objectives.</p>
  </div>
</div>

<div id="bib4" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS24,
        author      =   "O. Kupferman and N. Shenwald",
        title       =   "Games with Weighted Multiple Objectives",
        booktitle   =   atva24,
        series      = {Lecture Notes in Computer Science},      
        pages = {110--132},
        volume = 15054,
publisher = {Springer}
        year        =   2024
}
    </pre>
  </div>
</div>
<!-- Publication 5 -->
<div class="publication">
  <strong>Games with Trading of Control</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">CONCUR 2023</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract5').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib5').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/Games with Trading of Control.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
    <button class="pub-btn" onclick="window.open('papers/games-with-trading-of-control-full-version.pdf')">
      <img src="icons/full-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Full Version (under review)
    </button>
  </div>
</div>


<div id="abstract5" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>The interaction among components in a system is traditionally modeled by a game. In the turned-based setting, the players in the game jointly move a token along the game graph, with each player deciding where to move the token in vertices she controls. The objectives of the players are modeled by ω-regular winning conditions, and players whose objectives are satisfied get rewards. Thus, the game is non-zero-sum, and we are interested in its stable outcomes. In particular, in the rational-synthesis problem, we seek a strategy for the system player that guarantees the satisfaction of the system's objective in all rational environments. In this paper, we study an extension of the traditional setting by trading of control. In our game, the players may pay each other in exchange for directing the token also in vertices they do not control. The utility of each player then combines the reward for the satisfaction of her objective and the profit from the trading. The setting combines challenges from ω-regular graph games with challenges in pricing, bidding, and auctions in classical game theory. We study the theoretical properties of parity trading games: best-response dynamics, existence and search for Nash equilibria, and measures for equilibrium inefficiency. We also study the rational-synthesis problem and analyze its tight complexity in various settings.</p>
  </div>
</div>

<div id="bib5" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS23,
  author    = {O. Kupferman and N. Shenwald},
  title     = {Games with Trading of Control},
  booktitle =  concur23,
  series    = {LIPIcs},
  volume    = {279},
  pages     = {19:1 -- 19:17},
  year      = {2023}
}
    </pre>
  </div>
</div>

<!-- Publication 6 -->
<div class="publication">
  <strong>The Complexity of LTL Rational Synthesis</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">TACAS 2022</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract6').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib6').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/The Complexity of LTL Rational Synthesis.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
    <button class="pub-btn" onclick="window.open('https://dl.acm.org/doi/10.1145/3648473')">
      <img src="icons/full-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Full Version (ACM ToCL 2024)
    </button>
  </div>
</div>


<div id="abstract6" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>In rational synthesis, we automatically construct a reactive system that satisfies its specification in all rational environments, namely environments that have objectives and act to fulfill them. We complete the study of the complexity of LTL rational synthesis. Our contribution is threefold. First, we tighten the known upper bounds for settings that were left open in earlier work. Second, our complexity analysis is parametric, and we describe tight upper and lower bounds in each of the problem parameters: the game graph, the objectives of the system components, and the objectives of the environment components. Third, we generalize the definition of rational synthesis, combining the cooperative and non-cooperative approaches studied in earlier work, and extend our complexity analysis to the general definition.</p>
  </div>
</div>

<div id="bib6" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS22,
        author      =   "O. Kupferman and N. Shenwald",
        title       =   "On the Complexity of LTL Rational Synthesis",
        booktitle   =   tacas22,
        pages       =   "25-45",
        series      =   lncs,
        volume      =   "13243",
        publisher   =   springer,
        year        =   2022
}
    </pre>
  </div>
</div>

<!-- Publication 7 -->
<div class="publication">
  <strong>Perspective Multi-Player Games</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">LICS 2021</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract7').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib7').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/Perspective Multi-Player Games.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
  </div>
</div>


<div id="abstract7" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>Perspective games model multi-agent systems in which agents can view only the parts of the system that they own. Unlike the observation-based model of partial visibility, where uncertainty is longitudinal -- agents partially observe the full history, uncertainty in perspective games is transverse -- agents fully observe parts of the history. So far, researchers studied zero-sum two-player perspective games. There, the objective of one agent (the system) is to satisfy a given specification, and the objective of the second agent (the environment) is to fail the specification. We study richer and more realistic settings of perspective games. We consider games with more than two players, and distinguish between zero-sum games, where the objectives of the players form a partition of all possible behaviors, zero-sum games among coalitions, where agents in a coalition share their objectives but do not share their visibility, and non-zero-sum games, where each agent has her own objectives and is assumed to be rational rather than hostile. In the non-zero-sum setting, we are interested in stable outcomes of the game; in particular, Nash equilibria. We show that, as is the case with longitudinal uncertainty, transverse uncertainty leads to undecidability in settings with three or more players that include coalitions or non-zero-sum objectives. We then focus on two-player non-zero-sum perspective games. There, finding and reasoning about stable outcomes is decidable, and in fact, unlike the case with longitudinal uncertainty, can be done in the same complexity as in games with full visibility. In particular, we study rational synthesis in the perspective setting, where the goal is to generate systems that satisfy their specification when interacting with rational environments. Our study includes Boolean objectives given by automata or LTL formulas, as well as a multi-valued setting, where the objectives are FLTL formulas with satisfaction values in [0,1], and the agents aim to maximize the satisfaction value of their objectives.</p>
  </div>
</div>

<div id="bib7" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS21,
        author      =   "O. Kupferman and N. Shenwald",
        title       =   "Perspective Multi-Player Games",
        booktitle   =   lics21,
        pages       =  "1--13",
        year        =  2021
}
    </pre>
  </div>
</div>

<!-- Publication 8 -->
<div class="publication">
  <strong>Perspective Games with Notifications</strong>
  <div class="authors">Orna Kupferman, Noam Shenwald</div>
  <div class="conference">FST&TCS 2020</div>
  <div class="buttons">
    <button class="pub-btn" onclick="document.getElementById('abstract8').style.display='flex'">
      <img src="icons/abstract-icon.svg" width="13" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>Abstract
    </button>
    <button class="pub-btn" onclick="document.getElementById('bib8').style.display='flex'">
      <img src="icons/bibtex-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>BibTeX
    </button>
    <button class="pub-btn" onclick="window.open('papers/Perspective Games with Notifications.pdf')">
      <img src="icons/pdf-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px;"/>PDF
    </button>
  </div>
</div>


<div id="abstract8" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">Abstract</h2>
    <p>A reactive system has to satisfy its specification in all environments. Accordingly, design of correct reactive systems corresponds to the synthesis of winning strategies in games that model the interaction between the system and its environment. The game is played on a graph whose vertices are partitioned among the players. Starting from an initial vertex, the players jointly generate a computation, with each player deciding the successor vertex whenever the generated computation reaches a vertex she owns. The objective of the system player is to force the generated computation to satisfy a given specification. The traditional way of modelling uncertainty in such games is observation-based. There, uncertainty is longitudinal: the players partially observe all vertices in the history. Recently, researchers introduced perspective games, where uncertainty is transverse: players fully observe the vertices they own and have no information about the behavior of the computation between visits in such vertices. We introduce and study perspective games with notifications: uncertainty is still transverse, yet a player may be notified about events that happen between visits in vertices she owns. We distinguish between structural notifications, for example about visits in some vertices, and behavioral notifications, for example about the computation exhibiting a certain behavior. We study the theoretic properties of perspective games with notifications, and the problem of deciding whether a player has a winning perspective strategy. Such a strategy depends only on the visible history, which consists of both visits in vertices the player owns and notifications during visits in other vertices. We show that the problem is EXPTIME-complete for objectives given by a deterministic or universal parity automaton over an alphabet that labels the vertices of the game, and notifications given by a deterministic satellite, and is 2EXPTIME-complete for LTL objectives. In all cases, the complexity in the size of the graph and the satellite is polynomial -- exponentially easier than games with observation-based partial visibility. We also analyze the complexity of the problem for richer types of satellites.</p>
  </div>
</div>

<div id="bib8" class="popupModal" style="display:none;position:fixed;z-index:1000;left:0;top:0;width:100%;height:100%;background-color:rgba(0,0,0,0.5);justify-content:center;align-items:center;">
  <div style="background:white;padding:20px;border-radius:10px;max-width:500px;text-align:left;box-shadow:0 5px 15px rgba(0,0,0,0.3);">
    <h2 style="margin-top:0;">BibTeX Citation</h2>
    <pre>
@inproceedings{KS20,
  author    = {O. Kupferman and N. Shenwald},
  title     = {Perspective Games with Notifications},
  booktitle = fsttcs20,
  volume = "182",
  pages = "51:1-51:16",
  series = {Leibniz International Proceedings in Informatics (LIPIcs)},
  year      = {2020}
}
    </pre>
  </div>
</div>
</div>
</div>



<!--## Contact Me-->

<div style="width:100%; margin:0 0; padding:50px 0; background-color:#172554; color:white; text-align:center; box-sizing:border-box;">
  <h2 class="white-line" style="text-align: center; margin: 0; display: block;">
  <img src="icons/bubble-icon.svg" width="24" style="background: transparent;vertical-align: middle;"/>
  <span style="vertical-align: middle;">Get In Touch</span>
</h2>

  <h3>
    I'm always interested in discussing research collaborations
  </h3>

  <p style="font-size: 1.2em;">
    <img src="icons/email-icon.svg" width="17" style="background: transparent; padding-right: 5px; vertical-align: middle; padding-bottom: 3px; padding-bottom: 2px;"/>firstname.lastname@mail.huji.ac.il
  </p>
</div>


<!-- JavaScript -->
<script>
document.querySelectorAll('.popupBtn').forEach(btn => {
  btn.onclick = () => {
    const modal = document.getElementById(btn.dataset.popup);
    modal.style.display = 'flex';
  };
});

// Close popup when clicking outside the content
document.querySelectorAll('.popupModal').forEach(modal => {
  modal.addEventListener('click', (e) => {
    if (e.target === modal) {  // click is on the overlay
      modal.style.display = 'none';
    }
  });
});
</script>

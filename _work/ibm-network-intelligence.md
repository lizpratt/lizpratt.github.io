---
title: "One customer, and a product about to be cancelled"
index: "02"
kicker: "Case study"
standfirst: "An agentic AI product for network operations with a single customer in Japan and a cancellation date approaching. The ask was to polish the interface. The finding was that nobody had established what job the product was for."
role: "Research lead, running the study personally while coaching a designer and a peer UXR lead"
org: "IBM Software with IBM Research, an internal technical incubation team"
period: "2024 to 2025"
methods: "SME listening tour, proto personas, JTBD interviews, ODI survey, journey mapping, Kano, concept testing across sprint cycles, private preview, retrospective"
share_image: "/assets/img/nwi/kano_map.png"
description: "How jobs-to-be-done and Kano prioritization turned IBM Network Intelligence from a cancellation candidate into a featured product at TechXchange 2025."
---

{% include chapter.html num="§ 01" title="The room I walked into" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>IBM Network Intelligence was agentic AI for network operations: anomaly detection, root cause
analysis, and automated remediation. When IBM Research brought it to my team in 2024, it had one
customer, in Japan, and it was heading toward a pause.</p>

<p>IBM Research had not historically been a research partner in the UX sense. Their mission is
"deliver what's next," which is a good mission, and in practice it meant the technology came first
and user needs were treated as optional.</p>

<p>Their ask was narrow. Help us iterate the digital experience, and review the sales materials.</p>

<p>My read was different. This was not an experience problem. It was a product-market fit problem,
and no amount of interface polish was going to rescue a product that had never been validated
against a real user need.</p>

</div>
</div>
</div>

{% include fig.html num="01" src="/assets/img/nwi/complexity_trap.png" caption="The hypothesis that had produced the product. Designing for one large, complex customer generates a great many features and not a great deal of value." %}

{% include chapter.html num="§ 02" title="Agreeing to help, then changing the question" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>I said yes to the ask, and then proposed we redefine the problem before answering it. Rather than
validate the solution that already existed, we would first establish what problems the product solved
and for whom.</p>

<p>Framing matters when you are asking a technology organization to slow down. I framed the research
goals in the language IBM Research already used: build a foundation for data-driven product
decisions that creates a credible path to real-world adoption. Not "your product has no users." Not
"you skipped discovery." A foundation, and a path.</p>

<p>The program covered the full discovery arc. A listening tour with subject matter experts. Proto
personas built from interviews and desk research. Journey mapping. A jobs-to-be-done analysis using
interviews plus outcome-driven innovation survey methodology. Then rapid concept testing folded into
sprint cycles, a private preview, and a retrospective.</p>

</div>
</div>
</div>

{% include fig.html num="02" src="/assets/img/nwi/research_roadmap.png" caption="The research roadmap, redrawn. Every phase has a named output and a decision it feeds, which is what made it possible to hold the timeline against engineering pressure." %}

{% include chapter.html num="§ 03" title="Naming the job" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>Jobs-to-be-done did the heavy lifting here, for a specific reason. A job statement is falsifiable
in a way that a feature request is not. When a product manager says users want better dashboards and
a network operations analyst says they need to know within ninety seconds whether an alarm is real,
those two statements are not in the same category, and only one of them can be tested.</p>

<p>The analysis produced one core job and seven high-priority jobs, laid out as a job map across seven
stages. From there we translated each job statement into a job task workflow that names the actor,
the system, the task, and the friction. That translation step is the part teams usually skip, and it
is the part that makes a job statement actionable by a designer.</p>

</div>
</div>
</div>

{% include fig.html num="03" src="/assets/img/nwi/jtbd_map.png" caption="The job map. One core job, seven high-priority jobs, arranged across seven stages of the work." source="Participant counts on this artifact are illustrative. See the note at the end of this page." %}

<div class="grid">
<div class="col-main">
<div class="prose">
<p>Three of those workflows carried most of the product's value, and each one exposed a different
kind of friction.</p>
</div>
</div>
</div>

{% include fig.html num="04" src="/assets/img/nwi/wf_triage.png" caption="Triage. A Tier-1 analyst deciding whether an alarm deserves a human at all." %}

{% include fig.html num="05" src="/assets/img/nwi/wf_diagnose.png" caption="Diagnose. A Tier-2 specialist assembling a causal story from evidence scattered across three systems." %}

{% include fig.html num="06" src="/assets/img/nwi/wf_remediate.png" caption="Remediate. A network engineering SME deciding whether to trust an automated action, and what happens when they do not." %}

{% include chapter.html num="§ 04" title="Where the work actually happens" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The journey map is a six-lane swimlane, and the six lanes are the finding. Three human roles: the
Tier-1 NOC analyst, the Tier-2 NOC specialist, and the network engineering SME. Three systems: SevOne
NPM and Mist, Network Intelligence itself, and the ITSM stack of ServiceNow and Slack.</p>

<p>Laid out this way, one thing becomes obvious. Network Intelligence was designed as though it were
the place the work happened. In the actual workflow it is one lane of six, and the handoffs between
lanes are where incidents go to die.</p>

</div>
</div>
</div>

{% include fig.html num="07" src="/assets/img/nwi/swimlane.png" caption="Six lanes: three roles and three systems. The product occupies one of them." %}

<div class="statement reveal">
  <p>The product was not competing with other products. It was competing with the <em>handoffs.</em></p>
</div>

{% include chapter.html num="§ 05" title="Eighteen capabilities, and the case for cutting thirteen" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The hardest influence problem on this program was persuading an organization that had spent years
building feature-first to make a decision data-first. Arguing about philosophy would have gone
nowhere. What worked was meeting them at their own standard of evidence.</p>

<p>So the prioritization was built to be statistically defensible rather than persuasive. Eighteen
candidate capabilities went into a Kano survey. The output was a ranked set with satisfaction and
dissatisfaction coefficients attached, which meant the conversation stopped being about whose
judgment was better and started being about what the data supported.</p>

<p>Five capabilities came out of it:</p>

<ol>
<li>Anomaly detection with noise suppression</li>
<li>Ranked root-cause hypotheses</li>
<li>Visible reasoning and an evidence trail</li>
<li>Remediation grounded in the customer's own runbooks</li>
<li>An automatic ITSM ticket that carries the hypothesis with it</li>
</ol>

<p>The third one is the interesting one. In an agentic product, showing the reasoning is not a
transparency nicety. It is the mechanism by which a Tier-2 specialist decides whether to act, and
without it the other four capabilities generate work rather than removing it.</p>

</div>
</div>
</div>

{% include fig.html num="08" src="/assets/img/nwi/kano_map.png" caption="The Kano map. Eighteen capabilities plotted by satisfaction and dissatisfaction coefficient." source="Coefficient values shown are illustrative and internally consistent. See the note at the end of this page." %}

{% include fig.html num="09" src="/assets/img/nwi/kano_cut.png" caption="The cut. Build, later, and not yet, with the reasoning attached to each band so the decision could be re-litigated on evidence rather than on memory." %}

{% include fig.html num="10" src="/assets/img/nwi/evidence_ladder.png" caption="How the study was kept honest. Each claim in the final recommendation is tagged with the strength of evidence behind it, so a reader can see the difference between a finding and a hypothesis." %}

{% include chapter.html num="§ 06" title="Design, and what the research changed" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The prototype went through three iterations. Testing surfaced 21 potential improvements, which we
grouped into four themes and narrowed to nine high-impact recommendations for the anomaly detection
experience.</p>

<p>The before and after pairs below are the ones worth showing, because in each case the change is
not cosmetic. It is a different answer to the question of what the interface owes the user.</p>

</div>
</div>
</div>

{% include pair.html num="11" a_label="Iteration 1" a_src="/assets/img/nwi/wire_v1.png" b_label="Iteration 3" b_src="/assets/img/nwi/wire_v2.png" caption="The structural shift across iterations. Version one presents everything the system knows. Version three presents a decision and the evidence for it." %}

{% include pair.html num="12" a_label="Before" a_src="/assets/img/nwi/cap1_before.png" b_label="After" b_src="/assets/img/nwi/cap1_after.png" caption="Anomaly detection with noise suppression. The before state reports every anomaly with equal weight, which is the same as reporting none." source="Interface studies are reconstructions built from shipped IBM Network Intelligence documentation on ibm.com/docs." %}

{% include pair.html num="13" a_label="Before" a_src="/assets/img/nwi/cap3_before.png" b_label="After" b_src="/assets/img/nwi/cap3_after.png" caption="Visible reasoning and evidence trail. The after state shows the chain the system followed, which is what makes an automated recommendation something a specialist can accept or reject on the merits." source="Reconstruction from public documentation." %}

{% include pair.html num="14" a_label="Before" a_src="/assets/img/nwi/cap5_before.png" b_label="After" b_src="/assets/img/nwi/cap5_after.png" caption="The ITSM handoff. The ticket now carries the hypothesis and the evidence into ServiceNow, so the analysis survives the lane change that used to lose it." source="Reconstruction from public documentation." %}

{% include chapter.html num="§ 07" title="The finding that changed how it was sold" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The most consequential insight of the whole program was not about the interface at all.</p>

<p>Network Intelligence's agentic AI was strongest not as a standalone product but packaged inside the
established IBM Software networking offerings, NS1 and SevOne, for enterprise customers, while
standing alone for small and mid-size businesses. Two different products for two different buyers,
from one codebase.</p>

<p>That redirected the sales approach and reframed how the product was positioned at TechXchange. It
also strengthened cross-collaboration between teams that had been operating as though they were in
different companies.</p>

<p>Research that changes the go-to-market model is unusual, and I think it happens for a boring
reason: we asked who the product was for before we asked what it should do.</p>

</div>
</div>
</div>

{% include chapter.html num="§ 08" title="Clarity is kind" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>I ran this research personally while coaching a designer and a peer UXR lead, neither of whom had
worked inside IBM Research's culture before. The research was not the hard part. The hard part was
holding momentum in an environment where the partners had no established process for acting on a
finding.</p>

<p>So I set explicit rules of engagement at the start. What research would and would not answer. How
findings would be reviewed and prioritized. What decision rights each team held. The phrase I used
with my team throughout was "clarity is kind," and it applied to every stakeholder conversation on
the program, including the uncomfortable ones.</p>

<p>I also used this project deliberately to build things that would outlast it: templates, process
guides, and a cross-collaboration model that a future researcher could pick up and use in a similar
environment. The design lead I coached moved onto a Design Principal promotion path.</p>

</div>
</div>
</div>

{% include chapter.html num="§ 09" title="Outcomes" %}

<div class="grid">
<div class="col-main">

<div class="ledger reveal">
  <div class="ledger__row">
    <div class="ledger__fig">1 <span class="unit">&rarr; TechXchange</span></div>
    <div class="ledger__txt">From one customer and cancellation risk to a featured product at IBM TechXchange 2025</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">18 <span class="unit">&rarr; 5</span></div>
    <div class="ledger__txt">Candidate capabilities narrowed to a statistically prioritized top five</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">1 + 7</div>
    <div class="ledger__txt">One core job and seven high-priority jobs defined, with job task workflows for each</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">21 <span class="unit">&rarr; 9</span></div>
    <div class="ledger__txt">Potential improvements identified, narrowed to nine high-impact recommendations for the anomaly detection prototype</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">1</div>
    <div class="ledger__txt">IBM Excellence in Product Leadership, awarded to the user research team</div>
  </div>
</div>

<div class="prose" style="margin-top:2.5rem">
<h3>What this one taught me</h3>
<p>A narrow ask is usually a symptom. When a team asks for interface help on a product with one
customer, the interface is rarely the thing that is broken, and saying so on day one would have ended
the engagement. Agreeing to the ask, and then earning the right to change the question, is how the
work got done. I would take that approach again.</p>
</div>

<div class="note">
  <strong>A note on the artifacts</strong>
  Everything narrative on this page is from the work as it happened: the core job statement, the one
  plus seven job structure, the eighteen-to-five narrowing, the 21 improvements and 9 high-impact
  recommendations, the packaging finding, the TechXchange outcome, and the award. The interface
  studies are reconstructions built from shipped IBM Network Intelligence documentation published on
  ibm.com/docs, because the original design files are not mine to publish. Kano coefficient values,
  participant counts, alarm volumes, and segment percentages shown in the diagrams are illustrative
  and internally consistent; they demonstrate the method and the shape of the result rather than
  reporting IBM's figures.
</div>

</div>
</div>

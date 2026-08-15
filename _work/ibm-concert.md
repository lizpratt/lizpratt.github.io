---
title: "Three ways of showing up"
index: "01"
kicker: "Case study"
standfirst: "IBM Concert was built to pull siloed products into one decision layer. Post-launch research found that customers wanted the capability and refused the destination. Here is how that finding survived contact with executive sponsors, and the design pattern it produced."
role: "UXR Program Director, owning the research workstream from discovery through GA and post-launch iteration"
org: "IBM Software, Austin"
period: "2023 to 2025"
methods: "Design thinking workshops, Kano surveys, generative interviews, concept testing, private previews, post-launch evaluative research"
team: "Researchers embedded in sprint cycles across the Concert program, inside a 20-offering research portfolio"
share_image: "/assets/img/concert/wf_choice_dashboard_vs_panel.png"
description: "How research at IBM redirected Concert from an integration-first platform to progressive disclosure, producing the IBM Sidekick pattern."
---

{% include chapter.html num="§ 01" title="The directive" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>In 2023, two IBM executives said out loud what a lot of people had been thinking. IBM was big, it
was bloated, and it needed to move faster. The mandate that followed was to coordinate existing IBM
offerings into a single platform aimed at the operational pain enterprise IT actually feels:
application sprawl, vulnerability management, and operational resilience.</p>

<p>The result was IBM Concert, built on watsonx.ai and Granite.</p>

<p>The research challenge had three parts, and they pulled against each other. Define what this
platform should do rather than what the technology could do. Move fast enough to keep pace with
engineering timelines that had already been compressed. And make the findings influential enough to
shape a roadmap that was already carrying executive expectations.</p>

</div>
</div>
</div>

{% include chapter.html num="§ 02" title="Making research structural instead of optional" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The first thing I did was argue for a full-lifecycle research roadmap. Not a usability test bolted
onto the end of a release, but research present at every phase, with the deliverables and the timing
agreed in advance.</p>

<p>The second thing mattered more. I worked with product and engineering leadership to get UXR tags
on every Epic in the development roadmap. That sounds like process housekeeping. It was not. It
created a structural record of which research finding produced which piece of the product, which
meant that at any point in the program I could show a sponsor the line from a study to a shipped
journey. Influence you can trace is influence you can defend.</p>

<p>In discovery I prioritized a design thinking workshop to align siloed teams before any features
were committed, then ran Kano surveys and interviews so prioritization happened with data rather
than by the loudest voice in the room. That framing, data over opinion, became the operating
language between research and product leadership for the rest of the program.</p>

</div>
</div>
</div>

{% include chapter.html num="§ 03" title="Concert 1.0: a place you go" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The first version of Concert was a destination. You left the console you were working in, you
arrived, you picked a dimension off a ring, and you drilled until you found the thing. Insight lived
in one room. Action lived in another.</p>

<p>It is a defensible design for a platform whose whole promise is unification. If the value is that
six things are finally in one place, then a home that shows you all six is the honest expression of
that value.</p>

<p>It also asks the user to do something before they can do anything: focus the view.</p>

</div>
</div>
</div>

{% include pair.html num="01" a_label="Wireframe" a_src="/assets/img/concert/wf_1_0_destination.png" b_label="Shipped" b_src="/assets/img/concert/sc_1_0.png" caption="Concert 1.0. The six-segment dimension ring, the prompt to select a dimension, and the CVE rail down the right side." source="Wireframe is representative, not a tracing. Every structural element is traceable to the shipped screen beside it; all values in the wireframe are neutral placeholders." %}

{% include chapter.html num="§ 04" title="The finding nobody had ordered" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The most consequential research on this program happened after launch, which is exactly when
research budgets usually get reassigned.</p>

<p>Discovery work found that users wanted access to Concert's capabilities and did not want the
complexity of a fully integrated platform. Customers who already carried an impression of IBM as
robust and complicated were not resonating with an integration-first value proposition. The 2.0
features were considered valuable. The way they were going to be delivered increased cognitive load,
and users said so.</p>

<p>That is an awkward finding to carry into a room of executive sponsors twelve months into a
high-visibility program. Suppressing it was an option. I presented it instead, with a recommendation
attached: design for progressive disclosure, and give users control over when and how information
appears.</p>

</div>
</div>
</div>

<div class="statement reveal">
  <p>Reframing the strategy from <em>integration-first</em> to <em>user-control-first</em> was not a design preference. It was what the evidence said.</p>
  <div class="attrib">Post-launch research recommendation, IBM Concert</div>
</div>

{% include chapter.html num="§ 05" title="The argument that actually moved the room" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The recommendation landed because I did not present it as a list of usability complaints. I
presented the theory first and the findings as evidence for it.</p>

<p>Situational Awareness, in the human factors literature, is a state of knowledge and the set of
processes a person uses to reach it. Once the room had that frame, the interview data stopped looking
like preference and started looking like a predictable consequence: the conceptual designs and
workflows were asking users to rebuild their state of knowledge from scratch every time they arrived
at Concert, in a context where they already had one.</p>

<p>This is what a doctorate in I/O psychology and human factors is actually for. Not the credential.
The ability to name the mechanism underneath a finding, so that a decision-maker can reason forward
from it instead of just accepting or rejecting a data point.</p>

<p>The executives accepted the pivot.</p>

</div>
</div>
</div>

{% include chapter.html num="§ 06" title="Concert 2.0: a layer over the work" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>The redesign came out of a coffee chat in an IBM breakroom. Someone was talking to us while
managing tasks across several applications, never losing the thread of either conversation. Watching
that window management is what produced the answer.</p>

<p>In 2.0, Concert stopped being a place and became a panel. It arrives inside the console the user
already had open, scoped to one entity, stacking status-coded sections from the products that feed it
and closing when the user is done with it. Same job. No new destination, and no dashboard sprawl.</p>

<p>The breakroom conversation also turned into a recurring series of in-person meetups where IBMers
bring design problems and talk them through over coffee. Good outcomes, and a real channel for people
to build a reputation inside a very large company.</p>

</div>
</div>
</div>

{% include pair.html num="02" a_label="Wireframe" a_src="/assets/img/concert/wf_2_0_layer.png" b_label="Shipped" b_src="/assets/img/concert/sc_2_0.png" caption="Concert 2.0 inside IBM Turbonomic. The host application keeps its chrome; Concert occupies roughly a third of the width, scoped to a named entity, with recommended actions at the bottom of the panel." source="Wireframe is representative. Structural elements are traceable to the shipped screen; values are neutral placeholders." %}

{% include chapter.html num="§ 07" title="Dashboard, or side panel" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>This was the decision the whole program turned on, so it is worth showing both options honestly.</p>

<p>A dashboard makes the platform legible. Everything the platform knows is visible in one view, which
is a real argument when the platform is the product being sold. A side panel makes the platform
useful. It concedes the destination and wins the workflow.</p>

<p>We chose the panel. The result was IBM Sidekick, a collapsible sidebar carrying a unified view of
key signals, health indicators, and recommendations, without forcing anyone into a monolithic
interface. It took the highest internal award at IBM TechXchange 2025, and it was reused across three
of the core products folded into Concert, then picked up by other IBM business units working against
the same "better together" mission.</p>

<p>The wider lesson the story carried inside IBM: a list of features no longer sells a product.
Features integrated in a way that respects the user's existing state of knowledge do.</p>

</div>
</div>
</div>

{% include fig.html num="03" src="/assets/img/concert/wf_choice_dashboard_vs_panel.png" caption="The choice, side by side. Left, insight as a destination. Right, insight as a layer over work already in progress." source="Schematic abstraction of the two options, not a capture of either." %}

{% include chapter.html num="§ 08" title="Concert 2.5: the arc past my tenure" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>Concert 2.5 was announced publicly in May 2026. The role picks the view, the headline is written
for you, and every metric arrives already interpreted. The interface has stopped being a surface you
read and started being something you talk to.</p>

<p>I want to be precise about this one. I set the direction the product kept walking. I did not ship
2.5. It is here because the arc is the argument, and the arc only makes sense with the third point on
it.</p>

<p>One line for a room: 1.0 asked the user to focus the view. 2.5 focuses it for them.</p>

</div>
</div>
</div>

{% include pair.html num="04" a_label="Wireframe" a_src="/assets/img/concert/wf_2_5_interlocutor.png" b_label="Shipped" b_src="/assets/img/concert/sc_2_5.png" caption="Concert 2.5. Role-adaptive views, agentic workflows with a human in the loop, and interpretation delivered rather than assembled." source="Announced May 2026, after my tenure. Included to complete the arc." %}

{% include fig.html num="05" src="/assets/img/concert/platform_architecture.png" caption="Where the argument ended up. One backend, three role-scoped views. The sources and the intelligence stayed constant; what changed was the surface, and which decision each role was trying to reach." source="Synthetic reconstruction built for portfolio use. No IBM confidential material." %}

{% include chapter.html num="§ 09" title="Running the team through it" %}

<div class="grid">
<div class="col-main">
<div class="prose">

<p>A high-visibility, executive-priority program is a difficult place to be a researcher. Several
product stakeholders will each believe your researcher works for them.</p>

<p>Most of my job was buffering. I set research priorities clearly enough that individual researchers
were not being pulled in three directions, and I ran weekly research readouts so findings stayed
visible at the product level and every researcher could see the line from their study to a decision.</p>

<p>The choice I fought hardest for was keeping researchers embedded in sprint cycles rather than
running in parallel. That took repeated negotiation with engineering leads for access. It paid for
itself: researchers could iterate in real time instead of arriving with findings after the decision
had already been made.</p>

<p>The team also built the Design Partner Program, which enrolled more than 200 Concert customers and
gave the roadmap a structured external voice. Partners joined private previews on a sprint cadence
ahead of launches. The research operations infrastructure behind it was replicated by other IBM
Software teams, and we were funded to run the Experience Zone at IBM Think 2024 and TechXchange 2025
so we could collect feedback and grow the participant pool at the same time.</p>

</div>
</div>
</div>

{% include chapter.html num="§ 10" title="Outcomes" %}

<div class="grid">
<div class="col-main">

<div class="ledger reveal">
  <div class="ledger__row">
    <div class="ledger__fig">80<span class="unit">+</span></div>
    <div class="ledger__txt">Mixed-method research sessions across the program</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">150<span class="unit">+</span></div>
    <div class="ledger__txt">IBM customers tested, from a pool of 500+ potential customers evaluated</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">130</div>
    <div class="ledger__txt">Findings that drove the release of 12 core product journeys, each tagged to the research insight behind it</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">200<span class="unit">+</span></div>
    <div class="ledger__txt">Customers enrolled in the Design Partner Program</div>
  </div>
  <div class="ledger__row">
    <div class="ledger__fig">3</div>
    <div class="ledger__txt">Awards: Red Dot Design Award (Concert 2025), Outstanding Technical Achievement (Concert 2024), and the highest internal award at TechXchange 2025 for IBM Sidekick</div>
  </div>
</div>

<div class="prose" style="margin-top:2.5rem">
<h3>What I would do differently</h3>
<p>The pivot was accepted on the strength of the theory and the qualitative evidence. What I did not
build, and wish I had, was the measurement to close it: task time and confidence scores on the panel
against the dashboard, collected before and after. The argument was right. It would have been
unarguable with a number attached, and that is the piece I now design into a program from the start.</p>
</div>

<div class="note">
  <strong>A note on the artifacts</strong>
  The wireframes on this page are representative rather than tracings. Every structural element
  (navigation, the dimension ring, panel sections, card layout, the assistant rail) is traceable to
  something visible in the screenshot beside it. Nothing structural is invented. All numeric values in
  the wireframes are neutral placeholders, and entity names are generic, because the sketch is there
  to show the thinking and the screenshot is there to show the product.
</div>

</div>
</div>

<!--
link: https://cdn.jsdelivr.net/gh/posetgar/preserving_data_training_test@main/style/ugent-theme.css

title: Research Data Management in practice
author:     Paula Oset Garcia
email:      rdm.support@ugent.be
comment:    This course introduces...
icon:       https://styleguide.ugent.be/files/uploads/logo_UGent_EN_RGB_2400_kleur_witbg.png
repository: https://github.com/posetgar/preserving_data_course
language:   en
@MERMAID:   true
mode: section
-->

#  RDM Training Design & Evaluation in Practice

This course corresponds to Module 4.2 in the [University of Vienna Data Steward Certificate Course.](https://rdm.univie.ac.at/data-stewards-at-the-university/become-a-data-steward/)

---

<h2>Course information</h2>

<h3>Course description</h3>
This session provides a practical introduction to designing and evaluating training in the domain of Research Data Management (RDM). It builds on the basic didactic concepts introduced in the previous session (4.1) and applies them through the design of an RDM training. In this follow-up session, the focus shifts from theory to practice. We will concentrate on actively thinking through how RDM training can be designed, adapted, and evaluated in your own context. Working in small groups, you will identify training needs, define the characteristics of your target audience, formulate learning objectives, and explore suitable learning activities.

By the end of the session, you will have taken the first steps toward developing an RDM training concept that is aligned with learner needs, supported by clear outcomes, and grounded in thoughtful instructional design.

During the session, the following topics will be addressed:

- Brief introduction to Ghent University Data Stewards training  
- Training example: mapping an RDM course delivered by Ghent University data stewards to the ABC learning design method  
- Overview of different RDM learning activities  
- Evaluating and adapting training: how to include evaluation in training and adapt according to feedback or delivery method  
- Hands-on work: getting started with the design of RDM training


<div class="ugent-box ugent-example">
<h3>Learning outcomes</h3>
<p>Upon completion of this session, students will be able to:</p>

<p>- Explain why investing time in training design is essential and describe the overall training lifecycle (from needs analysis to evaluation)</p>
<p>- Analyze the characteristics and needs of the target audience</p>
<p>- Identify and define the topics, learning objectives, and outcomes for the course</p>
<p>- Propose appropriate learning activities and learning types for the different course topics</p>
<p>- Sketch a plan to include assessment and feedback mechanisms for the course</p> 
<p>- Evaluate the effectiveness of the learning activities proposed by peers</p>
<p>- Process and incorporate feedback into their own training design or concept</p> 
<p>- Develop a sense of ownership and responsibility for their own learning</p>
</div>


<h3>Methods</h3>
This lesson includes short lectures and group discussion, as well as smaller group work tasks. It is an interactive session involving knowledge-sharing and discussion among learners.

<h3>Assignment</h3>
Individually designing a training concept using the template given (2-3 pages).
The details of the assignment will be discussed during the live session and uploaded to Moodle.

<div class="ugent-box ugent-example">
<h3>Example</h3>
<p>This is an example with UGent styling.</p>
</div>

<div class="ugent-box ugent-activity">
<h3>Activity</h3>
<p>Try applying the ADDIE model to your own training.</p>
</div>

<div class="ugent-box ugent-learning">
<h3>Learning Outcome</h3>
<p>You will be able to identify key instructional design principles.</p>
</div>

<div class="ugent-box ugent-warning">
<h3>Warning</h3>
<p>Do not skip the analysis phase—it saves time later!</p>
</div>

## Why spending time on training design?

<h3>Slides</h3>
<iframe
  src="https://ugent.h5p.com/content/1292761112369681927/embed"
  width="100%"
  height="670"
  frameborder="0"
  allowfullscreen="allowfullscreen"
  allow="geolocation *; microphone *; camera *; midi *; encrypted-media *">
</iframe>

<h3>Introduction</h3>
In the last two previous years, we asked participants of the module how much time they spent on different aspects of training design? These were the results:

<!-- Chart.js library -->
https://cdn.jsdelivr.net/npm/chart.js</script>

<!-- Canvas placeholder -->
<canvas id="rdm-radar" style="max-width: 760px; width: 100%;"></canvas>

<script>
(async () => {
  // 1) Load CSV (raw GitHub URL to your CSV file)
  const csvUrl = "https://raw.githubusercontent.com/posetgar/preserving_data_training_test/main/data/training_design_time.csv";

  const text = await fetch(csvUrl).then(r => r.text());
  const rows = text.trim().split(/\r?\n/).map(r => r.split(","));

  // 2) Extract labels & datasets
  const headers = rows[0];                    // ["Aspect","2024","2025"]
  const labels  = rows.slice(1).map(r => r[0]);
  const y2024   = rows.slice(1).map(r => +r[1]);
  const y2025   = rows.slice(1).map(r => +r[2]);

  // UGent colors
  const UGENT_BLUE   = "#1E64C8";
  const UGENT_YELLOW = "#FFD200";

  // 3) Create radar chart
  const ctx = document.getElementById("rdm-radar").getContext("2d");
  new Chart(ctx, {
    type: "radar",
    data: {
      labels,
      datasets: [
        {
          label: headers[1] || "2024",
          data: y2024,
          backgroundColor: "rgba(30,100,200,0.25)",
          borderColor: UGENT_BLUE,
          pointBackgroundColor: UGENT_BLUE,
          borderWidth: 2
        },
        {
          label: headers[2] || "2025",
          data: y2025,
          backgroundColor: "rgba(255,210,0,0.25)",
          borderColor: UGENT_YELLOW,
          pointBackgroundColor: UGENT_YELLOW,
          borderWidth: 2
        }
      ]
    },
    options: {
      responsive: true,
      plugins: {
        legend: { position: "top" },
        tooltip: { enabled: true },
        title: {
          display: true,
          text: "How much time do you spend on different aspects of training design?"
        }
      },
      scales: {
        r: {
          suggestedMin: 0,
          suggestedMax: 5,
          ticks: { stepSize: 1 }
        }
      }
    }
  });
})();
</script>


Scale

**1** I do not spend any time on this aspect
**2** I spend **little** time on this aspect
**3** I spend a **moderate** amount of time on this aspect
**4** I spend **quite a lot** of time on this aspect
**5** I spend **most** of my time on this aspect


| Aspect                               | Average (2024–2025) |
| ------------------------------------ | -------------------:|
| Analyzing training needs             |                 2.9 |
| Defining learning objectives/outcomes|                 2.7 |
| Defining the audience                |                 2.6 |
| **Creating content & learning activities** |               **4.3** |
| Designing assessment methods         |                 2.1 |
| Training evaluation                  |                 1.8 |

As you can see, most people spend most of their time in creating content, spend the least ammount of time in assessment and evaluation, and spend limited ammount of time in the training design phase.


<h3> Why spending time on training design? </h3>

Good training does not happen by accident. Investing time in training design ensures that the learning experience is purposeful, relevant, and effective. By consciously planning who the training is for, what it should achieve, and how it will be delivered, you create a structure that supports both the trainer and the learners.

<details>
  <summary><strong>1. Align training with real needs</strong></summary>

If you understand who your learners are and what they struggle with, you can tailor the training to what truly matters.

**Tip:** Instead of giving a generic RDM overview to postdocs, you focus on *GDPR in practice* and *repository selection* because that’s where they typically struggle.

</details>

<details>
  <summary><strong>2. Define clear learning outcomes</strong></summary>

Clear outcomes help you decide what to include, what to skip, and how to check whether learning occurred.

**Tip:** Instead of “understand DMPs”, define: *“Learners can complete the data summary table for their own project.”* For policy sessions: *“Learners can identify which RDM and Open Science policies apply to their project.”*

</details>

<details>
  <summary><strong>3. Choose appropriate learning activities</strong></summary>

Spending time on designing makes you plan **how** learners will learn, not just **what** you will present. Learning activities become meaningful, because they support specific outcomes.

**Tip:** Rather than only presenting slides about file naming, use a short activity where they fix poorly named files. Instead of just showing a FAIR checklist, ask learners to compare datasets in repositories and discuss FAIRness.

</details>

<details>
  <summary><strong>4. Increase engagement and motivation</strong></summary>

Good design keeps learners active rather than passive.

**Tip:** Break long webinars into short blocks of content, and include polls, quizzes, or breakout discussions. Let participants bring **their own RDM issues** and discuss them in small groups.

</details>

<details>
  <summary><strong>5. Make evaluation and improvement possible</strong></summary>

With clear goals and structure, it is easier to assess whether the training worked — and to adapt based on feedback or delivery mode.

**Tip:** Instead of collecting only an end‑of‑course survey, include assessment/feedback moments during the session than can help you evaluate specific activities. After each edition, document what to keep, drop, or change.

</details>

<details>
  <summary><strong>6. Use time and resources efficiently</strong></summary>

Thoughtful design prevents overload, avoids unnecessary content, and focuses on what truly matters.

**Tip:** Rather than preparing an extensive slide deck covering all aspects of RDM, you may choose to focus on one key problem to work on (e.g. storage). You can also design reusable activities that can be adapted for future sessions. 

</details>

<br>


## Training design: what does it entail?

Training design is more than preparing slides or selecting activities. It is a
structured process that helps you create learning experiences that are relevant,
effective, and aligned with the needs of your audience. Most training design
approaches share a set of common components and follow a recurring cycle.

<h3> Key components of a training design cycle </h3>

- **Analysis**: Understanding your learners, their context, and their needs.
- **Design**: Translating needs into clear learning outcomes and selecting appropriate methods.
- **Development**: Creating learning materials, activities, and assessments.
- **Implementation**: Delivering the training in practice.
- **Evaluation**: Gathering feedback and assessing the effectiveness of the training.

These steps appear in many instructional design models. One of the most well‑known examples is the **ADDIE framework** (Analysis – Design – Development – Implementation – Evaluation). Other models (e.g., SAM, Backward Design, 5Es) offer similar guidance but with different emphases.

<h3> Why use a model? </h3>

A training design model helps you:

- **Stay focused** on the purpose of the training.
- **Ensure alignment** between learning needs, outcomes, methods, and assessments.
- **Avoid jumping prematurely into content creation**, which often leads to overload or materials that do not support learning.
- **Build a structure that supports evaluation and continuous improvement**.

Models give you a roadmap, but they are not meant to be followed rigidly.

It's important to keep in mind that training design is **iterative**, not linear. Although the model starts with *Analysis* and ends with *Evaluation*, in practice you will often:

- revisit earlier decisions,
- refine learning outcomes after testing activities,
- adjust methods based on learner feedback,
- update materials when changing context or delivery format.

**Evaluation is part of every stage.**  
You are constantly checking whether decisions support the intended learning outcomes.

It is tempting to start with *Development* (e.g., making slides), but investing time in *Analysis* and *Design* saves effort later and results in a stronger learning experience.

**What comes next**

In the next part of the course, we will explore each stage of the training design cycle in more detail and apply the steps to your own training concept.
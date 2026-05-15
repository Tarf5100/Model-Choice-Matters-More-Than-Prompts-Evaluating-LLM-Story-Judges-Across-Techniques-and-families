
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
</head>
<body>

  <h1>Model Choice Matters More Than Prompts: Evaluating LLM Story Judges Across Techniques and Families</h1>

  <p>
    This repository contains the implementation, prompts, analysis pipeline,
    and results for our research on <strong>LLM-based story evaluation</strong>
    using the <strong> <a href="https://github.com/dig-team/hanna-benchmark-asg" target="_blank"> HANNA benchmark </a> </strong>.
  </p>

  <hr>

  <h2>Abstract</h2>

  <p>
    Large language models (LLMs) are increasingly used as automatic evaluators
    of generated text, but their reliability for subjective tasks such as story
    evaluation remains unclear.
  </p>

  <p>
    This project systematically compares five prompting strategies across
    GPT-4.1 Mini and Claude variants on the HANNA benchmark.
  </p>

  <ul>
    <li><strong>Model choice matters more than prompt engineering</strong></li>
    <li><strong>Simple prompts outperform elaborate personas</strong></li>
    <li><strong>LLMs rank stories better than calibrated scoring</strong></li>
    <li><strong>Coherence is the hardest narrative dimension</strong></li>
  </ul>

  <hr>

  <h2>Research Questions</h2>

  <ul>
    <li>How do prompting techniques affect LLM-based story evaluation?</li>
    <li>Which prompting strategy aligns best with human judgment?</li>
    <li>Do different LLM families behave similarly as evaluators?</li>
    <li>Can LLMs reliably replace human annotators?</li>
  </ul>

  <hr>

  <h2>Dataset</h2>

  <p>
    We use the <strong>HANNA (Human-ANnotated NArratives)</strong> benchmark:
  </p>

  <ul>
    <li>1,056 generated stories</li>
    <li>Human ratings across six narrative dimensions:</li>
  </ul>

  <ol>
    <li>Relevance</li>
    <li>Coherence</li>
    <li>Empathy</li>
    <li>Surprise</li>
    <li>Engagement</li>
    <li>Complexity</li>
  </ol>

  <hr>

  <h2>Models Evaluated</h2>

  <h3>GPT Family</h3>
  <ul>
    <li>GPT-4.1 Mini</li>
  </ul>

  <h3>Claude Family</h3>
  <ul>
    <li>Claude Sonnet 4.5</li>
    <li>Claude Haiku 4.5</li>
    <li>Claude 3 Haiku</li>
  </ul>

  <hr>

  <h2>Prompting Techniques</h2>

  <table border="1" cellpadding="8" cellspacing="0">
    <tr>
      <th>Technique</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>Role 1</td>
      <td>Human Annotator persona</td>
    </tr>
    <tr>
      <td>Role 2</td>
      <td>Story Expert persona</td>
    </tr>
    <tr>
      <td>Role 3</td>
      <td>Creative Writing Professor persona</td>
    </tr>
    <tr>
      <td>Instruction-Based</td>
      <td>Step-by-step procedural evaluation</td>
    </tr>
    <tr>
      <td>Zero-Shot</td>
      <td>Minimal prompting baseline</td>
    </tr>
  </table>

  <hr>

  <h2>Evaluation Metrics</h2>

  <h3>Error Metrics</h3>
  <ul>
    <li>Mean Absolute Error (MAE)</li>
    <li>Root Mean Square Error (RMSE)</li>
  </ul>

  <h3>Agreement Metrics</h3>
  <ul>
    <li>Exact-Match Accuracy</li>
    <li>Off-by-One Accuracy</li>
    <li>Cohen’s Kappa</li>
  </ul>

  <h3>Correlation Metrics</h3>
  <ul>
    <li>Spearman Correlation</li>
    <li>Pearson Correlation</li>
  </ul>

  <hr>

  <h2>Key Findings</h2>

  <ol>
    <li>
      <strong>Model Choice &gt; Prompt Design</strong><br>
      GPT-4.1 Mini consistently outperformed Claude.
    </li>
    <li>
      <strong>Simpler Prompts Work Better</strong><br>
      Instruction-Based and Role 1 prompts achieved the strongest performance.
    </li>
    <li>
      <strong>Complex Personas Hurt Performance</strong><br>
      The “Creative Writing Professor” persona significantly degraded results.
    </li>
    <li>
      <strong>LLMs Rank Better Than They Score</strong><br>
      Models preserved rankings better than absolute score calibration.
    </li>
    <li>
      <strong>Coherence Is the Hardest Dimension</strong><br>
      Both GPT and Claude struggled most with coherence evaluation.
    </li>
  </ol>

  <hr>

  <h2>Authors</h2>

  <ul>
    <li>Nouf AlMansour</li>
    <li>Nour AlGhomlas</li>
    <li>Tarfah Bin Moammar</li>
    <li>Shahad AlMutairi</li>
    <li>Lujain AlHarbi</li>
  </ul>

  <p>
    <strong>Supervisor:</strong> Dr.Hend Alrasheed
  </p>

</body>
</html>

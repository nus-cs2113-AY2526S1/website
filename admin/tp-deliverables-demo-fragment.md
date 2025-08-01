{% if cs2103 %}==**To reduce workload, this deliverable <span class="text-danger">has been removed from tP requirements</span> this semester.**==

<panel type="secondary" header="Details ... (no longer applicable)" peek>
{% endif %}

* **Record a demo** of all the product features, in a reasonable order. Some options:
  * Screen record each feature and tie it up (see the  "Suggested tools" below for tool options).
  * Schedule + record a zoom meeting within the team, where you share your screens and do the demo.
* **The quality of the demo will not affect marks** as long as it serves the purpose (i.e., demonstrates the product features). Hence, don't waste too much time on creating the video.
* **Audio explanations** are strongly encouraged{% if not cs2113 %} (but not compulsory) -- alternatively, you can switch between slides and the app to give additional explanations{% endif %}.
* **Annotations and other enhancements** to the video are optional (those will not earn any extra marks).
* **All members taking part** in the demo video is encouraged but not compulsory.
* **File name:** `[TEAM_ID][product Name].mp4`  %%e.g., [{{ example_team_id }}][ContactsPlus].mp4%% (other video formats are acceptable but use a format that works on all major OS'es).
* **File size:** Recommended to keep below 200MB. You can use a low resolution as long as the video is in usable quality.
* **Submission:** Submit to Canvas (via the corresponding assignment).
* **Deadline:** 2 days after the main deadline
* **Suggested tools:**
  * Ink2Go: You can use this to record your screen and annotate if necessary. [Here](https://wiki.nus.edu.sg/display/cit/Ink2go+Instructions+for+Students) are some instructions from NUS CIT to help you get started.
  * [Handbrake](https://handbrake.fr/): A free/open-source tool to help convert videos to MP4.

#### <span class="badge bg-info">Demo</span> <span class="text-info">Duration</span>

* **Strictly 18 minutes for a 5-person team, 15 minutes for a 4-person team**, 21 minutes for a 6-person team. Exceeding this limit will be penalized.
<!--
* **An additional 5 minutes will be given to set up** i.e., you will be given access to the demo station 5 minutes before your allocated start time.~~
-->

#### <span class="badge bg-info">Demo</span> <span class="text-info">Target audience</span>

* **Assume you are giving a demo to a higher-level manager of your company**, to brief them on the current capabilities of the product. This is the first time they are seeing the new product you developed. The actual audience are the evaluators (two tutors).

#### <span class="badge bg-info">Demo</span> <span class="text-info">Scope</span>

* ==**Start by giving an overview of the product**== so that the evaluators get a sense of the full picture early. Include the following:
  * **What** is it? %%e.g., FooBar is a product to ensure the user takes frequent standing-breaks while working.%%
  * **Who** is it for? %%e.g., It is for someone who works at a PC, prefers typing, and wants to avoid prolonged periods of sitting.%%
  * **How** does it help? Give an overview of how the product's features help to solve the target problem for the target user

<div class="indented-level2">

Here is an example:
```{.no-line-numbers}
Hi, welcome to the demo of our product FooBar. It is a product to ensure the user takes
frequent standing-breaks while working.
It is for someone who works at a PC, prefers typing, and wants to avoid prolonged periods
of sitting.
The user first sets the parameters such as frequency and targets, and then enters a
command to record the start of the sitting time, ... The app shows the length of the
sitting periods, and alerts the user if ...
...
```
</div>

* There is no need to introduce team members or explain who did what. %%Reason: to save time.%%
<!--
* It is fine for one member (or only some members) to take part in creating the video, although sharing the load among team members is encourages.
* **Each person should do a fair share of the demo**. However, it's OK for one member to do all the typing.
* **There is no need for each person to demo their own work**.
-->
* **Present the features in a reasonable order**: Organize the demo to present a cohesive picture of the product as a whole, presented in a logical order.
* **No need to cover design/implementation details** as the manager is not interested in those details.

#### <span class="badge bg-info">Demo</span> <span class="text-info">Structure</span>

* **Demo the product using the same executable** you submitted <!--, on your own laptop, using the TV.-->
* **Use a sufficient amount of <tooltip content="`Mr aaa` is not a realistic person name">_realistic_</tooltip> demo data.** %%e.g at least 20 data items%%. Trying to demo a product using just 1-2 sample data creates a bad impression.
<!--
* **It can be a _sitting down_ demo.** You'll be demonstrating the features using the TV while sitting down. But you may stand around the TV if you prefer that way.
* **It will be an uninterrupted demo.** The audience members will not interrupt you during the demo. That means you should finish within the given time.
* **Dress code**: The level of formality is up to you, but it is recommended that the whole team dress at the same level.
-->

#### <span class="badge bg-info">Demo</span> <span class="text-info">Tips</span>

* **Plan the demo to be in sync with the impression you want to create.** For example, if you are trying to convince that the product is easy to use, show the easiest way to perform a task before you show the full command with all the bells and whistles.

<!--
* **Spend as much time as possible on demonstrating the actual product.** Not recommended to use slides (if you do, use them sparingly) or videos or lengthy narrations.
Avoid skits, re-enactments, dramatizations etc. This is not a sales pitch or an informercial. While you need to show how a user use the product to get value, but you don’t need to act like an imaginary user. For example,<br>
[Instead of this] `Jim get’s a call from boss. "Ring ring", "hello", "oh hi Jim, can we postpone the meeting?" "Sure". Jim hang up and curses the boss under his breath. Now he starts typing ..etc.`<br>
[do this] `If Jim needs to postpone the meeting, he can type …`<br>
It’s not that dramatization is bad or we don’t like it. We simply don’t have enough time for it.
Note that CS2101 demo requirements may differ. Different context → Different requirements.
* **Showcase how the feature improves the user’s life** rather than simply describe each feature.
* **Rehearse the steps well** and ensure you can do a smooth demo. ==Find a [_golden path_](https://www.ibtimes.co.uk/sleight-hand-white-lies-bottle-scotch-how-apple-pulled-off-first-iphone-launch-1600085) and stick to it==. Poor quality demos can affect your grade.
* **Don’t waste time repeating things the target audience already knows.** e.g., no need to say things like "We are students from NUS, SoC".
* **No need to introduce next presenter** at the end of your part %%Reason: to save time%%.


#### <span class="badge bg-info">Demo</span> <span class="text-info">Special circumstances</span>

* **If a significant feature was not merged on time:** inform the tutor and get permission to show the unmerged feature using your own version of the code. Obviously, unmerged features earn much less marks than a merged equivalent but something is better than nothing.
* **If you are unable to come to the demo due to a valid reason**, submit the evidence of your excuse %%e.g., MC%% to prof. The demo is part of course grading and ==absence without a valid reason== will cause you to lose marks.
-->

{% if cs2103 %}
</panel>
{% endif %}

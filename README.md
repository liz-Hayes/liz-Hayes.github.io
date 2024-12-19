<h1>Exploring the Age of Olympic Athletes</h1>

This narrative visualization explores the age of Olympic athletes. The
narrative describes how the average athlete age has changed over time and variations from sport to sport. This visualization allows for user interaction to
discover more insights into the dataset.

Follow this link to view the narrative visualization: https://liz-hayes.github.io./
Original Dataset: https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results/data

<h2>Structure</h2>
The narrative visualization is designed to follow a martini glass
structure. Scenes one and two begin the story for the reader by introducing
annotated data to tell a story to the user. These two scenes are the stem of the
martini glass. In scene 3, the data is opened up for user exploration. The user can
filter on athlete sex, season of the games, and medal earned to see how charts from
scenes one and two change.

<h2>Annotations</h2>
 I used d3-annotation to create annotations for scenes 1 and 2. The
annotations consistently used the d3.annotationCalloutCircle as well as the same
color and font to keep a consistent look. I used the default gray color and font for the
annotations to draw a distinction from the rest of the chart. The annotations
support the messaging by pointing out interesting data points and attempting to
provide an explanation to the user. For example, in scene one it is important to
provide an explanation to the user about missing data during World War II. The
annotation explains that the Olympics were cancelled during that period due to the
war. The annotations do not change within a single scene to keep things simple for
the user to see the story line.

<h2>Parameters</h2>
One important parameter used is the ‘scene’ parameter. This
parameter is used to load the corresponding scene. The parameter holds the
current state so that the correct scene is displayed when the user clicks the forward
or back button. Other important parameters are season, medal, and sex. In scene 3
the user interaction changes the content of array associated with each of these
parameters. The data is filtered based on the arrays.

<h2>Triggers</h2>
These buttons trigger functions that change the ‘scene’ parameter and
load a different scene. Additionally, as part of scene three, users can check and
uncheck boxes that change parameters. For both the check boxes and arrow
buttons, the color changes slightly when moused over to indicate to the user that
the button can be clicked.

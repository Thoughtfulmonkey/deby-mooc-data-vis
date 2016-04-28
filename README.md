# deby-mooc-data-vis

## Data Setup
Both the state diagram and activity grid diagram require a csv file that contains a grid of dates.  

- The dates should be when particular sections of the course were completed.
- Each row should be the data for a particular learner / student.
- The first row should be list headings.

In additiona the dates should be in floating point format, not as dates.  The included ExampleData.xlsx shows the difference between the two.  If you are using Excel, then you can just copy the dates and paste them as values.  Alternatively these could just be the day of the course, e.g. first day as 1, second as 2 etc.

ExampleData.csv shows the expected input.

## State Diagram

The use of this type of diagram for MOOC data was proposed by:

> Coffrin, C., Corrin, L., de Barba, P. & Kennedy, G. (2014).  Visualizing patterns of student engagement and performance in MOOC.  In Proceedings of the Fourth International Conference on Learning Analytics and Knowledge (LAK '14). ACM, New York, NY, USA, 83-92.

Once you have the required csv file, the changes required in the html file are minimal:

- Open state-diagram.html (or your own copy) in a text editor (e.g. Notepad)
- Find the section that includes the comment "Things to change"
- Change the filename for the csv file that you are loading
- Update the "units" to include the actual column headings in your csv file

Other values are optional, and their purpose is documented.


## Activity Grid Diagram

With the csv file in the appropriate format, there are a number of changes required in the html file:

- Open activity-grid-diagram.html (or your own copy) in a text editor (e.g. Notepad)
- Find the section that includes the comment "Things to change"
- Change the filename for the csv file that you are loading
- Update the "units" to include the actual column headings in your csv file
- Set 'start' date, in the format yyyy-mm-dd. This only affects labelling of the y axis, not the presentation of data.
- Set min to be the earliest date for data that you want to include. Essentially the minimum value in your dataset - if you want to display all data.  This should match the start date to ensure acurate display.
- Set the max value to be the latest date that you want to include. Essentially the highest value in your dataset.


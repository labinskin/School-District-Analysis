# School-District-Analysis

##### Overview

The school board has notified Maria and her supervisor that the `students_complete.csv` file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.

##### Results

- **How is the district summary affected?**
- Original
![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20District%20Summary.png)
- Updated
![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20District%20Summary.png)
- As indicated by the two DataFrames in comparison, the updated DataFrame indicates that the removal of the scores lowers the overall average math score, the percent passing math, and the percent passing reading, and the overall passing scores slightly, with decreases ranging from .1 percent to .3 percent.
- **How is the school summary affected?**
- Original
![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20School%20Summary.png)
- Updated
![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20School%20Summary%202.png)
- The only change in the school summary, as indicated by comparing the two DataFrames, is the slight decrease in all categories for Thomas High School.
- **How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?**
- Original
![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20Top%20and%20Bottom%20Five%20DataFrames.png)
- Updated
![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20Top%20and%20Bottom%20Five%20DataFrames.png)
- Thomas High School does not drop in the ranking of the High Performing Schools. They remain second. However, rather than having a .349 point lead over Griffin High School. They have only a .031 point lead over Griffin. The lost scores make the race for second much closer than before and makes second through fifth, almost even, with Cabrera High School being a clear .704 ahead in first place.
- **How does replacing the ninth-grade scores affect the following:**
  - **Math and reading scores by grade**
  - Original
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20Math%20Scores%20by%20Grade.png)
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20Reading%20Scores%20by%20Grade.png)
  - Updated
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20Math%20Scores%20by%20Grade.png)
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20Reading%20Scores%20by%20Grade.png)
  - There are no major changes to report here, outside of Thomas High School having a NaN for their 9th grade scores. The scores of their other grades and all other schools remains the same.
  - **Scores by school spending**
  - Original
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20Scores%20by%20Spending.png)
  - Updated
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20Scores%20by%20School%20Spending.png)
  - No changes in the scores for school spending. 
  - **Scores by school size**
  - Original
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20Scores%20by%20Size.png)
  - Updated
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20Scores%20by%20Size.png)
  - No changes in the scores for school size.
  - **Scores by school type**
  - Original
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Original%20Scores%20by%20Type.png)
  - Updated
  ![](https://github.com/labinskin/School-District-Analysis/blob/main/Resources/Updated%20Scores%20by%20Type.png)
  - No changes in the scores for school type.

##### Summary
The major changes were a drop in the scores of the district summary, specifically Thomas High School's scores. For the district, there a .1 point drop in Average Math Score, a .2 percent drop in % Passing Math, a .3 percent drop in % Passing Reading, and a .1 percent drop in % Overall Passing.

At Thomas High School specifically, there was a .068 point drop in Average Math Score, a .087 percent drop in % Passing Math, a .29 percent drop in % Passing Reading, and a .318 percent drop in % Overall Passing.

An outlier in Thomas High School's scores dropping is the Average Reading Score, which went up .048 points.

The other set of major changes, as noted above dealt with Thomas High's rank in the top five overall performing schools. As discussed above, rather than having a .349 point lead over Griffin High School. They have only a .031 point lead over Griffin. The lost scores make the race for second much closer than before and makes second through fifth, almost even, with Cabrera High School being a clear .704 ahead.

There were no changes in the scores by spending, size, or type. One possibility for this is that because the percentages for spending were rounded only 1 decimal place, any changes could have been relatively minor and rounded out, unlike the changes in the High/Low Performing School DataFrame. Additionally, for school by size and part of school type, there are no decimal places, as each percent is rounded to a whole number.

These are the differences in the PyCity School Data. Thomas High School's data decreased overall district scores, as well as Thomas High's own scores. The changes were not seen in some of the sorted DataFrames, but as noted, this could be from the formatting where decimal places were rounded off or rounded to whole numbers, compared to some of the data from the District Level DataFrames.

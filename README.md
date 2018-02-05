# data-incubator-project
Project on virtual learning enironment (VLE) dataset analysis
With the advancement of internet technology, virtual learning environments have emerged and grown rapidly. With large amount of student data, we can analyze the available datasets to find get valuable information on the selection and performance of online courses. Improvements can be made by knowing factors like age, gender, region disability, education level of students, and length, opening time, assignment load, amount of student register/withdraw, and final result of courses. With more information, it is possible to provide better courses and adjust to target students.

Link to dataset:
  https://analyse.kmi.open.ac.uk/open_dataset

Scipts used to generate sample plots:

> finalresult<-table(studentInfo$final_result)

> pie(finalresult)

> dev.copy2pdf(file="final_result_pie.pdf")

> genderage<-table(studentInfo$gender,studentInfo$age_band)

> barplot(genderage,main = "Gender and Age",col=c("darkblue","red"),legend = rownames(genderage), beside=TRUE)

> dev.copy2pdf(file="gender and age barplot.pdf")

# README



## Background

This is a dataset generated from production well tests on oil wells that produce under natural flow and gas lift artificial lift for a year.

There are 13,400 well tests (observations) in total for more than 40 fields, 100+ offshore platforms for 743 physical wells (drilled hole), and 995 strings (in dual wells).

These production well tests are taken periodically to assess the performance of the well. Generally a well under production test is disconnected from the common production manifold and reconnected to its own test separator and test tank. Typical measurements that are taken during a production well test are:

* Gross liquid production (BLPD)
* net oil BOPD)
* produced gas (MSCFD or MMSFCD)
* produced water (BWPD)
* wellhead pressure (psia)
* wellhead temperature (deg Farenheit)
* annulus pressure (psia)
* injected gas rate in gas lift wells, (MSCFD or MMSCFD)
* other calculated variables such as watercut, GOR, duration of the test, other units, etc.

Usually these tests have a duration of 24 hours but this could vary depending on conditions.

If the well test is not satisfactory it is marked as `rejected` and marked to be repeated. 

## Databook
There is an additional markdown file with desciption of the well test variables.
See the file `databook`.


## Well naming
A physical well is called a `HOLE`. A phsyical well is a well that has been drilled and completed. A nominal well is a string in dual completions where gas lift has been deployed. A dual completion has a long string **LS** and a short string **SS**. Each string produces from their own isolated formations, and act as separate wells with the only exception of the annulus which is a common point of injection. Each string, LS or SS, connects to its production manifold in the surface; they do not commingle subsurface.

That is why a physical well or hole sometimes contains two nominal wells. A nominal well is used to perform nodal analysis and other well performance activities.

The well names are composed by the field, platform, well number and completion type. The naming look similar to this:

                FILD-P001-LS
                ATHR-Q999-SS
                
If the well has a unique string, then the well ends in **TS**, as in tubing string.


## What can we learn from these well tests
Usually well tests are run to assess the productivity or performance of the well. The results of the well test acts as a diagnostic of the well and can also be used as troubleshooting method. The well test is a powerful indicator of the behavior of the well telling us how close or how far is from the technical potential or the well performance curves such as the IPR or VLP.

Well tests, together with reservoir and fluid properties are used to calibrate well models.



## What questions can data science address?

1. which field has the highest oil production?

2. when a field hit a 50% watercut?

3. which is the well that has the highest gas injection rate?

4. what is the well that produces more oil with less gas injection rate? (gas lift well)

5. is there a relationship between the GOR and watercut?

6. which well test variables are correlated?

7. which well test variables are the least correlated?

8. how many wells are natural flow, gas lift or another artificial lift method?

9. how many wells have dual completions?

10. which string (in dual completion wells) produces more oil? Short string or long string?

11. which wells were the ones with more tests during the current year?

12. which field had more well tests during the year?

13. which well was retested more in any field?

14. which wells were tested more than 24 hours?

15. what is the average well test duration?

16. what wells were more tested in a year?

17. what wells have to be repeated more than 5 times in a week?

18. what wells showed a considerable increase or decrease in gross production?

19. is there a relatioship between gas injection pressure and net oil production?

20. what fields produce with the highest watercut?

21. what fields have the highest and lowest GOR?

22. what wells were shut in the longest?

23. what wells were taken out of production during the year?

24. what wells decreased oil production the most?

25. what wells increased oil production?

26. what wells had the sharpest wellhead pressure decline?

27. what is the average gas injection pressure?

28. what are the fields and platforms with the highest and lowest gas injection pressure?

## Data cleaning

* Find NAs in numeric variables.

* Which variables have the highest percentage of NAs?

* Find empty observations in character variables. 

* Are there any character variables wit more than 95% of NAs?

* 


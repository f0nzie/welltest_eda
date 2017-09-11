# README



## Background

This is a dataset generated from production well tests on oil wells that produce under natural flow and gas lift conditions during a year.

There are 13,400 well tests in total for more than 40 fields, 100+ platforms for 743 physical wells and 995 strings.

These production well tests are taken periodically to assess the performance of the well. Generally a well under test is disconnected from the common production manifold and is connected to its own test separator and test tank. Measurements that are taken during a well test are:

* Gross liquid production
* net oil
* produced gas
* produced water
* wellhead pressure
* wellhead temperature
* annulus pressure
* injected gas rate (in gas lift wells)
* other calculated variables such as watercut, GOR, etc.

Usually these test have a duration of 24 hours but this could vary depending on conditions.
If the well test is not satisfactory it is marked as `rejected` and repeated.


## Well naming
A physical well is called a `HOLE`. A phsyical well is a well that is drilled. A nominal well is a well is a string in dual completions where gas lift is used. A dual completion has a long string **LS** and a short string **SS**. Each string produces from their own isolated formations and act as separate wells with the only exception of the annulus as a common point of injection. Each string, LS or SS, connect to its production manifold in the surface.

That is why a physical well or hole sometimes contains two nominal wells. A nominal well is used to perform nodal analysis and other well performance analysis.

The wells are composed by the field, platform, well number and completion type. The naming look similar to this:

                FILD-P001-LS
                ATHR-Q999-SS
                
If the well has a unique string, then the well ends in **TS**, as in tubing string.


## What can we learn from these well tests
Usually well tests are run to assess the performance of the well. The results of the well test acts as a diagnostic of the well and can also be used as troubleshooting method. The well test is a powerful indicator of the behavior of the well telling us how close or how far is from the technical potential or the well performance curves such as the IPR or VLP.

Well tests, together with reservoir and fluid properties are used to calibrate well models.



## What question can data science address?

* which field has the highest oil production?

* when a field hit a 50% watercut?

* which is the well that has the highest gas injection rate?

* what is the well that produces more oil with less gas injection rate? (gas lift well)

* is there a relationship between the GOR and watercut?

* which well test variables are correlated?

* which well test variables are the least correlated?

* how many wells are natural flow, gas lift or another artificial lift method?

* how many wells have dual completions?

* which string (in dual completion wells) produces more oil? Short string or long string?

* which wells were the ones with more tests during the current year?

* which field had more well tests during the year?

* which well was retested more in any field?

* which wells were tested more than 24 hours?

* what is the average well test duration?

* what wells were more tested in a year?

* what wells have to be repeated more than 5 times in a week?

* what wells showed a considerable increase or decrease in gross production?

* is there a relatioship between gas injection pressure and net oil production?

* what fields produce with the highest watercut?

* what fields have the highest and lowest GOR?

* what wells were shut in the longest?

* what wells were taken out of production during the year?

* what wells decreased oil production the most?

* what wells increased oil production?

* what wells had the sharpest wellhead pressure decline?

* what is the average gas injection pressure?

* what are the fields and platforms with the highest and lowest gas injection pressure?

# PASS Summit 2018
Repository for the PASS Summit data visualization talk. The final version of the pbix file can be found in the PASS_Summit_2018/PBIX folder. The Jupyter Notebook used in the session can be found in the root of this repository. The data set used in the Jupyter Notebook can be found in the PASS_Summit_2018/Data folder. You can go to this [link](https://docs.microsoft.com/en-us/power-bi/service-r-packages-support) to get a list of all of the R packages along with version that are available in the service. If you will like a tabular version of the list you can refer to the MS Excel workbook that is in the PASS_Summit_2018/RPackages folder. 

**Known limitations of R visuals in the Power BI desktoop ([Source Website](https://docs.microsoft.com/en-us/power-bi/desktop-r-visuals))**:

- Some of the visualization features that works in the Power BI Desktop do not work in the Power BI service. I am in communication with the Microsoft team to see how and when those issue will be resolved. I will update this README when I get more information. 
- The version of R that is used in the service lags behind the current version of R. At the time of this post, the version of R that is being used in the Power BI Service is R 3.4.2 which was released on 2017.09.28. Your R visual development should be done using the same R environment that the service is using. You can get previous versions of R from [CRAN](https://cran.r-project.org/bin/windows/base/old/). You can have multiple versions of R installed on the same machine but you may run into problems in Power BI. To avoid those problems I recommend that you just have the version of R that the Power BI service is using on your machine.
- Data size limitations – data used by the R visual for plotting is limited to 150,000 rows. If more than 150,000 rows are selected, only the top 150,000 rows are used and a message is displayed on the image.
- Calculation time limitation – if an R visual calculation exceeds five minutes the execution times out, resulting in an error.
- Relationships – as with other Power BI Desktop visuals, if data fields from different tables with no defined relationship between them are selected, an error occurs.
- R visuals are refreshed upon data updates, filtering, and highlighting. However, the image itself is not interactive and cannot be the source of cross-filtering.
- R visuals respond to highlighting other visuals, but you cannot click on elements in the R visual in order to cross filter other elements.
- Only plots that are plotted to the R default display device are displayed correctly on the canvas. Avoid explicitly using a different R display device.
- In this release, RRO installations are not automatically identified by the 32-bit version of Power BI Desktop, so you must manually provide the path to the R installation directory in Options and settings > Options > R Scripting.

**Additional Resources**:

- [R for Data Science](http://r4ds.had.co.nz/): I believe this book is the best introduction to the R programming language.

- [Guy in a Cube](https://guyinacube.com/): Great YouTube channel for all things Power BI. Patrick and Adam does a great job of keeping you informed with what's new in Power BI and they also provide great tutorials on how to use the tool.

- [Excel on Fire](https://www.youtube.com/channel/UCZgOVykPoRbSZQfY9YysiRQ):  Oz does a great job creating tutorials on how to use Power Query for data munging.

- [Mico Yuk](http://bibrainz.com/aof/author/micoyuk/): Mico Yuk and her staff at BI Brainz provides great training on how to effectively use data visualization to tell amazing stories about your data.

- In the near future I will be updating my [blog](https://dieselanalytics.com/) which has blogs that covers how to use R within Power BI. There will be future blogs covering how to use R within other areas of the Microsoft ecosystem. Be on the look out!

**Questions**

I attempted to be verbose in my explanations in the Jupyter notebook. If you have questions please reach me at info@dieselanalytics.com and I will answer them as quickly as I am able to.

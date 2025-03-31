---
layout: page
title: "San Francisco Drugs Crime Data Visualization"
description: "Exploring drug-related crimes using Bokeh, Matplotlib, and interactive maps."
---

<!-- Import Recoleta Font -->
<style>
    @import url('https://fonts.googleapis.com/css2?family=Recoleta:wght@400;700&display=swap');

    body {
        font-family: 'Recoleta', sans-serif;
        line-height: 1.7;
        color: #333;
        background-color: #fafafa;
        padding: 40px 20px;
        max-width: 800px;
        margin: auto;
    }

    h1, h2, h3 {
        font-weight: 700;
        color: #222;
        margin-bottom: 15px;
    }

    p {
        font-size: 17px;
        margin-bottom: 20px;
    }

    .code-block {
        background-color: #282c34;
        color: #fff;
        padding: 15px;
        border-radius: 6px;
        font-family: 'Courier New', monospace;
    }

      iframe {
    margin-top: 20px;
    border-radius: 10px;
    border: 1px solid #ddd;
    box-shadow: 3px 3px 12px rgba(0, 0, 0, 0.1);
    width: 100%;
    min-width: 700px; /* Ensures a minimum width of 700px */
    height: 700px; /* Adjust height as needed */
}
    

    .highlight {
        background: #f4f4f4;
        padding: 15px;
        border-left: 5px solid #4682B4;
        border-radius: 5px;
        overflow-x: auto;
    }

</style>

---
<figure>
  <img src="{{ site.baseurl }}/assets/drugs.png" alt="Drug Crimes Over the Years">
  <figcaption>Drug Crimes Over the Years in San Francisco</figcaption>
</figure>

---
## **Drug Crimes Over the Years**
 **Statistics on drug-related crimes in San Francisco have changed significantly over the past 20 years. After reaching a record high in 2009, the number of drug-related crimes steadily declined until 2017. But what caused this shift? Was it truly due to a decrease in drug use? Is this an issue affecting all of San Francisco, or is it concentrated in just a few areas? We will explore these questions using official government crime data collected over two decades.**



 During the late 2000s, San Francisco police increased drug enforcement efforts where drug activity was highly concentrated[1]. In the chart below, we can see the effect of those actions. That and the Great Recession led to increased unemployment and homelessness, both of which were linked to higher drug use and drug-related crimes. 

<figure>
    <img src="{{ site.baseurl }}/assets/OverYears.png" alt="Drug Crimes Over the Years">
    <figcaption>Drug Crimes in San Francisco Over the Years</figcaption>
</figure>


 Since 2010, the number of reported drug crimes has continuously declined. At first glance, this may seem like a positive trend. However, if that were the case, why in 2023, San Francisco recorded 806 drug overdose deaths[2], the highest number on record?

A major factor in the declining crime statistics is policy changes. In 2010, the California Legislature passed AB 2372 [3], which reclassified certain nonviolent offenses, including drug-related crimes, from felonies to misdemeanours. As a result, many offenses were no longer counted in felony crime statistics. This trend continued in 2014 with Proposition 47 [4], which further reduced penalties for drug offenses.   



---
## **Mapping Crime Incidents**
The interactive map below represents crime data collected across San Francisco. It highlights significant differences between districts. The Tenderloin has by far the highest number of drug-related crimes. Other districts follow, but with much lower numbers. The most affected areas are located in the city’s central region. 

<figure>
    <iframe src="{{ site.baseurl }}/assets/crime_map.html" width="100%" height="700px"></iframe>
    <figcaption>Interactive Crime Map of San Francisco</figcaption>
</figure>


---


  The Tenderloin has been known for years for its high crime rates, homelessness, and drug-related violence. Violent acts occur here more often than in other areas, often linked to the drug trade. In 2007, the neighbourhood saw escalating drug violence, including brazen daylight shootings, as gangs from San Francisco and the broader Bay Area fought for control of drug turf. Example of how bad the situation can be is seen on Haight Street, where people suffering from addiction struggle in plain sight. On January 31, 2014, parking was banned on both sides of the street to reduce violence and drug activity. Without parked cars to hide illegal activity, there were fewer loiterers, and a decrease in drug activity[5]. 

<figure>
  <img src="{{ site.baseurl }}/assets/HydeStreet.png" alt="Drug Crimes Over the Years">
  <figcaption>Hyde street, Tenderloin district in San Francisco</figcaption>
</figure>


---

##  **Drug crimes over years**

<figure>
  <iframe src="{{ site.baseurl }}/assets/bokeh_districts.html"></iframe>
  <figcaption>Interactive chart- Crimes over years by District</figcaption>
</figure>

 In the interactive chart above, we can see the trend in drug-related crimes. During the 2008, San Francisco police increased drug enforcement efforts, particularly in areas like the Tenderloin, Mission District, and South of Market, where drug activity was heavily concentrated. This initially led to higher reported crime numbers. After a significant decline, crime levels in the Mission District and South of Market remained relatively low. However, in 2018, offenses in the Tenderloin surged once again, reaching a significantly high level. This may be related to the rise in the popularity of fentanyl[6], as organized crime groups saw an opportunity to introduce it into an already active drug market where users were seeking stronger substances. We can also compare that only Tenderloin district numbers was almost that bad as in 2010r. 

##  **Conclusion**
 This analysis highlights the importance of identifying the true causes behind data changes. An apparent trend may not always reflect real progress but rather a legal or policy shift. It also illustrates how a single high-crime district can skew overall numbers, even when other areas show a decline in drug crimes.

---

Sources:  
[1] United States Department of Justice (2009) San Francisco Police Department and U.S. Attorney working together to curb violence. Available at: 
https://www.justice.gov/usao-ndca/san-francisco-police-department-and-us-attorney-working-together-curb-violence-national (Accessed: 31 March 2025)
[2] San Francisco Department of Public Health (2023) Drug overdose and treatment data and reports. Available at: https://www.sf.gov/resource--2023--drug-overdose-and-treatment-data-and-reports (Accessed: 31 March 2025).
[3] California Legislative Information (2010) AB-2372: Grand theft: threshold amount. Available at: https://www.leginfo.ca.gov/pub/09-10/bill/asm/ab_2351-2400/ab_2372_bill_20100902_enrolled.html (Accessed: 31 March 2025).
[4] California Courts (2014) Proposition 47 FAQs. Available at: https://www.courts.ca.gov/publication/proposition-47-faqs (Accessed: 31 March 2025). 
[5] Nevius, C.W. (2014) 'Turk Street parking ban aims to curb crime', San Francisco Chronicle, 6 February. Available at: https://en.wikipedia.org/wiki/Tenderloin%2C_San_Francisco (Accessed: 31 March 2025).
[6] Kron4 (2023) The rise of fentanyl in San Francisco. Available at: https://www.kron4.com/news/focus-on-fentanyl/the-rise-of-fentanyl-in-san-francisco/?utm_source=chatgpt.com (Accessed: 31 March 2025)


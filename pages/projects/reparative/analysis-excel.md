---
title: Analyzing the Metadata from a Reparative Lens Using Excel
layout: page
permalink: /reparative_analysis_excel.html
---

## Excel

### Introduction

Exploratory data analysis using widely available tools such as Excel to generate basic overviews of the metadata can provide a surprising amount of insight into an archive's digital holdings. While I did consider using other tools such as OpenRefine or Pandas to perform these tasks, I like to try and use tools that have low technical barriers to use and are familiar to a larger number of archivists when doing work that I want to make shareable.

Material digitized by an archive can be understood as an  artificial collection curated and stewarded by the archive. While individuals who work in the area of digital preservation have long understood that digital collections and the preservation files, access files, and metadata that compose them are separate collections that archives are responsible for stewarding, I think that this perspective can be extended to view and analyze these collections as an expression of an archive's priorities for digitization and public access. Digitization and metadata creation requires an investment of scarce resources and the materials an archive digitizes are not selected, digitized, described, and publicized in a vacuum. There is thought behind these decisions, and when there is no careful thought, the biases of the institution show through clearly. 

Note: I took an institution-centric approach in the language I used above. I would like to make clear that it is not "the archive" or "an archive" that digitizes materials--it is people. The materials selected for digitization are selected by one or a few select individuals who can choose to reinforce or oppose the historical systematic exclusion of individuals and communities of marginalized and often intersecting identities within digitized collections. Metadata schemas are created, relevant vocabularies chosen, and internal standards created by other individuals who can choose to use language that is offensive, discriminatory, or alienating to users who are members of communities historically marginalized by archives. The materials are then described by people who can further reinforce or oppose these issues. These layers of people and decisions made by people have the opportunity to continue compounding the inequity, white supremacy, and classism that have been inherent to much archival work. 

What follows is an overview of the composition of the digital collections before diving deeper into the specific user-supplied metadata that is more subject to bias.

### Collections

There are 90 collections represented by the 8,202 digitized items. The top five collections, in terms of frequency/percentage of total digitized items, represent 41.93% of all digitized items. This means that if a digitized collection is highly represented and contains items representing similar topics, even just a single collection has the ability to significantly sway the overall profile of digital collections at a particular institution. 

<table>
<thead>
  <tr>
    <th>collection</th>
    <th>frequency</th>
    <th>percentage</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>0099: Cabell-Wayne Historical Society Collection</td>
    <td>1060</td>
    <td>12.92</td>
  </tr>
  <tr>
    <td>0236: Fred B. Lambert Papers, 1809-1964</td>
    <td>1021</td>
    <td>12.44</td>
  </tr>
  <tr>
    <td>0842: Dr. and Mrs. Daniel Sharkey Greeting Card Collection</td>
    <td>557</td>
    <td>6.79</td>
  </tr>
  <tr>
    <td>0227: Marshall University Regional Photograph Collection</td>
    <td>468</td>
    <td>5.70</td>
  </tr>
  <tr>
    <td>0010: Catherine Bliss Enslow Papers</td>
    <td>335</td>
    <td>4.08</td>
  </tr>
  <tr>
    <td>0596: C. Clifford Caverlee Collection</td>
    <td>334</td>
    <td>4.07</td>
  </tr>
  <tr>
    <td>0703: Rosanna Blake Collection</td>
    <td>329</td>
    <td>4.01</td>
  </tr>
  <tr>
    <td>0853: Carl Barnett Photograph Collection</td>
    <td>265</td>
    <td>3.23</td>
  </tr>
  <tr>
    <td>0391: Eli Camden Henderson Papers</td>
    <td>246</td>
    <td>2.99</td>
  </tr>
  <tr>
    <td>0525: Doris C. Miller Papers</td>
    <td>211</td>
    <td>2.57</td>
  </tr>
  <tr>
    <td>0255: Catherine Bliss Enslow Papers</td>
    <td>195</td>
    <td>2.37</td>
  </tr>
  <tr>
    <td>0847: John Hawes Miller, Jr. West Virginia Postcard Collection</td>
    <td>178</td>
    <td>2.17</td>
  </tr>
  <tr>
    <td>0189: Dr. Charles A. "Carl" Hoffman Collection</td>
    <td>150</td>
    <td>1.82</td>
  </tr>
  <tr>
    <td>0787: Myers Family Collection</td>
    <td>144</td>
    <td>1.75</td>
  </tr>
  <tr>
    <td>0761: Marvin L. Stone Collection</td>
    <td>136</td>
    <td>1.65</td>
  </tr>
  <tr>
    <td>0792: Huntington Parks and Recreation Photo Collection</td>
    <td>130</td>
    <td>1.58</td>
  </tr>
  <tr>
    <td>0834: Matthew A. Reese Papers</td>
    <td>129</td>
    <td>1.57</td>
  </tr>
  <tr>
    <td>0484: William Wallace Photograph Collection</td>
    <td>127</td>
    <td>1.54</td>
  </tr>
  <tr>
    <td>0276: Harlow Warren Papers</td>
    <td>119</td>
    <td>1.45</td>
  </tr>
  <tr>
    <td>0770: Carrie Eldridge Collection</td>
    <td>110</td>
    <td>1.34</td>
  </tr>
  <tr>
    <td>0658: Louis A. Mobayed Collection</td>
    <td>105</td>
    <td>1.28</td>
  </tr>
  <tr>
    <td>0823: Robert and Sidney Day Collection</td>
    <td>102</td>
    <td>1.24</td>
  </tr>
  <tr>
    <td>0799: Jean Edward Smith Papers</td>
    <td>97</td>
    <td>1.18</td>
  </tr>
  <tr>
    <td>0403: Grady Risen Collection</td>
    <td>96</td>
    <td>1.17</td>
  </tr>
  <tr>
    <td>0816: First Presbyterian Church of Huntington</td>
    <td>90</td>
    <td>1.09</td>
  </tr>
  <tr>
    <td>0188: Ralph W. Brafford Collection</td>
    <td>75</td>
    <td>0.91</td>
  </tr>
  <tr>
    <td>0543: Cabell Co., W. Va. Public Library Collection</td>
    <td>67</td>
    <td>0.81</td>
  </tr>
  <tr>
    <td>0493: Revella Hughes Papers</td>
    <td>61</td>
    <td>0.74</td>
  </tr>
  <tr>
    <td>0118: Jane Adams Dingess Papers</td>
    <td>57</td>
    <td>0.69</td>
  </tr>
  <tr>
    <td>0797: Woman's Club of Huntington Collection</td>
    <td>57</td>
    <td>0.69</td>
  </tr>
  <tr>
    <td>0418: Whittaker-Glanville Family Papers</td>
    <td>56</td>
    <td>0.68</td>
  </tr>
  <tr>
    <td>0625: Mark Freeman Papers</td>
    <td>56</td>
    <td>0.68</td>
  </tr>
  <tr>
    <td>0819: Memphis Tennessee Garrison Papers</td>
    <td>56</td>
    <td>0.68</td>
  </tr>
  <tr>
    <td>0778: Jim Taylor Photograph Collection</td>
    <td>50</td>
    <td>0.60</td>
  </tr>
  <tr>
    <td>0380: Mary Burnside Reynolds Papers</td>
    <td>49</td>
    <td>0.59</td>
  </tr>
  <tr>
    <td>0633: Helen Alexander Papers</td>
    <td>49</td>
    <td>0.59</td>
  </tr>
  <tr>
    <td>0852: James E. Casto Papers</td>
    <td>47</td>
    <td>0.57</td>
  </tr>
  <tr>
    <td>0812: Anderson-Newcomb Company and Family Collection</td>
    <td>45</td>
    <td>0.54</td>
  </tr>
  <tr>
    <td>0846: Earl F. Dickinson Papers</td>
    <td>45</td>
    <td>0.54</td>
  </tr>
  <tr>
    <td>0405: Curtis F. Baxter Papers</td>
    <td>42</td>
    <td>0.51</td>
  </tr>
  <tr>
    <td>0644: Mae Newman Scrapbooks</td>
    <td>37</td>
    <td>0.45</td>
  </tr>
  <tr>
    <td>0790: Gil Kleinknecht Papers</td>
    <td>37</td>
    <td>0.45</td>
  </tr>
  <tr>
    <td>0194: Howard Burton Lee Papers</td>
    <td>35</td>
    <td>0.42</td>
  </tr>
  <tr>
    <td>0332: Jane Boedeker Shepherd Papers</td>
    <td>33</td>
    <td>0.40</td>
  </tr>
  <tr>
    <td>0547: Morrow Family Papers</td>
    <td>31</td>
    <td>0.37</td>
  </tr>
  <tr>
    <td>0711: Seamonds-Willey Family Papers</td>
    <td>31</td>
    <td>0.37</td>
  </tr>
  <tr>
    <td>0388: Oscar R. Shannon Photograph Collection</td>
    <td>30</td>
    <td>0.36</td>
  </tr>
  <tr>
    <td>0771: Stump Photograph Collection</td>
    <td>27</td>
    <td>0.32</td>
  </tr>
  <tr>
    <td>0636: James R. Shephard Papers</td>
    <td>26</td>
    <td>0.31</td>
  </tr>
  <tr>
    <td>0415: Sloan-Wyatt Family Papers</td>
    <td>25</td>
    <td>0.30</td>
  </tr>
  <tr>
    <td>0775: Thornburg Family Photographs</td>
    <td>23</td>
    <td>0.28</td>
  </tr>
  <tr>
    <td>0283: Dr. Henry Drury Hatfield Papers</td>
    <td>20</td>
    <td>0.24</td>
  </tr>
  <tr>
    <td>0818: Floyd Hoard Stark &amp; Pitt Hoard Stark Collection</td>
    <td>19</td>
    <td>0.23</td>
  </tr>
  <tr>
    <td>0008: George H. A. Kunst Papers</td>
    <td>17</td>
    <td>0.20</td>
  </tr>
  <tr>
    <td>0737: George Gunnoe Papers</td>
    <td>17</td>
    <td>0.20</td>
  </tr>
  <tr>
    <td>0463: William D. Birke Papers</td>
    <td>16</td>
    <td>0.19</td>
  </tr>
  <tr>
    <td>0437: Willis H. Franklin Papers</td>
    <td>15</td>
    <td>0.18</td>
  </tr>
  <tr>
    <td>0798: Frank E. Matthews, Jr. Collection</td>
    <td>15</td>
    <td>0.18</td>
  </tr>
  <tr>
    <td>0333: Ann Cutler Collection</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>0379: Alma Nease Noble Papers</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>0559: Benson J. Lubin Papers</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>0577: Rotary Club of Huntington,WV Chapter Records</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>0011: Mary Constance Enslow Collection</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>0302: Arvil Ernest Harris Papers</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>0474: Gill Family Papers</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>0536: Hines Family Papers</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>0104: Alfred T. Proctor Photograph Collection</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>0835: The Links, Incorporated Collection</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>0009: David Michael Gideon Papers</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>0616: Chesapeake &amp; Ohio Hospital Association Records</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>0839: Mildred Mitchell-Bateman Papers</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>0066: Harry Edmund Danford Papers</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>0343: Peaco Family Scrapbook</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>0813: Martha Joe Morehouse Collection</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>0760: Camp Creek Church of Christ Register and Record</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>0475: Nancy Murray Mann Papers</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>0006: Virgil Anson Lewis Papers</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0096: Nimrod Mason Papers</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0286: Leslie W. Self Papers</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0396: Carroll Family Papers</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0655: Ensign Family Papers</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0712: Creed Neff Papers</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0850: Oley Cornerstone Time Capsule</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>0245: Claude Morgan Papers</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>0587: Grimm Family Papers, 1900-1985</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>0047: Miller-Thackston Family Papers</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>0002: Laidley Family Papers</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>0257: Martha Elizabeth Carpenter Miller Collection</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>0348: Long Family Papers</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>0707: Thomas Morgan Photographic Negatives</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
</tbody>
</table>

### Formats 

Based on the formats represented, visual materials such as photographs, postcards (which were rarely transcribed if digitized, making them exclusively visual), and drawings are overwhelmingly represented. Visual materials are often scantly described by the original creators or owners and make it easier for bias to creep into description. 

<table>
<thead>
  <tr>
    <th>format</th>
    <th>frequency</th>
    <th>percentage</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Photograph</td>
    <td>5810</td>
    <td>70.83</td>
  </tr>
  <tr>
    <td>Postcard</td>
    <td>863</td>
    <td>10.52</td>
  </tr>
  <tr>
    <td>Drawing (Visual Work)</td>
    <td>591</td>
    <td>7.20</td>
  </tr>
  <tr>
    <td>Book</td>
    <td>477</td>
    <td>5.81</td>
  </tr>
  <tr>
    <td>No format</td>
    <td>128</td>
    <td>1.56</td>
  </tr>
  <tr>
    <td>Print (Visual Work)</td>
    <td>120</td>
    <td>1.46</td>
  </tr>
  <tr>
    <td>Graphic Art</td>
    <td>90</td>
    <td>1.09</td>
  </tr>
  <tr>
    <td>Government Record</td>
    <td>29</td>
    <td>0.35</td>
  </tr>
  <tr>
    <td>Architectural Document</td>
    <td>18</td>
    <td>0.21</td>
  </tr>
  <tr>
    <td>Correspondence</td>
    <td>17</td>
    <td>0.20</td>
  </tr>
  <tr>
    <td>Pamphlet</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>Poster</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Business Record</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Newspaper</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Advertisement</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>Painting (Visual Work)</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Cartographic Material</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Broadside (Notice)</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
</tbody>
</table>

### Places

Unsurprisingly given the institution's scope of materials that it acquires, the majority of items with documented place names is centered in West Virginia. This fact is not inherently problematic because archival collections get much of their strength through depth rather than breadth, making it all the more apparent when particular histories about a location are not documented. 

<table>
<thead>
  <tr>
    <th>place</th>
    <th>frequency</th>
    <th>percentage</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>No  location</td>
    <td>5000</td>
    <td>60.96</td>
  </tr>
  <tr>
    <td>Huntington, WV</td>
    <td>1668</td>
    <td>20.33</td>
  </tr>
  <tr>
    <td>New York, NY</td>
    <td>127</td>
    <td>1.54</td>
  </tr>
  <tr>
    <td>Davenport, IA</td>
    <td>90</td>
    <td>1.09</td>
  </tr>
  <tr>
    <td>Washington, D.C.</td>
    <td>67</td>
    <td>0.81</td>
  </tr>
  <tr>
    <td>White Sulphur Springs, WV</td>
    <td>37</td>
    <td>0.45</td>
  </tr>
  <tr>
    <td>Philadelphia, PA</td>
    <td>37</td>
    <td>0.45</td>
  </tr>
  <tr>
    <td>Chicago, IL</td>
    <td>37</td>
    <td>0.45</td>
  </tr>
  <tr>
    <td>Charleston, WV</td>
    <td>37</td>
    <td>0.45</td>
  </tr>
  <tr>
    <td>London, England</td>
    <td>33</td>
    <td>0.40</td>
  </tr>
  <tr>
    <td>Beckley, WV</td>
    <td>33</td>
    <td>0.40</td>
  </tr>
  <tr>
    <td>Wheeling, WV</td>
    <td>32</td>
    <td>0.39</td>
  </tr>
  <tr>
    <td>Guyandotte, WV</td>
    <td>27</td>
    <td>0.32</td>
  </tr>
  <tr>
    <td>Parkersburg, WV</td>
    <td>25</td>
    <td>0.30</td>
  </tr>
  <tr>
    <td>Cuba</td>
    <td>25</td>
    <td>0.30</td>
  </tr>
  <tr>
    <td>Grafton, WV</td>
    <td>23</td>
    <td>0.28</td>
  </tr>
  <tr>
    <td>Wayne, WV</td>
    <td>22</td>
    <td>0.26</td>
  </tr>
  <tr>
    <td>Himlerville, KY</td>
    <td>17</td>
    <td>0.20</td>
  </tr>
  <tr>
    <td>Morgantown, WV</td>
    <td>16</td>
    <td>0.19</td>
  </tr>
  <tr>
    <td>Elkins, WV</td>
    <td>16</td>
    <td>0.19</td>
  </tr>
  <tr>
    <td>Clarksburg, WV</td>
    <td>16</td>
    <td>0.19</td>
  </tr>
  <tr>
    <td>Gilbert Creek, WV</td>
    <td>15</td>
    <td>0.18</td>
  </tr>
  <tr>
    <td>Richmond, VA</td>
    <td>14</td>
    <td>0.17</td>
  </tr>
  <tr>
    <td>Martinsburg, WV</td>
    <td>14</td>
    <td>0.17</td>
  </tr>
  <tr>
    <td>Harpers Ferry, WV</td>
    <td>14</td>
    <td>0.17</td>
  </tr>
  <tr>
    <td>Ashland, KY</td>
    <td>13</td>
    <td>0.15</td>
  </tr>
  <tr>
    <td>West Virginia</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>Kenova, WV</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>Hinton, WV</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>St. Charles, MO</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Meadville, PA</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Fairmont, WV</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Cincinnati, OH</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Baltimore, MD</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Riverside, CA</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>Charles Town, WV</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>Bluefield, WV</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>Williamson, WV</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Milton, WV</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Logan, WV</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Gallipolis, OH</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Buckhannon, WV</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Weston, WV</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>Welch, WV</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>St. Louis, MO</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>Point Pleasant, WV</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>Kansas City, MO</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>Big Sandy Valley, KY</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>Barboursville, WV</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>Tel Aviv, Israel</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>Philippi, WV</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>Lewisburg, WV</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>Southampton, England</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Salt Rock, WV</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Rowlesburg, WV</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Paris, France</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Memphis, TN</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Mannington, WV</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Eleanor, WV</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Alderson, WV</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Webster Springs, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>St. Marys, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>San Francisco, CA</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Romney, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Pt. Pleasant, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Princeton, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Pittsburgh, PA</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>New Martinsville, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Moundsville, WV</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Irvine, KY</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Helsinki, Finland</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Atlantic City, NJ</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Tokyo, Japan</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>St. Petersburg, FL</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Spencer, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Shepherdstown, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Sarah Ann, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Salem, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Richwood, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Ravenswood, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Prichard, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Piedmont, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Norris, TN</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Marlinton, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Lexington, VA</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Lexington, KY</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Keyser, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Kanawha Falls, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Gauley Bridge, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Ceredo, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Brooklyn, NY</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Berkeley Springs, WV</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Arlington, VA</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Pence Springs, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Pearl River, NY</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Paintsville, KY</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Oxford, England</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Mullens, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Montreal, Canada</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Montgomery, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Maysville, KY</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Marietta, OH</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Greenbottom, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Gary, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Fulton, MO</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Eton, England</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Chester, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Burma</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Athens, WV</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Williamsburg, VA</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Wellsburg, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Weirton, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Virginia Beach, VA</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Taipei, Taiwan</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Stuttgart, Germany</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Stockholm, Sweden</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Shoals, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Seoul, Korea</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Ronceverte, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Renick, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Rainelle, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Pike County, KY</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Peytona, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Ona, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Omar, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Niagara Falls, NY</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Newell, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Miami Beach, FL</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Marion, OH</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Louisa, KY</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Japan</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Ironton, OH</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Indianapolis, IN</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Hundred, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Howells Mill, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Hampton Roads, VA</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Greensboro, NC</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Gauley Mountain, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Gauley Junction, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Ft. Gay, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Ft Lauderdale, FL</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Danville, NY</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Culloden, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Cox's Landing, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Clifftop, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Charleston, SC</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Catlettsburg, KY</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Bramwell, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Boston, MA</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Boomer, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Bethany, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Berlin, Germany</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Aurora, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Atlanta, GA</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Athens, OH</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Ansted, WV</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Allegheny, PA</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Zanesville, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Winterburn, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Winona, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Winfield, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Winchester, VA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Winchester, KY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Williamstown, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Wilberforce, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>West Union, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>West Sand Lake, NY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Waynesboro, PA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Waterloo, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Wardensville, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Wappocomo, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Walton, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Walnut Ridge, AK</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Waco, TX</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Vincen, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Vienna, VA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Verdun, France</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Venice, Italy</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>University City, CA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Union, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Tunnelton, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Trenton, NJ</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Torchlight, KY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Thurmond, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Thomas, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Terra Alta, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Temple, TX</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Tango, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Tampa, FL</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Sweet Springs, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Spray, NC</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Spain</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>South Charleston, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Silver Spring, MD</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Shinnston, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Shenandoah Junction, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Shelby, KY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Scarbro, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>San Jacinto, CA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Samp, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Salt Lake City, UT</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Rome, Italy</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Roach, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Riviera Beach, FL</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Ripley, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Rangoon, Burma</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Portsmouth, VA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Portland, ME</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Poppa, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Pertersburg, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Penzance, England</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Pennsboro, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Paw Paw, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Parsons, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Palm Beach, FL</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Orange Walk, British Honduras</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Nuttall, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>North Africa</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Norfolk, VA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Newcastle, England</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Newburg, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>New Cumberland, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>New Creek, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Nestorville, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Nashville, TN</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Naples, Italy</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Nanjing, China</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Muskogee, OK</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mount Hope, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mora, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Moorefield, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mobile, AL</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mill Creek, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mexico</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Meriden, CT</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>McMechen, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>McComas, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Matoaka, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Matewan, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mackinac Island, MI</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Los Angeles, CA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Longacre, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>London, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Little Falls, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Little Brier Creek, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Lincolnton, NC</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Lesage, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Leningrad, Russia</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Lebanon, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Landgraff, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Ladoga, IN</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Kingwood, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jamestown, VA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jacksonville, NC</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jacksonburg, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Institute, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hot Springs, AR</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Horton, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hopemont, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hong Kong, China</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hillsboro, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Henderhoot, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hazard, KY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hawk's Nest, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hawaii</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hartford, CT</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hartford City, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Harrisville, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Harman, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hamlin, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hamburg, Germany</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Groton, CT</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Greensboro, PA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Great Cacapon, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Glenville, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Glen Alum, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Gassaway, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>French Lick, IN</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Frederick, VA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Franklin, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fonda, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Flagstaff, AZ</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Ferguson, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fayette Bridge, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Elmira, NY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Elm Grove, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Ellis, KS</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Edgewater, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>East Bank, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Durham, NC</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Dunlevie, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Duluth, MN</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Downs Station, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cumberland, MD</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cowen, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Covington, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Columbus, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Clothier, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cleveland, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Clendenin, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Chimney Corner, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Chesapeake, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Charlotte, NC</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Chanute, KS</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Centerville, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cass, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cashmere, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Camp Douglas, IL</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Camp Chase, OH</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cameron, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Butcher Hollow, KY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Brownsville, PA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Brookside, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Brighton, England</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Binghamton, NY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bethan, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Belington, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bedington, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bartow, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Barger Springs, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Avis, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Auxier, KY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Auburn, NY</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Anawalt, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Amos, WV</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
</tbody>
</table>

### Dates

While I initially had the dates broken down by individual years, I realized that this approach did not add to my understanding of the digitized materials but instead obscured them by being overly specific. To generalize the results, I broke them down into decade ranges. For instance, a date range of "1900s" represents the time period from 1900 to 1909. The range of dates of digitized material demonstrate that the collection features no materials that may have documented indigenous histories in the area.

<table>
<thead>
  <tr>
    <th>date range</th>
    <th>frequency</th>
    <th>percentage</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>No date</td>
    <td>1999</td>
    <td>24.37</td>
  </tr>
  <tr>
    <td>1900s</td>
    <td>1011</td>
    <td>12.32</td>
  </tr>
  <tr>
    <td>1930s</td>
    <td>899</td>
    <td>10.96</td>
  </tr>
  <tr>
    <td>1910s</td>
    <td>789</td>
    <td>9.61</td>
  </tr>
  <tr>
    <td>1950s</td>
    <td>696</td>
    <td>8.48</td>
  </tr>
  <tr>
    <td>1970s</td>
    <td>569</td>
    <td>6.93</td>
  </tr>
  <tr>
    <td>1940s</td>
    <td>458</td>
    <td>5.58</td>
  </tr>
  <tr>
    <td>1920s</td>
    <td>365</td>
    <td>4.45</td>
  </tr>
  <tr>
    <td>1960s</td>
    <td>330</td>
    <td>4.02</td>
  </tr>
  <tr>
    <td>1860s</td>
    <td>286</td>
    <td>3.48</td>
  </tr>
  <tr>
    <td>1890s</td>
    <td>233</td>
    <td>2.84</td>
  </tr>
  <tr>
    <td>1880s</td>
    <td>203</td>
    <td>2.47</td>
  </tr>
  <tr>
    <td>1980s</td>
    <td>184</td>
    <td>2.24</td>
  </tr>
  <tr>
    <td>1870s</td>
    <td>114</td>
    <td>1.38</td>
  </tr>
  <tr>
    <td>1990s</td>
    <td>38</td>
    <td>0.46</td>
  </tr>
  <tr>
    <td>2000s</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>1850s</td>
    <td>8</td>
    <td>0.09</td>
  </tr>
  <tr>
    <td>2010s</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>1840s</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>1820s</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>1830s</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
</tbody>
</table>

### Creators

Nearly 85% of all items do not have a creator listed. Without knowing the creator, it is thus hard to characterize who in the collection might be erased through description or lack of description. 

<table>
<thead>
  <tr>
    <th>authors</th>
    <th>frequency</th>
    <th>percentage</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>No author</td>
    <td>6935</td>
    <td>84.55</td>
  </tr>
  <tr>
    <td>Fred Bussey Lambert</td>
    <td>475</td>
    <td>5.79</td>
  </tr>
  <tr>
    <td>Army Corps of Engineers</td>
    <td>105</td>
    <td>1.28</td>
  </tr>
  <tr>
    <td>Barta Studios</td>
    <td>81</td>
    <td>0.98</td>
  </tr>
  <tr>
    <td>Merrill Hastings</td>
    <td>76</td>
    <td>0.92</td>
  </tr>
  <tr>
    <td>Earl F. Dickinson</td>
    <td>30</td>
    <td>0.36</td>
  </tr>
  <tr>
    <td>Adalbert Johann Volck</td>
    <td>29</td>
    <td>0.35</td>
  </tr>
  <tr>
    <td>Charles B. Hall</td>
    <td>25</td>
    <td>0.30</td>
  </tr>
  <tr>
    <td>US Army Engineers Intelligence Division</td>
    <td>18</td>
    <td>0.21</td>
  </tr>
  <tr>
    <td>United States Army</td>
    <td>15</td>
    <td>0.18</td>
  </tr>
  <tr>
    <td>Eplion</td>
    <td>14</td>
    <td>0.17</td>
  </tr>
  <tr>
    <td>Joe Jablonski</td>
    <td>13</td>
    <td>0.15</td>
  </tr>
  <tr>
    <td>Jack Burnett</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>Thomas Studio</td>
    <td>12</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>Kaplan</td>
    <td>11</td>
    <td>0.13</td>
  </tr>
  <tr>
    <td>Robert R. Rosenfield</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>W. J. B. Gwinn</td>
    <td>10</td>
    <td>0.12</td>
  </tr>
  <tr>
    <td>J. Foster</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Proctor Studios</td>
    <td>9</td>
    <td>0.10</td>
  </tr>
  <tr>
    <td>Bernard</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>Thomas Luther</td>
    <td>7</td>
    <td>0.08</td>
  </tr>
  <tr>
    <td>W. Archibald Wallace</td>
    <td>6</td>
    <td>0.07</td>
  </tr>
  <tr>
    <td>Foster</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>H. Eplion</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Harlow Warren</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Joseph Barta</td>
    <td>5</td>
    <td>0.06</td>
  </tr>
  <tr>
    <td>Cummins</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Fred Burns</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>H. Cazad</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Hupco Studios</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>J. Burnett</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>James Kriegsmann</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>M. Kaplan</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Shlomo Lavie</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>T. H. Higgins</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>Virgil Hatton</td>
    <td>4</td>
    <td>0.04</td>
  </tr>
  <tr>
    <td>A. B. Walter</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Arnout Hyde</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Bill Wasile</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>C. R. Stewart</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>C. R. Thomas</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Charles D. Lemley</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Cook Photo</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>David P. Cruise</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Harry L. Dailey</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Jack B.</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>James Auchincloss</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Norman C. Mahan</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Norman Mahan</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Rimkus</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>S. V. Matthews</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Staley</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Thomas Photo</td>
    <td>3</td>
    <td>0.03</td>
  </tr>
  <tr>
    <td>Antonio Trujillo</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Arza Barnett</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>B. B. Lovins</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Bernard Erwin</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Cazad</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>David Smith</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Erskine</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>H. M. Cazad</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Herb Clagg</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>HUPCO</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Kirk Studio</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Lewis-Smith</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Louise Pote</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Mel Chamowitz</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Michael Anderson</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Proctor Studio</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Rick Haye</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Rinkus</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>S. Matthews</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Signal Corps U.S. Army</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Thornton Barrett</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>U.S. Army Signal Corps</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>Young and Carl</td>
    <td>2</td>
    <td>0.02</td>
  </tr>
  <tr>
    <td>A. G. Gilmour</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>A. H. Plecker</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>A. P. Gates</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>A. P. Snider</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>A. Russell</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>A. W. Warren</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Alex Kahle</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Arnold Sachs</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>B. L.H. Dabbs</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>B. Zadd</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Barnett</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Ben Wooley</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bernard C. Erwin</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Blessing and Kuhn</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bliss Chatfield</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bob Gay</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Bob Kennedy</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Brent Ball</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Burnet</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Burnette</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>C. E. Hancock</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>C. E. Wheelock</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>C. Hancock</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>C. W. Chapman</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Catherine Bliss Enslow</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Cecil W. Stoughton</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>D. F. Brandon</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Dana Forester</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>David Bendann</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Dial</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>E. B. Bensell</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Earp Studio</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Edmunds</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Edward Wilson and W. Irving Adams</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Elizabeth Shoumatoff</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Eplion Studio</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Erskine, Proctor, &amp; Tully Studio</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Eureka Photo</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Everett Julio</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>F. A. Rundle</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>F. Altizer</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fabian Bachrach</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fayer</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fenner</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fred Jones</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Fred William Schaefer</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>G. S. Davis</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Gaston Longet</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Gene Coole</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>George W. Kirk</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Gerald S. Ratliff</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Guy M. Coffman</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>H. J. Lieting</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>H. L. Wasserman</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>H. Monroe Baker</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>H. Nelson</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>H. T. Anthony</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hallman</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Harry Cornwell</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Harry Phillips</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Henry Britt</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Honk</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Huff</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Hupco Studio</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Irvin Dugan</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Italian State Tourist Office</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. Abresch</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. D. Haning</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. L. Giles</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. Murphy</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. Nuzum</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. W. Murphy</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>J. W. Sweeney</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jack Burnet</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jack Dickinson</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>James Abresch</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>James Moran</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jamie Samsell</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jean Thomas</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jemenez</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jim Vallance</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Jim York</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Joe Barta</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Joe Fletcher</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>John G. Fay</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>John McCormack</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>John Miehle</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>John P. Killoran</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>John T. Wild</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>John Watkins and Charles Watkins</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Karl Kemp</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>L. Bernard</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>L. Garcia</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Lewis F. Nathan</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>M. M. Griswold</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mabel Sykes</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mahan of Ashland</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Massey</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Matthew Brady</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Maunce</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Maurice Seymour</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Melvin Grubb</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Merrill Green</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Moseley</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Mosely</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>NASA</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>National Photo Service Company</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Nernard</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Nicola Marschall</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Noel Beard</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>P. C. Hunter</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Premier Studio</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>R. Lee Thomas</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Richard Smith</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Robert H. McNeill</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Rowe Photos</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Shaw</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Stonewall Art Gallery</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>T. A. Morgan</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Tom Hamer</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Tom Jones</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Vandamm</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Virgil Apger</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>W. H. Whitehead</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>W. J. Moulton</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>W. L. Rainer</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>W. P. Bennet</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>W. W. Foster</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>W. Wallace</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Walker Peck</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Wells Photo</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Wild J. B. Boette</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>William Aiken Walker</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>William D. Goebel</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Willie McGehee</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>Zinn</td>
    <td>1</td>
    <td>0.01</td>
  </tr>
</tbody>
</table>



---
layout: page
permalink: /papers/
title: Papers
pubs:

    - year: "2022"
      groups:
        - title:   "HiMFR: A Hybrid Masked Face Recognition Through Face Inpainting"
          author:  "M. Baharul Islam, M. Imran Hosen"
          pub:     "International Conference on Pattern Recognition Workshop: Deep Learning for Visual Detection and Recognition-2022"
          type:     c
          url:     "https://cmt3.research.microsoft.com/DLVDR2022"    
          doi:          
        - title:   "Maked Face Inpainting Through Residual Attention UNet"
          author:  "M. Imran Hosen, M. Baharul Islam"
          pub:     "Innovations in Intelligent Systems and Applications Conference (ASYU 2022)"
          type:     c
          url:     
          doi:       
        - title:   "Emotion, Age and Gender Prediction Through Masked Face Inpainting"
          author:  "M. Baharul Islam, M. Imran Hosen"
          pub:     "Towards a Complete Analysis of People: From Face and Body to Clothes (T-CAP Workshop at ICPR 2022) (Accepted)"
          type:     c
          url:     "https://cmt3.research.microsoft.com/TCAP2022"    
          doi:     
             
    - year: "2021"
      groups:
        - title:   "An Effective Multi-Camera Dataset and Hybrid Feature Matcher for Real-Time Video Stitching"
          author:  "M. Imran Hosen, M. Baharul Islam and A. Sadeghzadeh"
          pub:     "36th International Conference on Image and Vision Computing New Zealand (IVCNZ)"
          type:     c
          url:     
          doi:     "https://doi.org/10.1109/IVCNZ54163.2021.9653352"
          note:          

---

## Publications
Lab faculty members indicated in **bold**. Papers marked using [DBLP](https://dblp.uni-trier.de/){:target="_blank"} color codes.  
{: .pubinfo}
{% for pub in page.pubs %}
### {{pub.year}}
{% for entry in pub.groups %}
{% if forloop.first %}
*({{ forloop.length }} publications)*{: .pubcount}
{% endif %}
{% if entry.internal %}[{{entry.title}}]({{entry.url | prepend: site.baseurl}}){% else %} {% if entry.url %}<span>[{{entry.title}}]({{entry.url}}){:target="_blank"}</span>{% if entry.type=='j' %}{: .journal}{% else %}{: .conf}{% endif %}{% else %}<span>[{{entry.title}}]({{entry.doi}}){:target="_blank"}</span>{% if entry.type=='j' %}{: .journal}{% else %}{: .conf}{% endif %} {% endif %} {% endif %}<br />
<span class="authors">{{entry.author | replace: 'John See', '**John See**' | replace: 'Lai-Kuan Wong', '**Lai-Kuan Wong**' | replace: 'Albert Quek', '**Albert Quek**'}}</span><br />
<span class="publication">{{entry.pub}}
{% if entry.url %} &nbsp;[![pdf](/images/pdf-icon.png)]({{entry.url}}) {% endif %} {% if entry.doi %} [![doi](/images/doi-icon.png)]({{entry.doi}}) {% endif %} {% if entry.note %} <span class="note">[{{entry.note}}]</span>{% endif %}</span>
{% endfor %}
{% endfor %}

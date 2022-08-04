---
layout: page
permalink: /papers/
title: Papers
pubs:

    - year: "2022"
      groups:
        - title:   "Retinal Image Restoration and Vessel Segmentation using Modified Cycle-CBAM and CBAM-UNet"
          author:  "Alnur Alimanov, Md Baharul Islam"
          pub:     "Innovations in Intelligent Systems and Applications Conference"
          type:     c
          url:     "https://cmt3.research.microsoft.com/DLVDR2022"    
          doi:  
	  note:	   "Accepted"
        - title:   "HiMFR: A Hybrid Masked Face Recognition Through Face Inpainting"
          author:  "M. Baharul Islam, M. Imran Hosen"
          pub:     "International Conference on Pattern Recognition Workshop: Deep Learning for Visual Detection and Recognition"
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
          pub:     "Towards a Complete Analysis of People: From Face and Body to Clothes (T-CAP Workshop at ICPR 2022)"
          type:     c
          url:     "https://cmt3.research.microsoft.com/TCAP2022"    
          doi:     
          note:	   "Accepted"   
        - title:   "Stereoscopic Video Quality Assessment Using Modified Parallax Attention Module."
          author:  "Imani, Hassan, et al."
          pub:     "Digitizing Production Systems. Springer, Cham, 2022. 39-50."
          type:     
          url:     "https://www.researchgate.net/profile/Hassan-Imani/publication/356125832_Stereoscopic_Video_Quality_Assessment_Using_Modified_Parallax_Attention_Module/links/61ca1840e669ee0f5c6a953f/Stereoscopic-Video-Quality-Assessment-Using-Modified-Parallax-Attention-Module.pdf"   
          doi:     
          note:	    
        - title:   "Three-Stream 3D deep CNN for no-Reference stereoscopic video quality assessment."
          author:  "Imani, Hassan, Md Baharul Islam, and Nafiz Arica."
          pub:     "Intelligent Systems with Applications 13"
          type:     
          url:      "https://www.researchgate.net/profile/Hassan-Imani/publication/357274721_Three-Stream_3D_Deep_CNN_for_No-Reference_Stereoscopic_Video_Quality_Assessment/links/61ca16eed4500608166fb1f3/Three-Stream-3D-Deep-CNN-for-No-Reference-Stereoscopic-Video-Quality-Assessment.pdf"
          doi:     
          note:	    
        - title:    "A New Dataset and Transformer for Stereoscopic Video Super-Resolution."
          author:  "Imani, Hassan, Md Baharul Islam, and Lai-Kuan Wong"
          pub:     "Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition"
          type:     
          url:      "https://arxiv.org/pdf/2204.10039.pdf"
          doi:     
          note:	   
        - title:    "Triplet Loss-based Convolutional Neural Network for Static Sign Language Recognition"
          author:  "Arezoo Sadeghzadeh, Md Baharul Islam"
          pub:     "Innovations in Intelligent Systems and Applications Conference"
          type:     
          url:     
          doi:     
          note:	  "Accepted"
    - year: "2021"
      groups:
        - title:   "Deep Covariance Feature and CNN-based End-to-End Masked Face Recognition "
          author:  "Masum Shah Junayed, Arezoo Sadeghzadeh, Md Baharul Islam"
          pub:     "IEEE International Conference on Automatic Face and Gesture Recognition"
          type:     c
          url:     
          doi:    
          note:  
        - title:   "Real-Time YOLO-based Heterogeneous Front Vehicles Detection"
          author:  "Masum Shah Junayed, Md Baharul Islam, Arezoo Sadeghzadeh, Tarkan Aydin"	
          pub:     "INISTA-2021"
          type:     c
          url:     
          doi:     
          note:     
        - title:   "An Effective Multi-Camera Dataset and Hybrid Feature Matcher for Real-Time Video Stitching"
          author:  "M. Imran Hosen, M. Baharul Islam and A. Sadeghzadeh"
          pub:     "36th International Conference on Image and Vision Computing New Zealand (IVCNZ)"
          type:     c
          url:     
          doi:     "https://doi.org/10.1109/IVCNZ54163.2021.9653352"
          note:          
        - title:  "Towards Stereoscopic Video Deblurring Using Deep Convolutional Networks."
          author:  "Imani, Hassan, and Md Baharul Islam."
          pub:     "International Symposium on Visual Computing. Springer, Cham"
          type:    c
          url:     "https://yahootechpulse.easychair.org/publications/preprint_download/tp2f"
          doi:     
          note:     
        - title:  "BinoVFAR: An Efficient Binocular Visual Field Assessment Method using Augmented Reality Glasses"
          author:  "Md Baharul Islam, Arezoo Sadeghzadeh"
          pub:     "Symposium on Virtual and Augmented Reality"
          type:    
          url:     
          doi:     
          note:
        - title:  "An Efficient Video Desnowing and Deraining Method with a Novel Variant Dataset"
          author:  "Arezoo Sadeghzadeh, Md Baharul Islam, Reza Zaker"
          pub:     "International Conference on Computer Vision Systems"
          type:    c
          url:    
          doi:     
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

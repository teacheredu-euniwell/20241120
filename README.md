<!--
version:  2024.11.20.01

author:   Manuela Ulrich, Sebastian Tillmann, Sarah Roos, Michael Kowalczyk, Samantha Jacobs

email:    teacheredu.euniwell@uni-konstanz.de

comment:  Self-study Module about Diversity & Inclusion in Education
          
logo:     https://euniwell.de.cool/wp-content/uploads/liascript/images/euniwell-oer-cc-header.svg 

icon:     https://euniwell.de.cool/wp-content/uploads/liascript/images/euniwell-oer-cc-header.svg

language: en

narrator: English Female

mode:     Textbook
dark:     false

date:     20/11/2024

attribute: The OER Self-study Module "Diversity & Inclusion in Education" of the European University for Well-Beeing is licenced under [CC-BY-SA 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/) license.

  ![cc by sa](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/CC_BY-SA_icon.svg/320px-CC_BY-SA_icon.svg.png)

translateWithGoogle: true

@onload
const showFootnote = window.LIA.showFootnote

window.LIA.showFootnote = (ref) => {
  if (window.LIA.settings.mode === "Textbook") {
    document.getElementById("footnote-" + ref).scrollIntoView()
  } else {
    showFootnote(ref)
  }
}
@end

script:  https://h5p.org/sites/all/modules/h5p/library/js/h5p-resizer.js

@h5p_embed: @h5p_embed_(@uid,@0)

@h5p_embed_
<iframe id="h5p_@0" style="width:100%;" srcdoc='<!DOCTYPE html><html lang="de"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0"><style>body{display:flex;justify-content:center;align-items:center;height:100vh;margin:0;background-color:#f0f0f0}.loader{border:16px solid #f3f3f3;border-top:16px solid #3498db;border-radius:50%;width:80px;height:80px;animation:spin 2s linear infinite}@keyframes spin{0%{transform:rotate(0deg)}100%{transform:rotate(360deg)}}</style></head><body><div class="loader"></div></body></html>'></iframe>
<script run-once>
fetch('@1')
    .then(response => {
        if (!response.ok) {
            throw new Error('Netzwerkantwort war nicht ok ' + response.statusText);
        }
        return response.text(); // Abruf als Text
    })
    .then(htmlText => {
        document.getElementById('h5p_@0').srcdoc = htmlText;
        send.lia("LIA: stop");
    })
    .catch(error => {
        console.error('Es gab ein Problem mit dem Abruf: ', error);
        send.error("LIA: stop");
    });

"LIA: wait"
</script>
@end

@style
.admonition {
    padding: 15px 20px;
    margin-bottom: 20px;
    border: 1px solid transparent;
    border-radius: 4px;
    box-shadow: 0 1px 1px rgba(0,0,0,0.05);
    position: relative;
    line-height: 1.4;
}
.admonition::before {
    margin-left: -5rem;
}
.admonition.note {
    color: #31708f;
    background-color: #d9edf7;
    border-left: 5px solid #31708f;
}
.admonition.warning {
    color: #8a6d3b;
    background-color: #fcf8e3;
    border-left: 5px solid #8a6d3b;
}
.admonition.danger {
    color: #a94442;
    background-color: #f2dede;
    border-left: 5px solid #a94442;
}
.admonition-title {
    font-weight: bold;
    margin-bottom: 10px;
}
@end


@admonition: @admonition_(@uid,@0,@1)

@admonition_: <script modify="false">
  setTimeout(() => {
    const parent = document.getElementById('admon-@0').parentElement.parentElement.parentElement.parentElement;

    parent.classList.add("admonition");
    parent.classList.add("@1");

  }, 100);
  `LIASCRIPT: <div class="admonition-title" id="admon-@0">@2</div>`
  </script>

-->

# EUniWell OER self-study module _Diversity & Inclusion in Education_ (Pre-Final)

![Path](d4b91a49393010ddcb82917307b4545165404108.png)

> "People who want inclusion look for ways to make it happen, and people who don't want it look for rationalizations."
>
> -- Hubert Hüppe, Member of the German Bundestag, former German Federal Government Commissioner for Matters relating to Persons with Disabilities.[^1]

---

<center>![EUniWell Logo 600px](fcd26efb0c7e9ee0fc94acd9950ef051f61eb024.png)</center>

---

<center>![Open Educational Resources Logo 400px](5f82bcc0432dc534d4ef6221e42d6da6f3ca5abb.png)</center>

---

<center>![CC-BY-SA Logo](6488c4c276be65038e169dd344ebd104989e611d.png)</center>

---

[^1]: V. Aichele, LL.M., S. Bernot, C. Hübner, S. Kroworsch, B.Leisering, P. Litschke, L. Palleit, K. Pöllmann, J. Striek. (2019). Wer Inklusion will, sucht Wege - Zehn Jahre UN-Behindertenrechtskonvention in Deutschland. Deutsche Institut für Menschenrechte, Monitoring-Stelle UN-Behindertenrechtskonvention. https://www.institut-fuer-menschenrechte.de/fileadmin/Redaktion/Publikationen/Wer_Inklusion_will_sucht_Wege_Zehn_Jahre_UN_BRK_in_Deutschland.pdf Own translation.



## About this OER
The OER self-study module _Diversity and Inclusion in Education_ aims to foster the development of fundamental competences in the field of diversity and inclusion in education.

It was developed as part of Work Package 6 of the [European University for Well-Being (EUniWell)](#6) project at the University of Konstanz.

---

Target Group
----------

The OER is aimed at teachers and student teachers , but it is also open to wider audiences in the area of education.

No prior knowledge is required
-------------------------------------------

[Chapter Overview & Learning Objectives](#3)
------------------------

Duration
----------------
  __The entire module takes about X hour(s)__ <-gelb

Certificate of Participation
-------------------
  
A certificate of participation is available to participants who pass the final examination at the end of the module (with 80% or more correct answers).

ECTS 
---------------

The recommended ECTS allocation is: xxx <-gelb

Accessibility Commitment Statement
---------------------------

We aim to ensure that this Open Educational Resource (OER) adheres to the [WCAG 2.1 Level AA guidelines](https://developer.mozilla.org/en-US/docs/Web/Accessibility/Understanding_WCAG) to the greatest extent possible.

While we strive to meet the criteria outlined for Levels A and AA compliance, please be aware that [LiaScript](https://liascript.github.io/), the main authoring software used for this OER, does not provide specific information regarding accessibility compliance.

We integrate interactive [H5P](https://h5p.org/) modules and use those which are marked as “accessible” in the official [H5P Content types recommendations list](https://help.h5p.com/hc/en-us/articles/7505649072797-Content-types-recommendations).


Feedback
---------
We are committed to continuous improvement and welcome [anonymous feedback](https://padlet.com/teacheredueuniwell/public-feedback-for-euniwell-oer-diversity-inclusion-t9twf0p8n7gd2wo3) on our public feedback wall to discuss and enhance the content quality and accessibility of the OER.

Authors
--------

The content of this OER has been provided by the University of Konstanz as part of the EUniWell project funded by the European Union.

OER Project Team: 

* Sarah Roos (Project Coordination)
* Dr. Manuela Ulrich (Diversity & Inclusion) 
* Dr. Sebastian Tillmann (Unconscious Bias)
* Michael Kowalczyk (Educational Media)
* Samantha Jacobs (Student Assistant)

The case vignettes were created by teacher education master’s students during the 2024 summer semester at the University of Konstanz.

The Chapter Header Illustrations are by [Manfred Steger](https://pixabay.com/de/users/1848497/) published under the [Pixabay Content License](https://pixabay.com/service/license-summary/).

Contact
--------

Email: [teacheredu.euniwell@uni-konstanz.de](mailto:teacheredu.euniwell@uni-konstanz.de)

Creative Commons License
------------------------

The OER self-study module _Diversity and Inclusion in Education_ of the European University for Well-Being is licensed under CC BY-SA 4.0 International.

![CC-BY-SA-150px](5fbe7b9e9f35632164db2917a52dcdf5ce4c8136.png)

Sharing and further processing is expressly permitted subject to the conditions of attribution, non-commercial use, and distribution under the same license conditions.

All content marked as All Rights Reserved are not subject to this license.

Download
-------------- 

* Download the self paced learning module as a SCORM Package (ZIP)
* Download the self paced learning module project files (ZIP)

### Chapters and Learning Goals

![Chapters](8fdfcda3337077656fb061a31c50927ae2f37d2d.png)

> [__About this OER__](#2)

> [__About the EUniWell Project__](#6)

> [__UNESCO Global education report on inclusion and education__](#9)

> [__Chapter 1 - System-Theoretical Perspectives__](#11)
>
> Social structures and global influences determine inclusion and inclusive education in our constantly evolving societies; this framework influences institutions and interactions and shapes the perceptions and identities of groups and individuals. With regard to the aims of inclusion and quality education, we should see the individual in the middle of society. Furthermore, we should look at the everyday interactions in our nearest socio-ecological environments and remind ourselves that thinking and acting in inclusive ways is everyone's responsibility.
> 
> __Learning Goals__
>
> * You are able to describe the significance of inclusive education and its impact on society.
> * You are able to explain the application of systems theory to the school system (including multi-level and ecosystemic models).
> * You are able to describe how symbolic interactionism explains social behaviors related to inclusion. 

> [__Chapter 2 - Discrimination, Diversity and Inclusion__](#16)
> 
> __Learning Goals__
>
> * You are able to define and describe diversity and inclusion and to delineate related concepts such as exclusion, segregation, and integration.
> * You are able to describe forms of discrimination.

> [__Chapter 3 - Inclusion in Global Legal Foundations__](#20)
>
> __Learning Goal__
> 
> * You are able to describe the significance of international treaties and their implications for inclusion in education.

> [__Chapter 4 - Inclusive School Structures and Practices__](#24)
>
> __Learning Goals__
> 
> * You are able to specify what inclusive education means.
> * You are able to explain how inclusive education could be implemented in schools at different levels (i.e. education system, single school, lesson).

> [__Chapter 5 - Examples of Students´ Diversity in Inclusive Classrooms__](#31)
>
> __Learning Goals__
> 
> * You are able to describe the characteristics of student diversity in different dimensions.
> * You are able to appraise situations possibly involving discrimination in schools/lessons, analyse them from the students' point of view, and indicate and justify a course of action appropriate to the situation.

> [__Chapter 6 - Final Quiz__](#41)

> [__Chapter 7 - Unconscious Bias (Add-on)__](#42)
> 
> __Learning Goals__
>
> * You will learn to recognise key features of unconscious bias.
> * You will find out which biases occur in the school environment.
> * You will learn through practical examples how biases can be avoided.


> [__Your Feedback__](#49)

> [__Bibliography__](#50)

> [__Author Credits and Contact Information__](#51)

> [__Downloads__](#52)

### Key Themes 

Education is strongest when it embraces the diversity of individuals. Everyone should have equal educational opportunities. to participate in quality education. Inclusion could make this possible - but we need to consider the complexity of societies here.

__Chapter 1__ 

Social structures and global influences determine inclusion and inclusive education in our constantly evolving societies; this framework influences institutions and interactions and shapes the perceptions and identities of groups and individuals. With regard to the aims of inclusion and quality education, we should see the individual in the middle of society. Furthermore, we should look at the everyday interactions in our nearest socio-ecological environments and remind ourselves that thinking and acting in inclusive ways is everyone's responsibility.

__Chapter 2__ 

People have different characteristics in various social, biological, and psychological dimensions and act differently in their interactions with others. This can lead to discriminatory situations. Looking at the historical development of diversity as well as inclusion and their definitions (and at the problems involved in finding value-free descriptions of the phenomena) reveals that concepts and terms such as diversity, integration, and inclusion have shifted over time. Some researchers refer to a paradigm shift that has taken place in modern society.

__Chapter 3__ 

With the help of global cooperation, international legal frameworks (e.g. the Universal Declaration of Human Rightshuman rights convention) and national ratificationrights (e.g. of the ratification of the UN Convention on the Rights of Persons with Disabilities (CRPD), in Germany in 2009) have been agreed over time to ensure that people can live together in societies without discrimination. Looking to the future, the UN Sustainable Development Goals (SDGs) highlight shared visions and common goals for fostering inclusion as a socio-political process and the well-being of all generations.

__Chapter 4__ 

Educational institutions should ensure that individuals (children, students, teachers, and other involved adults) are aware of global values and inclusive objectives so that they can put them into practice. To achieve this, social institutions need quality frameworks (e.g. multi-professional teams, team teaching, and integrative approaches in the school system)

__Chapter 5__ 

Teachers must be able to respond to the different needs and requirements of each individual student. To achieve this, they must be sensitised to the various dimensions of diversity (social-cultural, biological-physical, and psycho-emotional). Furthermore, they must learn how to react in inclusive lessons, experiment with what makes quality inclusion possible, and engage in reflection with colleagues in the school context and other professionals.

__Chapter 6__

Final Quiz

__Chapter 7 (Add-on)__

The human species benefits from a foundation of specific cognitive abilities. However, this also means that all individuals are influenced by unconscious biases that guide their thoughts and actions throughout their lives - including teachers expected to approach special educational needs or migration fairly.


### Tune in: Keywords and Crossword

Fill in the crossword using terms from the word cloud.

<center>![Crossword](6a4f268f21956c4b8f8bce75420772e09e4a9321.png)</center>

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=25" width="958" height="716" frameborder="0" allowfullscreen="allowfullscreen" title="Crossword"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


## About EUniWell

The European University for Well-Being (EUniWell) is a joint project funded by the European Union. EUniWell unites [eleven European universities](https://www.euniwell.eu/about/universities) with the aim of improving the well-being and quality of life of European citizens.

<center>![EUniWell Logo 600px](fcd26efb0c7e9ee0fc94acd9950ef051f61eb024.png)</center>

Why Well-Being?
---

EUniWell's approach aligns with the Council of the European Union's call for a knowledge-based strategy to advance the "Economy of Wellbeing" and promote synergies between society, research, and the environment. Despite high life expectancies and human development in Europe, the well-being of young people is threatened by challenges like climate change, new diseases, rising populism, societal divides, and war. Addressing these issues requires a holistic approach where higher education, research, and innovation play crucial roles. EUniWell aims to foster well-being through research, education, and civic engagement, shaping policies and pedagogy to enhance skills development and improve the quality of life of European citizens.[^1]

> __Aims of EUniWell__
> 
> "Based on our joint values – democratic, inclusive, diverse, research and challenge-based, inter- and transdisciplinary, entrepreneurial, and co-creational – we aim to develop an action-oriented response to well-being, grounded in high profile research expertise, educational leadership and civic engagement. EUniWell aims to play a critical, intermediary role in shaping research-based policy and pedagogy to inform decision-making, underpin skills development, and realise a measurable impact on our students' learning experience and European citizens' quality of life."[^2]

Systemic Approach
---

EUniWell's five thematic arenas enable a multifaceted and multicultural approach to addressing well-being that leverages the diverse strengths and expertise of the project members. EUniWell's vision emphasises viewing these dimensions from a systemic and global perspective rather than a purely individual one.

<!-- data-type="none" -->
| EUniWell Arenas                                                                                                                                       | Sustainable Developement Goals (especially) |
| ----------------------------------------------------------------------------------------------------------------------------------------------------- |:----------------------------------------------:|
| 1. [Health and Well-Being](https://www.euniwell.eu/what-we-do/research-and-outreach/arena-1-well-being-and-health)                                    |                      (3)                       | 
| 2. [Social Equality and Well-Being](https://www.euniwell.eu/what-we-do/research-and-outreach/arena-2-individual-and-social-well-being)                |               4 / 5 / 10 / (16)                |
| 3. [Environmental Change and Well-Being](https://www.euniwell.eu/what-we-do/research-and-outreach/arena-3-environment-urbanity-and-well-being)        |             6 / 7 / 11 / 12 / (13)             |
| 4. [Culture, Multilingualism, and Well-Being](https://www.euniwell.eu/what-we-do/research-and-outreach/arena-4-culture-multilingualism-and-well-being) |                 (10) / 16 / 17                 |
| 5. [Teacher Education and Well-Being](https://www.euniwell.eu/what-we-do/fields-of-action/arena-5-teacher-education-and-well-being)                             |                      (4)                       |

---

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=19" width="950" height="702" frameborder="0" allowfullscreen="allowfullscreen" title="17 Sustainable Developement Goals"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


---
[^1]: EUniWell. (2023). EUniWell Mission Statement. https://www.euniwell.eu/fileadmin/user_upload/Downloads/Key_documents/2023_EUniWell_Mission_Statement_-_updated.pdf

[^2]: EUniWell. (n.d.). Our Alliance. European University for Well-Being. Retrieved November 19, 2024, from https://www.euniwell.eu/about/our-alliance


### Teacher Education and Well-Being

![Teacher Education](589bb7000e371e9906249dba9a52d00930c50c9b.jpg)

> “We will thus demonstrate that diversity, inclusion, and co-creation do not come at the expense of research excellence, but actually drive and accelerate it, enable equity and enhance universal well-being." 
>
> -- EUniWell (2023)[^1]

Arena 5: Teacher Education and Well-Being
---

The Teacher Education Arena is driven by the Sustainable Development Goal (SDG) "Quality Education" (SDG 4), which brings together many societal needs addressed by other SDGs (e.g. SDG 5 "Gender Equality", SDG 10 "Reduced Inequality"). Its mission is to promote well-being in the school and educational context on the individual, societal, and international levels, in collaboration with many actors in education and civil society. The education and training of (future) teachers and students is one of the pressing challenges and responsibilities of the 21st century. The design of compassionate and vivid school communities, learning environments, and teaching pedagogies plays an important role in advancing the democratic systems and values of our society and its legacy for Europe's future. 

What We Do
--- 

EUniWell aims to increase the attractiveness and the recognition of the teaching profession, the social value of education, and the co-creation of communities of well-being in schools. This will be achieved through the development and dissemination of joint interdisciplinary research, innovative and high-quality education and professional training programmes, the linking of school networks, and the involvement of societal stakeholders. This arena aims to prepare, support, and strengthen our teachers for the current challenges they face in our classrooms and societies. We follow a holistic flat-hierarchy approach that brings different expertise, perspectives, systems, and structures together. We emphasise the necessity of an international, transversal curriculum based on core issues in teacher education such as inclusion and diversity, guidance, sustainability, democracy, health, and the digital transformation and focused on defining and developing key skills for the teaching profession. We are inspired to tackle the phenomena and realities of the 21st century by looking at what lies ahead, across the European continent and worldwide.

Our objectives in Arena 5 are centred around four key areas:
---

1. __Innovative research__ 

     Advancing trans-institutionaljoint research in the area of teacher education and well-being. Analysing new educational and pedagogical affordances, defining diverse professional skills and training needs, especially for second career teachers. Exploring innovative approaches and training.

2. __Teacher education programs and educational provision__ 

     Developing academic content and supporting training provision focused on the professionalisation of teaching, lifelong learning, and skills for the future, especially in the area of multilingualism and cultural competences. Defining and expanding a common guiding framework based on professional standards elaborated during EUniWell's pilot phase. Creating open educational resources (OERs), online and hybrid training modules and courses, especially for cross-cutting topics (e.g. such as diversity and inclusion, or social media and digital literacy).

3. __Collaboration and networking__ 

     Facilitating knowledge exchange and networking opportunities for actors of all career phases according to their specific needs. Connecting local schools by expanding the European School Network established during EUniWell‘s pilot phase, bringing together teacher educators, students and civic stakeholders. Organising international conferences and lecture series addressing current and future challenges encountered by teachers and educators.

4. __Community engagement__ 

     Linking theoretical and practical knowledge transfer locally and globally. Creating international mobility experiences for teaching student teacherss, e.g. by promoting internships to foster a global sense of community through the experience of a local sense of belonging. Developing regionally-based training pacts to tackle international questions with local solutions.

(EUniWell, 2024)[^2]


[^1]: EUniWell. (2023). EUniWell Mission Statement. https://www.euniwell.eu/fileadmin/user_upload/Downloads/Key_documents/2023_EUniWell_Mission_Statement_-_updated.pdf

[^2]: EUniWell Teacher Education Team. (n.d.). Arena 5: Teacher Education and Well-Being. European University for Well-Being. Retrieved Winter 11, 2024, from https://www.euniwell.eu/what-we-do/fields-of-action/arena-5-teacher-education-and-well-being



### Definition of Teachers´ Professional Standards

> "In a new social contract for education, teachers must be at the centre and their profession  
> revalued and reimagined as a collaborative endeavour which sparks new knowledge to bring about 
> educational and social transformation 
>
> -- UNESCO (2021)[^1]

One of the key foci that were adressed during EUniWell´s pilot phase (2019-2023) was the need for further professionalization of teaching,  especially for the future generations of teachers, in order to prepare them for the pressing environmental, technological, and social challenges they are facing on a national and international level. Therefore teacher training should provide and equip them with future skills like "sustainability, well-being, inclusion, and social cohesion." (Del Gobbo et al., 2023)[^2].

In a first step, based on literature and on the survey comparison of professional standard frameworks per country, common professional standards for European teachers were defined in new competence areas, with the aim to establish a common framework for learning outcomes for European Teacher Education. This should lead, in a second step, to the definition of a transversal curriculum for European teachers.

<center>![Teacher Education Arenas Logical Framework](6bc7dc2ca1faf27fb016f3bb78f6f529e554db2f.png) Teacher Education Arenas Logical Framework, Del Gobbo et al. (2023)[^2]</center>
<br>

The new competence areas for teachers' professionalization were defined as:

1. Sustainability
2. Healthcare
3. Well-being
2. Inclusion

For each area, professional standards have been identified and articulated into sub-professional standards, and the related professional behaviours expected by teachers of the future. 

Professional Standards for Inclusion
====

The idea of inclusion refers both to an ideological stance and an approach to designing education.

"When referring to the design of education, inclusion implies a classroom where the diversity of students is acknowledged in that all students are provided with a meaningful education (Florian, 2017[^3]; Popkewitz, 2004[^4]). Thus, an inclusive classroom holds a diversity of students where inclusion regards social, spatial, and didactical aspects of education (Asp-Onsjö, 2006[^5]).

* The teacher is knowledgeable and confident in implementing research-based inclusive education.
* The teacher is able to plan and adapt differentiated education, respecting the different needs of students.
* The teacher promotes supportive education, aiming at fostering independent, self-confident, and critical learners." 

(EUniWell, 2022)[^6]

Examples of Professional Standards and Related Professional Behaviours (Inclusion)
---

<!-- data-type="none" -->
| Core Competence                          |                                      Professional Standards                                       |                                                                                                                          Sub-Components Standards |                                                   Expected professional behaviour |
| :---------------------------------------- |:-------------------------------------------------------------------------------------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------| :---------------------------------------------------------------------------------|
| Create an inclusive learning environment | Being able to plan and adapt differentiated education that respects the different needs of students |                                                                          Being able to plan inclusively and accommodate the (special) needs of pupils.  | Assessing each student's abilities and challenges within the specific learning group | 
| -                                        |                                                 .                                                 | Being able to adapt curriculum requirements to students' (special) needs and being able to create differentiated learning materials and environments |Adapting curriculum requirements to students' (special) needs and creating differentiated learning environments|

(EUniWell, 2022)[^6]

[^1]: UNESCO, International Commission on the Futures of Education. (2021). Reimagining our futures together: a new social contract for education. UNESCO. https://doi.org/10.54675/asrb4722

[^2]: Del Gobbo, Daniela Frison, André Bresges, Donna J. Dawkins, Jan Springob, Juan Antonio Solis Becerra, Ibolya Túri, Magali Hersant, Giovanna. (2023). Sustainability, health care, well-being, and inclusion: toward new professional standards for the teachers of the future. Nuova Secondaria , 5, 146-154.

[^3]: Florian, L. (2017). Teacher education for the changing demographics of schooling: Inclusive education for each and every learner. In Teacher education for the changing demographics of schooling (pp. 9-20). Springer, Cham.

[^4]: Popkewitz, T. S. (2004). Educational standards: Mapping who we are and are to become. The Journal of the Learning Sciences, 13(2), 243-256.

[^5]: Asp-Onsjö, L. (2006). Åtgärdsprogram - dokument eller verktyg? En fallstudie i en kommun. https://gupea.ub.gu.se/handle/2077/16941

[^6]:EUniWell, University of Florence. (2022). Deliverable Report (D3.27) Definition of common professional standards for European teachers.



## UNESCO Global Education Report on Inclusion and Education

> "Education makes an essential contribution to building inclusive and democratic societies, where differences of opinion can be 
> freely expressed and where the wide range of voices can be heard, in pursuit of social cohesion and in a celebration of diversity." [^1]
>
> --Right Honourable Helen Clark, Chair of the GEM Report Advisory Board, Former Prime Minister of New Zealand.

Inclusion and Education
-------

Watch the Inclusion and Education: #AllmeansALL video presenting insights from the 2020 UNESCO Global Education Monitoring report.

This video provides an overview of how education that is not inclusive affects children and what can be done to promote change and to ensure that all children have access to an inclusive and equitable quality education.

!?[UNESCO 2020 Global Education Monitoring Report](https://www.youtube.com/watch?v=kEyjlqixq9c "Source: https://www.youtube.com/watch?v=kEyjlqixq9c")

<details>

<summary>~~**Click here to show the Video Transcript**~~</summary>

Intro:

Everyone is different. The 2020 Global Education monitoring report on inclusion and education believes that education is strongest when it embraces diversity. Learners should not have to adapt to the system; instead, education systems should adapt to their needs. When students do not feel welcome in school, they are less likely to learn. This is everyone's loss. But rich and poor countries too often educate some children apart. Children who have a disability, have been displaced, speak a different language, or are poor and disadvantaged.

Problems:

School design may favour some students over others, as do many laws and policies. Teachers are often ill-equipped to cater for students diverse needs. Children may not recognise the way they are portrayed in textbooks. Some may not see themselves there at all. They receive the message that they do not belong. Testing sometimes follows a narrow vision of education and consequently some students leave education earlier than they should. These are complex problems to solve, but a belief in the right to education is a belief in inclusion. Children have different learning speeds and needs. They need curricula that are flexible, creative and relevant. How we prepare teachers matters. They must be given the tools and training to achieve our vision for reform. The resources we know can help the marginalised. Educators, support staff and equipment should be shared so that everyone can benefit.Better data on those left behind will help us reach them. Disadvantages often accumulate. We can't address inclusion one group at a time.

Conclusion:

Redressing these disadvantages requires funds. These must be equitable and target individual specific needs. We must work together on these tasks across government ministries, from central to local authorities with civil society supporting governments and  schools opening doors to the community. Inclusion in education requires a change in mindset in society, so that education for all means education for everyone without an exception. Achieving this is everybody's business, including yours.

</details>

---

For more information download the full report on the [UNESCO 2020 Global Education Monitoring Report website](https://www.unesco.org/gem-report/en/inclusion)

---

[^1]: UNESCO. (2020). Global Education Monitoring Report 2020: Inclusion and education: All means all. Paris. UNESCO. https://doi.org/10.54676/jjnk6989

In the Next Chapter
---
The next chapter outlines the underlying social structures that influence the development, perception, and handling of inclusion and diversity and will help you to reach a more in-depth understanding of this area.


## 1. Systems Theory Perspectives

![Theory Lecture](d0855f7569cb6b14f58a621ca2df352bd2b07792.png)

To help you to gain a broader and deeper understanding of the central topics of diversity and inclusion and of wider social facts and processes, we will begin with a look at selected theories and models from the educational and social sciences.References to school theory are highlighted and specific examples of teacher professionalisation are explained.

> __Learning Goals__
>
> * You are able to describe the significance of inclusive education and its impact on society.
> * You are able to explain the application of systems theory to the school system (including multi-level and ecosystemic models). 
> * You are able to describe how symbolic interactionism explains social behaviours related to inclusion.


### 1.1 Interrelations of Main Social Systems

Early sociologists assume certain universal functional requirements in societies and recognise a de facto differentiation of social systems (Parsons, 1968)[^1]. The sociological model below, "Social Subsystems" by Fend (2009)[^2] represents a structural-functionalist perspective.

It forms the basis of school theory and depicts three major systems of society in abstract terms. The decisive factors here are the interrelationships and the fact that school is located as an institution in the Eeducation system that dependsing on the politicsal and economic systems.

<center>![Global Organisations and Systems](9d7fc7ffa434c017de67ef5df1028cf0633d4358.png) Global Organisations and Systems, own illustration based on Fend (2009) p.36 [^2]</center>
<br>

The model shows that the socialisation order of a society can be characterised by the three subsystems of politics, economics and education.

* The __political system__ sets the framework conditions for the other two systems.

* The __economic system__ organises work and the production and distribution of goods.

* The __education system__ organises the production of qualifications and mental infrastructures.

Under the conditions of increasing global competition between economic centres, for example, the EU considered it necessary to invest in people in order to raise the level of education of the entire population. Education, understood as a labour market-related qualification, was given central importance. At the same time, educational institutions such as schools must ensure that individuals acquire the skills they need to participate in society. By acquiring these social skills, individuals should be able to strengthen democratic development and social cohesion.

Despite this orientation of the education system, not all individuals can participate equally. This leads to marginalisation and individual disadvantage, for example due to race and social background.

Social Movements
---
Initiated by successful anti-discriminatory social activists, political guidelines and recommendations were established (e.g. US Civil Rights Act 1964). In particular, education systems were called upon to engage in the establishment of inclusive development in the sense of progressive, sustainable modernisation.

Inclusion as a Special Phenomenon in Current Society
---

Let us imagine inclusion at the centre of this social systems model.

<center>![Inclusion in the Center of Social Systems](532d6c4d7706b6c5685e028a77b44b02da5da557.png) Inclusion in the Center of Social Systems, own illustration based on Fend (2009) p.36[^2]</center>
<br>


With regard to the education system, schools as institutions have the tasks of __ensuring inclusion__ and __further developing inclusion__. Last but not least, inclusion is about the individual in society. In the education system, this concerns students, teachers, parents, and school management.



What You Will Find in the Next Section
---

We use Bronfenbrenner's socio-ecological model to illustrate the position of the individual within social structures.

[^1]: Ellis, D. P. (1968). SOCIOLOGICAL THEORY AND MODERN SOCIETY. By Talcott parsons. New York: The free press 1967. 564 pp. $12.50. Social Forces; a Scientific Medium of Social Study and Interpretation, 47(1), 90–91. https://doi.org/10.2307/2574723

[^2]:Fend, H. (2009). Neue Theorie der Schule. VS Verlag für Sozialwissenschaften. https://doi.org/10.1007/978-3-531-91788-7

### 1.2 Bronfenbrenners Ecological Systems Theory

Uri Bronfenbrenners Ecological Systems Theory posits that human development is influenced by the interactions between an individuals and their multiple _environmental systems_. (Bronfenbrenner 1977)[^1] These systems are nested within each other, each layer representing a different level of influence. 

Video: Bronfenbrenner´s Ecological Systems 
---

!?[](https://www.youtube.com/watch?v=g6pUQ4EDHeQ)

<details>

<summary>~~**Click here to show the video transcript**~~</summary>

In 1964, a young psychologist appeared before the US congress with a mission.
It was a time when most people thought that the reason poor people stayed poor was a matter of biology 
and had nothing to do with the environment they grew up in.

The psychologist, Uri Bronfenbrenner, wanted to change that and convince the world that to help those less fortunate, we also need to
change their surroundings. But did he succeed?

Bronfenbrenner's Ecological System Theory conceives that a child is influenced by five ecological forces.

First comes the microsystem of family and friends that affect the child directly.
Second are the forces of the connections between the people around the child:parents with teachers and teachers with peers.

Then there are links between social settings that do not directly involve the child,such as the father with his boss,the peers with
their parents and the teacher with the principal. 

Next, is the overarching culture, religion and social norms that influences all others. 
And lastly, there is time - which changes everything over the course of one’s life.

Children are born into a Microsystem that influences the child's experiences directly.

Children from unfortunate backgrounds are more likely to experience problematic family structures 
-even if it’s simply for the fact that parenting is more difficult if you are poor.

They also encounter more negative situations at school or bad influences through friends.

Consequently, a child that grows up in a negative microsystem,will find it hard to succeed. 

The Mesosystem represents the interconnections between the elements that surround the child. 
For example the relationship between the father and the school teachers.

If the father doesn’t get along with a teacher,the child might suffer.

The EXOSYSTEM involves links between social settings that do not involve the child.

For example, a child's experience at home can be influenced by their parent's experiences at work.

If the mother loses her job, there might be more arguments with the father,resulting in changes in their interaction with the child.

The MACROSYSTEMdescribes the overarching culture that influences all other systems,such as a child’s geographic location and ethnicity.

Intelligent people who happen to live in bad places are more likely to move to better ones.

But that also means that they are more likely to be strangers in a richer society.

So regardless of the child’s biological potential or upbringing, on a macro level he or she may still be at a disadvantage.

The CHRONOSYSTEM,refers to changes in the child,and the environment over time.

As the child grows up the parents may stop loving each other and divorce, which can be traumatic for an eight year old boy.Five years later,
he may have come to terms with how things turned out.But when the boy turns 16, his mom’s new boyfriend moves into their tiny 
apartment, and things get difficult again.

Bronfenbrenner, who was influenced by Lev Vygotsky and Kurt Lewin, convinced the US congress that a child’s prospect is not
genetically predestined,but is the result of the larger environment they happen to be placed in.

Children who grow up in unfortunate social structures therefore need a form of support that not only reaches their families,but also
elements of their community. 

Bronfenbrenner's theory helped form the Head Start program in 1965,a government program that has served more than 35 million poor children since. 

Decades later, Bronfenbrenner and Stephen Ceciproposed an extension of this theory, called the "bioecological model".

This new model recognizes gene–environment interactions and acknowledges the role of heritability, but adds that genes themselve are under the
influence of the environment.

In other words, the process of heritability varies in a magnitude of potentials.

How much a child can make of the potential they inherit,depends on the ecological environment.

Bronfenbrenner made a critical contribution to our realization that parent-child relationships do not exist in a social vacuum but are embedded
in the larger structures, such as community, society, and culture.

In order to develop well, he allegedly said, “every child needs at least one adult who is irrationally crazy about him or her.”

Now it’s your turn,make five circles, draw yourself in the center and add a timeline at the bottom. Then add all the people, institutions and forces that affect your life.

On the timeline below you can add some major events from the past and those you expect in the future.

Can you tell how the 5 forces are shaping your life?

</details>

---

Microsystem
-----
"The _microsystem_ encompasses all those factors that are attributed to an individual and their  actions by another individual, i.e. certain external characteristics, abilities, etc. These are personal influencing variables that are localised in the individual (Seifert 2011, S.115f.)" quoted from Epp (2017)[^2]. 

Mesosystem
-----
"The _mesosystem_ "comprises the interrelationships between the areas of life in which the developing person is actively involved (for a child, for example, the relationship between home, school and group of mates; for an adult, the relationship between family, work and circle of acquaintances)" (Bronfenbrenner 1981, p.41). Accordingly, the various life contexts in which an individual moves belong to the mesosystem (Seifert 2011, S.118)" quoted from Epp (2017)[^2].

Exeosystem
-----
"An _exosystem_ is understood to be areas "in which the developing person is not personally involved, but in which events take place that influence or are influenced by what happens in their area of life" (Bronfenbrenner 1981, p.42). This includes formal and informal social structures, [...] This includes the larger institutions of society - not only those that are systematically structured, but also those that arise spontaneously - and how these unfold at the concrete local level (Bronfenbrenner 1978,S.36)" quoted from Epp (2017)[^2].

Makrosystem
---
"The concept of the _macrosystem_ "refers to the fundamental similarity in form and content of the lower-order systems (micro-, meso- and exo-) that exist or could exist in the subculture or the entire culture, including their underlying worldviews and ideologies" (Bronfenbrenner 1981, p.42). [...] which permeate society as a whole. This includes, for example, political, economic, social, legal or educational patterns (Bronfenbrenner 1978, p.36)". quoted from Epp (2017)[^2]

![The ecosystemic development model](https://euniwell.de.cool/wp-content/uploads/liascript/images/bronfenbrenner-epp.png "The ecosystemic development model according to Epp (2017)[^2] - translated from German")


By understanding these layers of influence, educators can be sensitised to create more inclusive and diverse educational environments.


Now it´s your turn
-------
Paint the Bronfenbrenners ecosystem circles and draw yourself in the center. Fill in the circles reflecting on the following questions.

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=31" width="958" height="276" frameborder="0" allowfullscreen="allowfullscreen" title="Questions for Bronfenbrenner"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


---

In the next section
-------

Given the interactions and influence of individual thought structures in relation to inclusion in this complex framework, we will consider the level of interaction between two individuals. The theory of sysmbolic interactionism will help us to understand how new meanings and thought structures can emerge from interactions.

---

[^1]:Bronfenbrenner, U. (1977). Toward an experimental ecology of human development. The American Psychologist, 32(7), 513–531. https://doi.org/10.1037/0003-066x.32.7.513

[^2]: Epp, A. (2017). Bronfenbrenner’s Ecological Systems Theory as a Sensitization and Examination Pattern for Empirical Analyses. Forum Qualitative Sozialforschung Forum: Qualitative Social Research, 19(1). https://doi.org/10.17169/fqs-19.1.2725

### 1.3 Symbolic Interactionism Theory

In his symbolic interactionism theory Mead (1986)[^1] distinguishes three concepts of the individual: I, ME & SELF.

* __I__

   Mead understands the "I" as a psychological component. This is where people's creative and impulsive emotions and actions occur. 

* __ME__

  The "Me" is the social component and the objective part of the person. It is shaped by the respective society and comes into conflict with external expectations and attitudes of other people.

* __SELF__
  
  The "Self" arises from the interaction between Me and I and develops from processes of experience and development. 
  
  The Self is not a fixed construct and continues to develop in the process.

  The Self reflects a person's self-perception and self-image.

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/i-me-self.png "Individuum: I, ME & SELF., own illustration")

Based on the descriptions and theoretical considerations, we can deduce that _inclusive attitudes_ and the _sense of belonging_ they create are also ongoing social-systemic and individual developments. In social interactions, we can actively shape inclusion and reflect on our own inclusive attitude.

The following model, based on the idea of symbolic interactionism theory (Mead,1986 see also Joas,1989;Helle,2001)[^1] shows how inclusion can arise from social interactions and result in an individual attitude.

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/inclusive-attitudes.png "Individuals´ interaction, own illustration.")


In the next section
---------
In the following you can test your acquired knowledge.

---

[^1]: Mead, George H. (1968 [1934]). Geist, Identität und Gesellschaft: aus der Sicht des Sozialbehaviorismus (Ed. Ch.W. Morris). Berlin: Suhrkamp. / Joas, Hans (1989). Intersubjektivität – Die Entwicklung des Werkes von G. H. Mead. Berlin: Suhrkamp. / Helle, Horst J. (2001). Theorie der symbolischen Interaktion: ein Beitrag zum verstehenden Ansatz in Soziologie und Sozialpsychologie (3rd ed.). Düsseldorf: Westdeutscher. 


###	1.4 Summary Quiz

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=30" width="958" height="687" frameborder="0" allowfullscreen="allowfullscreen" title="Fends Social Systems Interaction (Drag &amp; Drop)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=29" width="958" height="688" frameborder="0" allowfullscreen="allowfullscreen" title="Bronfenbrenners Ecological Model (Drag&amp;Drop)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


## 2. Discrimination, Diversity and Inclusion


![](https://euniwell.de.cool/wp-content/uploads/liascript/images/flux.png)

This chapter looks at the definitions of diversity and inclusion. From a social-historical perspective, we take a closer look at conceptual changes and differences of _exclusion_, _separation_, _integration_, and inclusion in education. With regard to actual recognition of diversity, we also take a closer look on the term _discrimination_ as the opposite of inclusion.

> __Learning Goal__
>
> * You are able describe basic definitions of "diversity", „inclusion“ and to deliniate related concepts such as exclusion, separation and integration.
> * You are able to describe forms of discrimination.

### 2.1 Definitions

The ethymological origin of discriminate is in Latin "discriminare" and means, to distinguish, separate, segregate.

Discrimination takes place in many areas of everyday life: Housing, education, the employment system, health and social services, policing, the administration of justice, representation in the media and political participation. In social science and political discussion, discrimination refers to disadvantages identified on the basis of group-specific differences in accordance with the principles of equality and equal treatment. 

> __A Definition of Discrimination__
>
> "treating a person or particular group of people differently, especially in a worse way from the way in which you treat other people, because of their race, gender, sexuality, etc."[^1]

Further examples are religion, political beliefs, age, health and gender identity. Catalogs of characteristics are open-ended. [^2]

Forms of discrimination
---
* Direct discrimination
* Indirect discrimination
* Harassment
* Bullying
* (Multiple discrimination or multidimensional discrimination)
* Intersectional deiscrimination

Following the definition, we would like to add that since the UN Convention, "people with disabilities" should be explicitly added to dictionary contributions. Age could also be recorded; the relevance is reflected, for example, in the educational science discussion of children's rights and in the debate about when young people are allowed to vote politically. People in nursing homes also often experience discrimination.

> Please, think about your own biographie and current life remembering: Where have I experienced discrimination myself in my childhood as a student?

Is there any current situation in my social or physical environment where I meet discrimination in the narrow or broad sense? Feel free to note your own definition of discrimination according to the current situation - even if it is not you who is affected, but another person in your environment.

[^1]: https://dictionary.cambridge.org/dictionary/english/discrimination
[^2]: https://heimatkunde.boell.de/de/2008/02/18/institutionelle-diskriminierung-im-bildungs-und-erziehungssystem-theorie


The current concepts are subject to the current problem that there is no standardised definition. Due to the orientation of this OER, we are working on the following book chapters / articles: 

* Walgenbach (2021)[^1] and Bührmann (2018)[^2] for the term of diversity.
* Cramer and Harant (2014)[^3] and Stichweh (2007)[^4] for the term of inclusion.

These articles provide a value-free definition of diversity on the one hand and a sociological definition of inclusion on the other.

> __Definition of Diversity__
>
> We define diversity as social fact that reflects the variety and difference of
> individuals in a society. The variety and difference is reflected on three levels. 
> __1.__ social, __2.__ biological, __3.__ psychological-emotional.

> __Definition of Inclusion__
>
> Stichweh (2007, p. 113)[^4] distinguishes between three contexts of origin:
>
> __1.__ _Sociological systems theory_ - this speaks of inclusion and exclusion by 
> analysing the form of participation and consideration of people in social systems. 
>
> __2.__ _French social theory_, which since Durkheim has almost united the concept of 
> inclusion with that of solidarity in a society. Inclusion and exclusion then 
> signify the success or failure of solidarity. 
>
> __3.__ _British welfare state theory_, which 
> conceptualises the communicative consideration of people in social systems as 
> membership according to the _paradigm of citizenship_.

---





[^1]: Walgenbach, K. (2021). Erziehungswissenschaftliche Perspektiven auf Vielfalt, Heterogenität, Diversity / Diversität, Intersektionalität. Verlag Julius Klinkhardt. https://doi.org/10.25656/01:22247
[^2]: Bührmann, A. D. (2018). Diversität. socialnet Lexikon [last access: 26.09.2024]. https://www.socialnet.de/lexikon/6324
[^3]: Cramer, C., & Harant, M. (2014). Inklusion – Interdisziplinäre Kritik und Perspektiven von Begriff und Gegenstand. Zeitschrift fur Erziehungswissenschaft: ZfE, 17(4), 639–659. https://doi.org/10.1007/s11618-014-0584-4
[^4]: Stichweh, R. (2007). Inklusion und Exklusion in der Weltgesellschaft – Am Beispiel der Schule und des Erziehungssystems. In J. Aderhold & O. Kranz (Eds.), Intention und Funktion (pp. 113-120). VS. https://doi.org/10.1007/978-3-531-90627-0_5


### 2.2 Exclusion, Separation, Integration & Inclusion in Education

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=23" width="958" height="604" frameborder="0" allowfullscreen="allowfullscreen" title="UN-CRPD Extinction, Exclusion, Separation, Integration, Inclusion"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>

Source [^1]

Kuhzl in 2015 umwadneln

In the next section
--------
We want to invite you to reflect about discrimination.



[^1]: Grosche, M. (2015). Was ist Inklusion? Ein Diskussions- und Positionsartikel zur Defi nition von Inklusion aus Sicht der empirischen Bildungsforschung. In P. Kuhl, P. Stanat, B. Lütje-Klose, C. Gresch, H. A. Pant, & M. Prenzel (Eds.), Inklusion von Schülerinnen und Schülern mit sonderpädagogischem Förderbedarf in Schulleistungserhebungen (pp. 17–39). Springer Fachmedien Wiesbaden. https://doi.org/10.1007/978-3-658-06604-8




### 2.3 Exercise: Thinking About Inclusion from a Student Perspective
-------------------

> "Inclusive education is differentiated from “integration,” which was identified with the late 1970s and 1980s advocacy movement to educate students with developmental disabilities in regular schools albeit in self-contained classrooms rather than in special education schools with little or no contact with general education students, settings, or curricula (Sailor et al., 1989) and from _“mainstreaming,”_ in which students with disabilities are members of special education classes but “visit” general education classes to engage in educational and social activities with same-age general education peers (Halvorsen & Neary, 2001; Sailor, 1991). Unlike integrated or mainstreamed students, students who receive inclusive educational services are members of the general education classroom community. According to Halvorsen and Neary (2001), “the single most identifiable characteristic of inclusive education is membership. Students who happen to have disabilities are seen first as kids who are a natural part of the school and the age appropriate general education classroom they attend” (Hunt & McDonnall, 2007, S. 270)[^1]


Task: Interactive reflection on inclusive settings in the classroom
---

Watch the following video to get an understanding of the differences between integration, perceived inclusion and true inclusion.

Pay attention on the following:

* How homogeneous and heterogeneous is the class community portrayed?
* Observe who is located and moves where in the classroom?
* Who interacts with whom and how?
* What impressions, feelings and wishes does the narrator describe?


!?[What Is Inclusion?](https://www.youtube.com/watch?v=3VMz06iVzqs&t=32s)


<details>

<summary>~~**Click here to show the video transcript**~~</summary>

Integration

I don't understand why I'm at the back  f the class. I wish I was like everyone else. I want to do what they are doing. But here I am doing this a same old number activity watching as my classmates learn something else. Don't they know that they're setting me up to fail? Don't they know they hold my future in their hands? I want to work in my class, learn what they are learning and do the activities they do. But here I am stuck at the back, limited by low expectations. Having a one-on-one teacher aide just teaches me to rely on them and means I get less attention from the teacher. I'm not included in the classroom, I am in the same room but segregated from my peers, sat to the side or back working on different things and missing out. I want to be free to learn with my peers reach my full potential and be seen to be like everyone else. I need something to change. 

Perceived inclusion

You may be wondering what was wrong with this picture? I'm in the classroom with my peers, sitting on my seat, learning the same things as everyone else. You may think this is inclusion, but it's not. I am stifled, limited and held back from reaching my full potential. Though I love my teacher aid, I don't get to think for myself. In fact a lot of the time my teacher aid does it for me, even whispering the answer in my ear when I already know it. The more she is with me the more I realized that there is no point in me thinking for myself because she would give me the answer anyway. I'm sure there are other kids who also need to her help, does she need to be with just me? Can´t she help others? Surely If I need help I can put my hand up and ask my teacher like my friends do. My friends and classmates want to help me but by having someone right next to me they can't. I need to learn from my peers, be able to do group work and be challenged. I want to be allowed to fail or succeed and learn from it. I need something to change. 

Inclusion

Can you find me in the crowd? Inclusion is more than just a word. It is a culture, a mindset and an expectation that everyone can and will learn and succeed along their age-appropriate peers. I know it can be challenging to include me in the learning as sometimes I might require extra resources and information but giving me space to learn from my teacher and peers is the best way to challenge me and allow me to grow. I want to learn the same things as my classmates and I want teachers to have the same expectations of me as my friends. Mmy learning may need to be modified by I still want the opportunity to show what I can do, not focus on what I can't. Treat me the same as any other student and watch me flourish. I will rise to the challenge of expectations you set for me. Are you ready to really include me?

</details>

---

Drag & Drop you observations into the corresponding field.
-------

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=32" width="958" height="688" frameborder="0" allowfullscreen="allowfullscreen" title="Integration, percieved inclusion &amp; inclusion (Drag &amp; Drop)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


[^1]: Hunt, P., & McDonnall, J. (2007). Inclusive education. In van der Gaag, R.J. S. L. Odom, R. H. Horner, M. E. Snell, & J. Blacher (Eds.) (2007). Handbook of developmental disabilities. New York/Londen: Guilford Press. https://doi.org/10.1007/BF03089708

## 3. Inclusion in Global Legal Foundations

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/human-rights.png)

Inclusion is a historically evolved concept whose basic idea is anchored in human rights.

Its establishment in the UN Convention on the Rights of Persons with Disabilities, which is based on a fundamental human rights-based understanding of disability, has contributed to its general dissemination.

Subsequently, the concept of inclusion was partly detached from its reference to people with disabilities and became a general principle for dealing with diversity in society. The perception of the increasing divide between people in different socio-economic situations, gender issues, generational conflicts and the challenges of cultural and religious diversity in the face of increased migration also came into focus.

> __Learning Goals__
>
> * You are able to describe the significance of international treaties and their implications for inclusion in education.


###	3.1 Treaties as Historical Milestones.

International legal treaties and frameworks play a crucial role in advancing global standards for human rights and inclusion and diversity in education.

Among the most influential are the __1948 Universal Declaration of Human Rights (UDHR)__, the __1966 International Covenant on Civil and Political Rights (ICCPR)__, and the __International Covenant on Economic, Social and Cultural Rights (ICESCR)__. Together they formed the bedrock of international human rights law, also emphasizing the universal right to education.

The __1989 Convention on the Rights of the Child (CRC)__ further underscored the specific needs and rights of children, advocating for their right to receive education in a manner that respects their inherent dignity and promoted their overall development. Complementing these frameworks, the Salamanca Statement adopted in 1994, called for inclusive education systems that accommodate all children, regardless of their physical, intellectual, social, emotional, linguistic, or other conditions.

In addition, the __2006 Convention on the Rights of Persons with Disabilities (CRPD)__ strengthened the commitment to inclusion by emphasizing the right of persons with disabilities to access quality education without discrimination and on an equal basis with others. This Convention has been instrumental in shifting perspectives towards a more inclusive and equitable approach to education.

The __Sustainable Development Goals for 2030 (SDGs) __established in 2015, particularly Goal 4.5 which aims to eliminate gender disparities in education and ensure equal access to all levels of education for the vulnerable provided a comprehensive roadmap for global education development.

Together, these international legal instruments and goals compel governments and educational institutions to recognize and address the diverse needs of all learners.

Timeline of international humann rights and education for all treaties
-----------------------

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=15" width="95%" height="625" frameborder="0" allowfullscreen="allowfullscreen" title="EN - Timeline - Legal Foundations for Diversity &amp; Inclusion in Education"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>

### 3.2 Sustainable Developement Goals 2030 (SDGs) 2015

The [Sustainable Development Goals (SDGs)](https://sdgs.un.org/goals) were established in 2015 during the United Nations Sustainable Development Summit as a universal call to action to end poverty, protect the planet, and ensure prosperity for all by 2030. 

They were created to address the global challenges facing humanity, including inequality, climate change, and peace and justice.

SDG 4 - Quality Education
---

__Sustainable Development Goal (SDG) 4__ on education calls for inclusive and equitable quality education and lifelong learning
opportunities for all by 2030. It emphasizes inclusion and equity as laying foundations for quality education and learning.

SDG 4 also calls for building and upgrading education facilities that are child-, disability-, and gender-sensitive and for
providing safe, non-violent, inclusive and effective learning environments for all.

To achieve this ambitious goal, countries should ensure inclusion and equity in and through education system and programs.
This includes taking steps to prevent and address all forms of exclusion and marginalization, disparity, vulnerability and
inequality in educational access, participation, and completion as well as in learning processes and outcomes. It also requires
understanding learners’ diversities as opportunities in order to enhance and democratize learning for all students. See UNESCO (2017)[^1]

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=19" width="950" height="702" frameborder="0" allowfullscreen="allowfullscreen" title="17 Sustainable Developement Goals"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>

---

[^1]: UNESCO. Assistant Director-General for Education, 2010-2018 (Qian Tang), & UNESCO. (2017). A Guide for ensuring inclusion and equity in education. UNESCO. https://doi.org/10.54675/mhhz2237

###	3.3 Summary Quiz

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=37" width="958" height="544" frameborder="0" allowfullscreen="allowfullscreen" title="International treaties (Question set)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>

## 4. Inclusive School Structures and Practices

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/school.png)

It becomes clear that inclusion is a sense of belonging, feeling respected and valued and being seen for who we are as individuals. However, it takes a certain level of commitment and supportive energy from school leaders and colleagues, as well as other educators, for us as individuals and as a collective to be inclusive in the school system (see Miller & Katz, 2002)[^1].

> “Inclusive education is meaningful only when embedded in understandings about 
> community and communality, only when seen as both reflective of, and creative of
> inclusion in society”
>
> --Thomas (2013)[^2]. 

With this quote in mind, underpinning this OER is a broad understanding of inclusive education including changes and modifications in structures, approaches, strategies, teaching methods and content. The intention is that social systems involved near (such as schools and families) or far (such as school principals, university teachers, politicians) in school education, overcome barriers and discrimination with a vision serving to provide all students with equitable and participatory education (cf. also Köpfer et al., 2021)[^2].

> __Learning Goals__
> 
> * You are able to specify what inclusive education means.
> * You are able to explain how inclusive education could be implemented in schools on different levels (i.e., educational system, single school, lesson).


[^1]: Frederick, A., & Katz, J. H. (2002). The Inclusion Breakthrough: Unleashing the Real Power of Diversity Miller. Berrett-Koehler Punlishers, Inc.

[^2]: Thomas, G. (2013). A review of thinking and research about inclusive education policy, with suggestions for a new kind of inclusive thinking. British Educational Research Journal, 39(3), 473–490, p.485. https://doi.org/10.1080/01411926.2011.652070

[^3]: Köpfer, A., Powell, J. J. W., & Zahnd, R. (2021). Handbuch Inklusion international / International Handbook of Inclusive Education (A. Köpfer, J. J. W. Powell, & R. Zahnd, Eds.). Verlag Barbara Budrich. https://library.oapen.org/handle/20.500.12657/46311



### 4.1 Inclusive Education – a Broad Term with a Common Sense


> "An important element of inclusive education involves ensuring that all teachers are prepared to teach all students. Inclusion cannot be realized unless teachers are empowered agents of change, with vlues, knowledge and attitudes that permit every student to succeed. Despite their differences in teacher standards and qualifications, education systems are increasingly moving away from identifying problems with learners and towards identifying barriers to learning. To complete this shift, education systems must design teacher education and professional learning opportunities that dispel entrenched views that some students are deficient, unable to learn or incapable." 
>
> -- UNESCO (2020)[^1] 

Core values and competence areas of inclusive teaching
---


<center>![Core Values and Competence Areas of Inclusive Teaching](5f47ce12bd53b47705bf96714a1a99404cdc8ffe.png)Core Values and Competence Areas of Inclusive Teaching, UNESCO (2020)[^1]</center>

------
<details>

<summary>~~**Click here to show the "core values and competence areas of inclusive teaching" text table**~~</summary>

<!-- data-type="none" -->
| Core values and competence areas of inclusive teaching | Core values competence areas                                                                                          | Core values competence areas                                                                                                                          ||
| ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| __Support All Learners__                               | Promote academic, practical, social, and emotional learning for all                                                    | Engage effective teaching approaches in heterogenous classes based on understanding a variety of learning processes and how to support them |
| __Work With Others__                                       | Work with parents and families to engage them effectively in students' learning                                                 | Work with other education professionals, including collaboration with other teachers                                                                  |
| __Value Learner Diversity__                                | Understand inclusive education (e.g. its foundations in equality, human rights, diversity, and democracy for all) | Respect and value learner diversity and view it as an asset asset                                                                                                 |
| __Engage in Professional Development__                     | Be a reflective practitioner (i.e. systematically evaluate one's own performance)                                      | View initial teacher education as the foundation for ongoing professional learning                                                                    |

(UNESCO, 2020)[^1]

</details>

---

The values, core competences, values, and professional standards listed here reflect current developments and recommendations for action in the area of inclusion and diversity.

In the next section
----

In the following, we focus on the Response-to-intervention approach as a way of targeted prevention that is implemented in successful educational nations. 

[^1]: UNESCO Global Education Monitoring Report Team, International Task Force on Teachers for Education. (2020). Inclusive teaching: preparing all teachers to teach all students. https://unesdoc.unesco.org/ark:/48223/pf0000374447 


### 4.2 Response-To-Intervention Approach

Based on the question of how successful educational nations deal with pupils who do not reach the minimum standards in maths or language, _“Response to Intervention_ (RTI) is a highly effective approach to supporting at-risk pupils and getting positive learning outcomes" (Hattie, 2018)[^1].

> The main objective of RTI is not to identify students for special education but rather to help all students achieve at a proficient level and ultimately make adequate yearly progress. 

That means, it is not about categorising children as “need special support” and “no need of special support”, but about knowing exactly who is “not yet able” or successful enough in achieving competences, but can achieve with targeted support and encouragement. Therefore, ongoing diagnostics is necessary (Osberg, 2010)[^2].

The RTI approach is often visualised as a pyramid and a model of three levels or tiers. 

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/rti-model.png "RTI Model. Pretti-Frontczak et al., 2014, p. 110[^4]")

* __Tier 1__

   The lowest level __(tier 1)__, which benefits all learners, is regular teaching and responding adaptively to different learning requirements. But some learners need more. 

* __Tier 2__

   Children whose diagnostics indicate competences that they have not yet achieved receive a _focussed intervention_ as short-term, curriculum-based intensive small group and/or individual interventions at the next higher level __(tier 2)__, in order to catch up with the class. In many schools, this affects between 15 and 20 per cent of all pupils; depending on the context of the school, the proportion can be even higher. 

* __Tier 3__

   The third stage __(tier 3)__ means _“special intervention”_, it is used for learners for whom the focussed intervention has not yet been sufficient. It is designed for the longer term, is individualised and is based on in-depth diagnostics. This often affects around five per cent of learners, for whom responsible and professional pedagogical action can be guaranteed through this form of intervention (University of Rostock 2024)[^3].

Ongoing individual diagnostic in inclusive classes, individual support for both high-achieving and low-achieving students





Video: RTI Model explained
-------
Let's view the following video to find out more details about the approach.

!?[](https://www.youtube.com/watch?v=nkK1bT8ls0M&t "Source: https://www.youtube.com/watch?v=nkK1bT8ls0M")

<details>

<summary>__Click here to show the video transcript__</summary>

Here we'll look at a three- tiered model often depicted as a triangle as one example of how a tiered framework can be used as a schoolwide strategy. For instructing all students all students will participate in tier one instruction at this level they'll receive effective differentiated instruction provided by the general classroom teacher as part of an evidence-based Core Curriculum. 

The evidence-based instruction offered at this level can be expected to meet the learning needs of 80 to 85% of all students for students who don't respond adequately to Tier 1 instruction. More intensive interventions come into play tier 2 interventions build upon the differentiated instruction provided at tier one by offering students more systematic instruction and intervention strategically designed to help them catch up in areas of difficulty.

These interventions are usually delivered to a small group of students within the general classroom either by the classroom teacher or by another team member supporting the teacher who has also been trained to deliver the interventions tier 2 intervention will be offered to the 15% of students for whom Tier 1 instruction was not sufficiently intensive to meet their specific learning needs. 

But here is a critical point students who receive targeted tier 2 interventions continue to participate in general tier one instruction. Tier two interventions do not replace the Core Curriculum they supplement it for example Dennis has been selected to receive tier 2 interventions. 

Based on the results of recent reading fluency data he'll continue to participate in the 90 minutes of core reading instruction that is provided to all students in tier one each day but in addition he'll spend another 30 minutes per day receiving targeted reading instruction at tier 2. 

Under RTI his opportunities for learning and for catching up to his classmates will have been extended we've saved the most intensive interventions available for the small percentage of students who still lag significantly behind their peers in making academic gains. 

Tier three interventions supplement the previous tiers by providing the most intensive evidence-based interventions to delivered to individual students or in very small groups. 

Again the intensity of instruction at this level increases the size of student groups is reduced and their opportunities for direct instruction extended interventions. 

In tier three may be delivered by an intervention specialist or even a special education teacher but again these interventions supplement the instruction provided at tier one not replace it and students do not have to be identified as disabled in order to receive these interventions. 

Only about 5% of all students will require these intensive tier 3 interventions of these students only a portion may go on to require special ed services

</details>

<br>

When looking at this approach, it quickly becomes clear that educational policies and structures as well as competences of the school principals as mangers are crucial. RTI needs cooperation between educational actors (school principals, teachers, other professions, also parents) and in fact, this is a key prerequisite for quality education and professionalisation. 

In the next section
-----
In the following, we will look at different types of cooperation.


[^1]: Waack, S. (n.d.). Hattie effect size list - 256 Influences Related To Achievement. VISIBLE LEARNING. Retrieved October 7, 2024, from https://visible-learning.org/hattie-ranking-influences-effect-sizes-learning-achievement/

[^2]: Riccomini, P., & Witzel, B. (2010). Response to Intervention in Math. Corwin Press. https://doi.org/10.4135/9781452219356

[^3]: Universität Rostock. (n.d.). The Response-to-Intervention Approach. Universität Rostock. Retrieved October 7, 2024, from https://www.rim.uni-rostock.de/en/response-to-intervention-approach/the-response-to-intervention-approach/


### 4.3 Cooperation und Multiprofessionalty

Types of Cooperation
------

Based on Lütje-Klose et al.(2024)[^1] a distinction can be made between:

*	_Multiprofessional cooperation_ (i.e. between different professional groups, e.g. involving teachers, special needs teachers and school social workers in multi-perspective and case-related counselling, diagnostics and support planning),

*	_Intraprofessional cooperation_ (i.e. within a professional group, e.g. between subject teachers) and

*	_Interprofessional cooperation_ (i.e. between two professional groups, e.g. classroom teachers and special needs teachers, who work together in a class in relation to teaching).

All types of cooperation require a partnership relationship in which __goals, knowledge, resources, tasks and responsibilities__ are consciously shared. Such a relationship requires the development of trust and respect. Furthermore, team development requires time and commitment (Friend & Cook, 2010)[^2].



Multi-professional teams
-----

Looking on international research, it is undisputed that _multiprofessional teams_ and successful cooperation between the different educational actors are particularly crucial for inclusive education and the individual support of a diverse student body (Köpfer et al., 2021)[^3]. 

The following illustration includes main features and conditions of successful multiprofessional teams.:

<center>![](https://euniwell.de.cool/wp-content/uploads/liascript/images/multiprof-teams-crop.png "Own illustration based on Widmer-Wolf (2018)[^4]")</center>

When establishing different kinds of cooperation, general schools can adopt changes in overall structure so that inclusion becomes a part of the school’s culture. The role of school leaders is crucial; they are a kind of managers in the schools but also responsible for social networking. 

Intraprofessional cooperation could be seen as a lower challenge because the actors have the same professional background, they have an idea of each other’s expertise and could change perspectives easier. Interprofessional cooperation is a main structure for inclusive lessons in general schools.


A model teachers` perspectives on co-teaching
----

Let’s have a look at what teachers need to be successful in inclusive classrooms. The following illustration is a model of teachers’ perspectives on the conditions for successful co-teaching by Jurkowski, S., Ulrich, M., & Müller, B. (2023)[^5]. 

<center>![](https://euniwell.de.cool/wp-content/uploads/liascript/images/jurkowski.jpg "3 Levels of co-teaching, Jurkowski, S., Ulrich, M., & Müller, B. (2023)[^5] ")</center>

The categories describe the conditions for successful co-teaching in inclusive classes on the levels of the educational system, the single school, and the teaching dyad.

<details>

<summary> __Level 1 - Educational System__ (click to view)</summary>

<br>

We identified two categories at the level of the educational system: __“teacher education”__ and __“inclusive school system”__.

The category __"teacher education"__ included aspects of professionalisation in the ﬁeld of inclusive education (i.e. study curricula, pre-service and in-service teacher training). The special education teachers interviewed stated their lack of didactical knowledge that they would need for teaching large groups. In contrast, the general teachers reported the need for knowledge about their students’ special needs to provide suﬃcient assistance to those students when the special education teacher is not in the class.

The category __"inclusive school system"__ reﬂected the teachers’ ideas about the implementation of inclusion and the educational opportunities for children with special needs. It became clear that the teachers have the wish for the development of a full-inclusive school system. However, some  were not convinced that the high-achiever would benefit.

</details>

<br>

<details>

<summary> __Level 2 - Single School__ (click to view)</summary>

<br>

The three main categories on this level concern structural and organisational conditions as well as attitudes towards co-teaching and co-teachers’ collaboration in inclusive classes: "organisation of inclusive teaching" (time for teaching dyads, equipment, and teaching concepts), "multi-professional cooperation" (cooperation within a school, with external professionals, and with parents and families), and "principals’ administration" (principals’ responsibility to provide co-teachers with guidelines as well as their attitudes towards inclusive schooling).

</details>

<br>

<details>

<summary> __Level 3 - Teaching dyad/co-teachers__ (click to view)</summary>

<br>

The level of the co-teacher contains six categories regarding to a social-emotional as well as role-related aspects: "relationship" (e.g., sympathy), "task assignment" (e.g., professional role-taking), "forms of collaboration" (e.g., shared reflecion on a lesson and constructive planning), individual "beneﬁts from co-teaching" (Entlastung, berufliches Lernen); "self-organisation" (Zeitfenster für Absprachen), and "inclusive learning arrangements" (je nach Klasse anpassen).

</details>

<br>



Overall, this chapter has shown which adjustments the school system - whether at the political-educational system level, the school management level or the teaching level - must be capable of acting on in order to organise inclusive education. 

In view of the legal situation, it should not be a question of whether inclusion is possible in the school context; instead, all educational stakeholders must act cooperatively in their various roles, set out on a journey and pursue common goals. Ultimately, development takes time and positive experiences!

In the next section
---

In the following chapter, we will move away from the professional level of action and look at the _diversity characteristics_ of the pupils that teachers may be confronted with in their classes.


---
[^1]: Lütje-Klose, Birgit, Wild, E., Grüter, S., Gorges, J., Neumann, P., Papenberg, A., & Goldan, J. (2024). Kooperation in inklusiven Schulen. Pädagogik (Weinheim). https://doi.org/10.14361/9783839460689

[^2]: Friend, M., Cook, L., Hurley-Chamberlain, D., & Shamberger, C. (2010). Co-teaching: An illustration of the complexity of collaboration in special education. Journal of Educational and Psychological Consultation: The Official Journal of the Association for Educational and Psychological Consultants, 20(1), 9–27. https://doi.org/10.1080/10474410903535380

[^3]: Köpfer, A., Powell, J. J. W., & Zahnd, R. (2021). Handbuch Inklusion international / International Handbook of Inclusive Education (A. Köpfer, J. J. W. Powell, & R. Zahnd, Eds.). Verlag Barbara Budrich. https://library.oapen.org/handle/20.500.12657/46311 

[^4]: Widmer-Wolf P. (2018). Kooperation in multiprofessionellen Teams an inklusiven Schulen. in T.Sturm & M.Wagner-Willi (Hrsg.), Handbuch schulische Inklusion (Kap 3.5). UTB. - https://doi.org/10.36198/9783838549590

[^5]: Jurkowski, S., Ulrich, M., & Müller, B. (2023). Co-teaching as a resource for inclusive classes: teachers’ perspectives on conditions for successful collaboration. International Journal of Inclusive Education, 27(1), 54–71. https://doi.org/10.1080/13603116.2020.1821449

### 4.4 Co-teaching

The most important aspects of establishing a _co-teaching_ relationship are outlined below. The differentiation of six established forms takes place under the point of the distribution of roles and responsibilities. Finally, we look at a video in which teachers share their experiences.

<center>![](https://euniwell.de.cool/wp-content/uploads/liascript/images/co-teaching-factors.png "Crucial factors for Co-teaching, own illustration")</center>


Three Steps for Developing Co-teaching
---

1. __Getting to know each other (similarities and differences)__

An important first step in the development of co-teaching is for the co-teaching partners to get to know each other, to discuss goals, interests, teaching and working styles and preferences for giving and receiving feedback. 

Spending hours together every day and sharing all aspects of teaching can be fun, but it can also lead to frustration and conflict. 

2. __Sharing roles and responsibilities__

The aim is to plan, implement and evaluate the lesson together and to share responsibilities. Different strengths of the co-teachers can come into play in the planning and design of lessons, but both should play an equal part in all aspects of the lesson. In well-functioning co-teaching classes, it is often impossible to tell at first glance who is a special needs teacher and who is a mainstream teacher because both are equally committed and have an equal say.

__Six Forms of Co-teaching__

In practice dividing up roles and responsibilities between two teachers can be achieved in either one of the following six forms or a mixture of them.

| Co-teaching Form                                                                       | Description                                                                                                                                                                                                                  | Use Case                                                                                                                                                        |
|:-------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| __Teacher & observer__ ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/teacher-observer.png) -   | One teacher leads a large-group instruction while the other gathers academic, behavioral, or social data on specific students or the class group.                                                                         | For detailed recording of the learning process, i.e. learning behavior/progress of individual pupils.                                                           |
| __Teacher & assistant__ ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/teacher-assistant.png)  | One teacher leads instruction while the other circulates among the students offering individual assistance.                                                                                                                  | If a teacher has special expertise for the teaching unit and for teaching units that require particular progress and intensive monitoring of the learning process. |
| __Team-teaching__ ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/team-teaching.png)        | Both teachers lead large-group instruction by both lecturing, representing opposing views in a debate, illustrating two ways to solve a problem, and so on.                                                                 | With team teaching, students experience open and differentiated lessons in which teachers and students work together.                                            |

| Co-teaching Form                                                                       | Description                                                                                                                                                                                                                  | Use Case                                                                                                                                                        |
|:-------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| __Parallel teaching__ ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/parallel-teaching.png)    | Two teachers, each with half the classgroup, present the same material for the primary purpose of fostering instructional differentiation and increasing student participation.                                             | To be able to better support pupils in the learning process by reducing the pupil-teacher ratio and to promote the participation of pupils.                        |
| __Station teaching__  ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/station-teaching.png)    | Instruction is divided into three nonsequential parts and students, likewise divided into three groups, rotate from station to station, being taught by the teachers at two stations and working independently at the third. | When learning content is complex but not hierarchical and to provide an overview of topics.                                                                        |
| __Alternative teaching__ ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/alternative-teaching.png) | One teacher works with most students while the other works with a small group for remediation, enrichment, assessment, pre teaching, or another purpose.                                                                     | If the level of achievement in the subject is very different and if some pupils have a parallel curriculum.                                                                                                    |
          |

^Table 1. is based on Friend, M., Cook, L., Hurley-Chamberlain, D., & Shamberger, C. (2010)[^1] and Studienseminar Hannover für das Lehramt für Sonderpädagogik: Handreichungen zur Ausbildung im gemeinsamen Unterricht. Own translation.[^2]^

__Video Playlist: Six forms of Co-teaching__

<iframe style="width: 100%; aspect-ratio: 16 / 9; margin-top: 10px " src="https://www.youtube.com/embed/videoseries?si=_pLFHznqfxMOQz3O&amp;list=PLCDsTyftAA2D_buI_Rti5phLZ1DdFsAMc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Regardless of which model of collaboration co-teachers implement, they are required to engage in an intensive examination of how both experts want to share their responsibility for planning, implementing and evaluating lessons. If both experts give each other appropriate freedom of action in these aspects, their competencies are not only used, but also expanded over time and can therefore be used more flexibly.

3. __Develop a shared classroom in detail__

Once co-teachers have laid the foundations for good collaboration and agreed on how to share their roles, it is important to think about the detailed issues of their collaboration. 

This includes understanding how to design and use the shared classroom and how to deal with class rules and consequences. 

__Questions that should be discussed in this context are:__

<details>

<summary> __How do we introduce co-teachers to pupils and parents?__</summary>

<br>

* From the first day of school letter, information evening, etc.

* Names of both teachers on the classroom door and on documents 

</details>

<br>

<details>

<summary>__Do we have equal access to resources?__</summary>

<br>

* Discussions about room/material design and allocation may seem minor at first, but they are crucial to ensure that both teachers have equal access. There are teachers who are very reluctant to share their materials - open communication is therefore important.

* It is helpful to work with the school management to ensure that there are enough materials and furniture in the classroom for both teachers.

</details>

<br>

<details>

<summary> __How will we share responsibilities?__</summary>

<br>

* It is important to share communication with families. This includes deliberately not dividing students into "my" and "your" students, but seeing all students and their families as "ours". Co-teachers must therefore agree how and with what frequency they frequency they wish to contact parents, who will inform parents about various events/appointments and how they will share messages from parents.

* Co-teachers need to agree what type of assessment of student performance they will use and at what time frame and interval. It is essential that both teachers have an equal say in the assessment of student work, project contributions and tests. 

* Co-teachers need to agree on class rules and rituals in advance, for example, rituals at the beginning and end of the day, when students want to use the bathroom or change classrooms; their tolerance limits when dealing with noise or rule violations; and agreements on deadlines regarding the communication and submission of homework.

</details>

<br>

<details>

<summary> __How do we share information?__</summary>

<br>

* It is important that co-teachers choose an effective communication system to share information, discuss upcoming deadlines, and plan lessons. 

* While some co-teachers meet immediately after class, other co-teachers prefer to email or call each other later. It is also helpful if co-teachers agree on a place where they both have access to messages from parents and collected materials.

</details>

<br>

On the one hand, it is crucial that co-teachers take enough time to discuss and answer these questions and, on the other hand, that any disagreements that do arise are not resolved in front of the students, but in private.

Only when co-teachers have taken the time to lay the foundations for co-teaching does it make sense for them to face up to the actual planning and implementation of joint lessons.



[^1]: Friend, M., Cook, L., Hurley-Chamberlain, D., & Shamberger, C. (2010). Co-teaching: An illustration of the complexity of collaboration in special education. Journal of Educational and Psychological Consultation: The Official Journal of the Association for Educational and Psychological Consultants, 20(1), 9–27. https://doi.org/10.1080/10474410903535380

[^2]: Studienseminar Hannover für das Lehramt für Sonderpädagogik. (n.d.). Handreichungen zur Ausbildung im gemeinsamen Unterricht. https://lehrerfortbildung-bw.de/s_sueb/alle/fb1/6_mat/3_zusammen/11_lit/Handreichungen-zur-Ausbildung-im-gemeinsamen-Unterrich.pdf 



### 4.5 Tipps for Planning Co-Teaching in the Classroom.

> __Your task:__
> 
> 1. Starting at 4 Min. watch the "Special Education and Regular Eduaction: Working Together" video interview with Christie Eleeson and LeeAnna Rabine. 
> 2. From their point of view, what are the outcomes and benefits for students and teachers?
> 3. Answer the question by using the "drag and drop" interaction below. 

Video: Special Education and Regular Education: Working Together
---

!?[](https://www.youtube.com/watch?v=jlc1ZU-P8jc "Source: https://www.youtube.com/watch?v=jlc1ZU-P8jc&")


<details>

<summary>__Click here to show the video transcript__</summary>

Co-teaching, at least at Hawthorne and I think elsewhere, is when we have all of our specialists come in
and we keep all of our kids inside the classroom. And we get the opportunity to work as a team within the classroom so that all the kids are staying inside our classroom. So we have LIA teachers that come into our rooms. We also have ELL teachers, and then we also have our SPED teachers that all come into our classroom during their times and work with our students. I find it very beneficial, having all of the specialists come into my classroom. One of the biggest benefits I find, is that we are all on the same page. And so at any point, during our collaboration, they come to our collaborations. They also look at, we write up a sheet every week that we share on the Google Docs and they're able to read through it and look at what we're teaching if they're not able to come to collaboration. But they try to come and then when we come into the room, we're able to work together, to hopefully help these students find success. And what we do and what I love is its, for me decreased a lot of the behaviors. Because those transitions are sometimes the hardest part for students. And when you take away those transitions, you have the opportunity for learning to increase and for the behaviors and the management to decrease. And so it's been really helpful because then we have more eyes onthe whole group.

* __Tanya:__ With pushing,we have anywhere between five to seven students in the classroom and they're all served under a reading or writing disability on an IEP. And I work with the teacher to help make sure their accommodations are in place, to help them out in the classroom and to also kind of troubleshoot, any issues the teacher may run into. And I'm just right there for them to talk to or to email quickly. And then I also work with emailing all of the case managers of those students, to let them know what they did that day, what they maybe missed if they got it done If they didn't. To kind of help those students stay caught upin those regular English classes. In there I don't treat them any differently and I help out all the students that are in there. Because I wanna make sure, that our students are not singled out. Because they already know they have a disability and they don't necessarily like if people know it as well. So that's kinda my goal is to help everybody out when they're, working on something to help all students out. And the teachers see that as well. They tell all the other teachers as well. Mrs. Bjerke is in here to help everybody. You can ask her, you can ask me if you have questions.

* __Aj__: Two teachers working together to meet the needs of students that struggle in math. It takes two adults so they can reach more students. And then were sharing the load of the teaching and great level material. The core math teacher kinda holds the, kinda more of the knowledge of that subject. So she teaches more of it. But as the class goes, I pop in ask questions, kinda think in terms and then go around and helping my students. And we both work together to adapt it or come up with ways to reach our students easier. It helps more students be able to get great level material presented at their level. So then we only have to do as many pull-outs where kinda the research classes. I mean they widen the gap for the learning where this allows them to be in getting great level materials presented at their level. The alternative to this yeah there's is pull out, which I also teach to those classes. The only alternative if we didn't have co-teaching, would be that we would have to pull out and try to modify the the curriculum at their level where this is more presented at theirs. They want their peers they don't feel like they're excluded.

* __Christi__: I have a better understanding of the materials just 'cause I've been doing this for four years. I actually started at Whittier as a co-teacher in the special ed department, and fell in love with the curriculum so I moved to math. And so I think it's good that I have the special ed background and it helps me in the co-taught classroom. But together we plan, we talk about things that we wanna do. We have bright ideas that don't always come to fruition. As a classroom teacher, I have to have knowledge of the special ed students. What their accommodations are and what I need to do. But it's always nice to have that second person in the classroom to come up with different strategies or maybe they suggest trying it a different way. Or when he questions the students, asking them a question in a different way than what I would've thought about asking it. Bouncing ideas off of them using them together, which is something that I don't know if it'll work talking it through with him. Sometimes he thinks I'm crazy, sometimes it works, sometimes it doesn't work. So it's nice to have that second third person 'cause there's a lot of movement in the morning with different math teachers and talking about what we're doing that day and why we're doing it and how we're doing it. And so it's nice to have somebody who knows our students and to bounce ideas off of them.

* __LeeAnna__: Another benefit that I have found, that we've done is flexible grouping. So that flexible grouping allows us to take kids that yes, they might be on an IEP, they might not be on an IEP, but they might need that additional support and we can put them together. And so there's some days that, I might have one of my specialists come in and they might not be working with a specific child that they're supposed to be working with. Based on the fact that, we know how many hours each of our students need for the required amount. And we can work together to fulfill those hours. So it's been pretty cool because then we have that opportunity together to work with the kids. And so if I'm not able to get a kiddo to be able to, if they're struggling with their reading and I'm not able to do something to help motivate them, one of my coworkers might be able to do that.  And one of my specialists and vice versa sometimes we'll look at each other and then say you know, Oh, we're really struggling here. I'm not sure what we need to do next. I can just go right over there and say, let's try this and they can do the same for me. So it's been really helpful for us to be able to build that comradery. And then those kids, don't even know that there's any difference between one from the other. And so they just, it's another day. All the people come in, all the people go out and they know that more than likely they're gonna be working in one of those groups. Mostly for our kiddos who come in, who are on an IEP, they have that label. That label can be very scary to parents. The older they get, the kids realize they have a label. But when, we have the co-teaching occurring, I don't even know if, the majority of my kids who are, are qualifying for SPED even knowing that they are. And that's the powerful piece for me because it's rebuilt relationships, confidence. It's shown them that they are a part of us, they're not any different. And I've been here for 12 years. And so seeing that growth over time and how we've changed and it's been a positive switch for me. It had to require some growth mindset on my part as well knowing that there's gonna be people in here as I'm teaching, I better be organized, I better have myself ready to go. And they might be a little louder than I typically would expect at a certain time. But the loudness is not them being off task, rather It's more on task. So that's been helpful for me too because then I can say, yes I hear them, but at the same time they're on task. They're doing what they need to be doing. They're answering questions, they're recalling whatever we're doing whether it's reading or writing or math. And so that's been really fun for us to see as well.  We have seen an increase in students passing rates in these classes where they struggled before. Because regular education teachers have, almost 100 students probably in a day that they see. And our students are a very small percentage of that. And so by, being able to have a teacher in there, who's monitoring those students, we can catch them and keep them caught up before they fall so far behind, that it's just impossible to get them caught up. It also gives them some confidence and also helps give them some skills. Like for me as the Freshmen English teacher, to kind of get those freshmen on the right path for the rest of high school in order to make sure they start off on a good foot. Some students have to be pulled to be read to. And so, they kind of I will talk to them privately like, Hey, we have a test coming up. After your teacher gives you your test, come with me, just leave the room like to make no big deal of it. They also, kind of know I'm the one to go to if they're stuck with something and they're not really sure. So that piece is nice as well as having that additional person who knows what they're doing and that works in study hall too. Like all of our students have the same study hall times roughly between fourth and fifth period and so, if their teacher has no idea what they did they can send them to us or to me, and then I can help them out. Or the teacher will come ask me what they're doing but, students, they kind of they know that I know but then they don't have to say anything about it either. Like they're struggling so I can kind of help them advocate for their needs too.

* __Aj__: They're with their peers, they're not being pulled out.They're not, again, back in the day where they're always excluded. And so getting the label of learning disability you're excluded from all your peers. While here they just feel like they're with everyone else. Most of the people in here, I would say half the students in here don't even know I'm a special ed teacher. They just think I'm another teacher in the room. That's the other perk is they're learning from the students that math is easier for them. So then the different mindset, the problem solving kinda hearing from them instead of just hearing from the same group of kids that are all just struggling in math. They do learn strategies from their peers. 'Cause the special ed kids bring a different mindset also. So they might not, math might not come easy, but they come up with a different way of thinking of stuff. So it also makes the ones who really get it easy to kinda slow down and rethink and then they can also teach. So, the best way that we know as teachers if a student can teach it, they really have a material down. So we do allow our students that excel to kinda step back sometimes and help the other students and kind of a win-win for both.

* __Christi__: With the collaboration it is nice for the lower level students to be able to speak to somebody middle ranger or higher, and bounce ideas off. But I also think that the higher level thinkers they benefit from the lower students just because, they bring in a different idea. So I think they feel more comfortable with each other and they're able to talk to each other. At the school I was at, I had to push in and it was my first year of teaching. I didn't know the math curriculum very well. And I was hoping that they would help out more and kind of lead me a little bit or share some of their knowledge. And I think from that experience it led me to, wanna co-teach and be part of it just because two brains are better than one.

* __Tanya__: For the regular ed students, some of them need that additional support. And sometimes I can pick out the regular students that they might wanna consider some additional supports for additional services as well. And they can ask for, they can ask me for my input too the regular teachers can as well. I like seeing how different teachers teach. Like that's what a benefit I've gotten out of Whittier. Oh that's really cool, I wanna try that because we don't get to go out and see other teachers, how they teach and just sit and watch them sometimes. And it's just, it's built some good relationships between the departments that we've worked with, with this. Because they, sometimes have a different perspective on special ed. And then once you're able to kinda see how we work and see what it looks like, it kind of helps them understand, how that department works and how we are there to help them as teachers and help their students settle in their classroom as well.

* __Aj__: As a special ed teacher, you're coming in and not knowing the material as well as a co-teacher 'cause they've taught it for years or that's all they have. It's depending on how comfortable I am with the material, I jump in more, I teach or most of the time I kinda sit back and kinda think about questions that I can ask to kinda help in particular my students are not even if they're special or just kind of struggling students what kind of questions should they be asking, that they probably don't feel comfortable asking themselves. And I'll raise my hand and ask those questions. They're kind of my main role, and going around and kinda observing what they're doing with their work and kinda seeing if they need help and trying to be in their voice.

* __LeeAnna__: I think the advice that I can give, when it comes to co-teaching is just to have that growth mindset and to give it a try. It's scary and a little overwhelming at first. There's still a little hesitation with some here but we've come a long way in the time that I've been here. But once you get there, you don't wanna ever lose it. And so even when we have all of our supports with our reading teachers coming in and our ELL and our SPED it's just nice because anytime we see each other in the hall, we're able to say, "hey, this is what I worked on, this is what I saw with the gains". And we've seen student achievement rise with all of these kids in growth. And our main focus is always growth. And to be able to have that language and that conversation with a variety of teachers, and we're all seeing the same thing. it's been really powerful for us when we see our scores slowly rising. And it's not all about test scores but it is nice to have that visual to say, this is working. So that when we're going this is a little extra work, we have to make sure we're making time with other people. But at the same time we have that benefit of knowing all the great things that are coming out of it. And these students are feeling like they belong and they love being in their natural setting, their classroom. And for them to know they're not gonna leave and they don't have to leave. And they see a variety of students rotating between the groups. They don't know any different. They think that's just a part of how teaching works. And so it's been really cool to see that it happened here.

</details>

<br>

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=39" width="958" height="687" frameborder="0" allowfullscreen="allowfullscreen" title="Benefits of Co-Teaching in the Classroom - Drag Drop"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


###	4.6 Summary Quiz



<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=34" width="958" height="1107" frameborder="0" allowfullscreen="allowfullscreen" title="Co-Teaching Forms and Applications (Drag &amp; Drop)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>



## 5. Examples of Students´ Diversity in Inclusive Classrooms

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/children-diversity.png)

In chapter 2, we defined the fact of diversity including the variety and difference of individuals in a society on three levels: social, biological, psychological. 

According to this theoretical frame and interdisciplinary empirical research, we take a closer look at three _dimensions of diversity_ and special characteristics of students: 

* (5.1) social and ethnic origin 
* (5.2) physical and cognitive abilities 
* (5.3) personality and gender 

Each chapter ends with a case-vignette. 

Moreover, in chapter (5.4), we put together a guideline "Reducing _Bias_ in Communication" that helps you as an educator being a sensitive teacher, colleague, and partner in cooperation. 

Let’s start with the last main chapter and focusing on the individual level of students. With regard to the diversity discourse, we deliberately refrain from making a rough distinction between general students and students with special education needs or at-risk-students wherever possible!

> __Learning goals:__
>
> * You are able to describe the characteristics of student diversity in different dimensions.
> * You are able to judge situations of discrimination in school/lessons, analyse the situation from the students’ point of view and indicate a course of action appropriate to the situation and to justify this.


###	5.1 Socioeconomical Inequality

Similar to the social level of diversity, sociologists focus on features of social origin examining causes, mechanism, and consequences of discrimination (see chapter 2.3) and social inequality. 

Inequality is social insofar as it arises through social processes. However, the challenge again lies in a value-free definition; e.g. the definition: "Social inequality exists when people have different levels of _well-being_" (Brüderl, 2019)[^1]. 

Here, defining well-being also is difficult. Because of that the following definition is preferred:

> __Definition: _Social inequality___
>
> Social inequality exists when people have different levels of primary and/or secondary intermediate goods. (Intermediate
> goods are the dimensions of social inequality such as education and financial capital.” (translated from Brüderl, 2019)[^1]

Whether inequality is just or unjust is another question, which we will not discuss here. 

For a common definition of social justice and a further description according to concepts, theory, and praxis see Abbott (2014).[^2]

> __Definition: _Social justice___
>
> Social justice is commonly viewed as a guiding principle to achieve a just society, understood both as a means as well as
> an end. It includes a wide variety of goals, including full and equal participation of individuals in all institutions; 
> fair, equitable distribution of material and nonmaterial goods; and recognition and support for the needs and rights of
> individuals. (cf. Abbott, 2014; see also Bell, 2007)[^2][^3]

In general, sociological researchers differ in terms of _ascriptive features_ such as origin, sex/gender, ethnicity, blood group, hair colour, age, etc. and acquired features such as occupation, education, income and wealth. It is assumed that ascriptive features do not influence human wellbeing directly, but indirectly via primary and secondary intermediate goods.

In the next chapter, you can see some interrelation between well-being and exemplary, primary and secondary primal goods.

Increasing Well-being
===

In principle, it is assumed that more or better intermediate goods increase individual well-being (see illustration according to Brüderl, 2019)[^4].

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/well-being-crop.png "Increasing well-being, own illustration based on Brüderl, J. (2019)[^4]")

This illustration does not claim to be complete. Where do you see migration/ethnicity and sex/gender?

Again and again, international comparative research showed that these aspects are crucial with regard to social and educational inequalities in current societies (OECD, 2024)[^5].

[^1]: Brüderl, J. (2019). Vorlesung Sozialstrukturanalyse. https://www.ls3.soziologie.uni-muenchen.de/studium-lehre/lehrmaterialien/ws-2019-2020/vorlesung-sozialstruktur_19.pdf

[^2]:Abbott, K. (2014). Social Justice. In A.C. Michalos (Ed.), Encyclopedia of Quality of Life and Well-Being Research. Springer. https://doi.org/10.1007/978-94-007-0753-5_2772

[^3]:Bell, L. A. (2007). Theoretical foundations for social justice education. In M. Adams (Ed.), Teaching for diversity and social justice (pp. 1–14). Routledge/Taylor & Francis Group.

[^4]:Brüderl, J. (2019). Soziale Ungleichheit. Vorlesung Sozialstrukturanalyse (Kapitel 4), LMU München, Germany. https://www.ls3.soziologie.uni-muenchen.de/studium-lehre/lehrmaterialien/ws-2019-2020/vorlesung-sozialstruktur_19.pdf 

[^5]:OECD. (2024). Education at a glance 2024: OECD indicators. OECD. https://doi.org/10.1787/c00cad36-en


### 5.2 Case-vignette "Social Origin"

Please, take your time and keep in your mind: This is an exercise to think about your role-taking as a teacher in diverse classroom settings; it is not a test for choosing right or wrong answers!

<center>![](https://euniwell.de.cool/wp-content/uploads/liascript/images/1-tina.jpg "AI Image Gen generated image based on own prompt[^1]")</center>

> __"Social origin" case description__
> 
> Tina, 14 years old, is a student in 8th grade at the city high school who lives with her parents and three younger 
> brothers out of town. Since her mother has fallen seriously ill and her father has to look after the cheese 
> dairy and the inn on his own, the family's finances have become increasingly difficult. Tina therefore helps out in the service 
> area of the restaurant after school and only does her homework late in the evening. She can barely keep her eyes open in class 
> and during the breaks she sits away from her friends to rest.
> 
> As a teacher, you have no idea how much of a burden Tina is. She was always rather quiet in class and her performance was in the 
> middle range. However, when it comes to the class trip, she doesn't seem to be looking forward to it at all. You are worried - 
> and rightly so, because Tina then comes to you with the news that she doesn't want to go on the picnic next week or on the school 
> trip. She had a fight with her best friend - an answer that makes you think. The two friends sit next to each other in class.

Here, you can see some possible reactions. 
---

Please, think about your preferred action as the teacher. Also, reflect why you would do this as a first reaction? You can also note other ideas on a separate note (sharing with us on the [feedback wall](https://padlet.com/teacheredueuniwell/oerdiversityinclusion) in the section "content" after finishing this OER).

- Seek contact with the parents
- Accept Tina's decision without asking further questions
- Motivate Tina to participate
- Ask Tina and her friend to talk
- Seek dialogue within the teaching staff
- other ideas?

[^1]: Photorealistic image of a tired 14-year-old girl in 8th grade, sitting at her desk in a bright classroom, looking worried, with droopy eyes, while classmates chat nearby. A calendar shows an upcoming class trip.

### 5.3 Ethic and Migration

Ethnic origin, which is systematically linked to various dimensions of inequality, can be operationalised in very different ways (e.g., via the place of birth in the country of origin or in the destination country). This operationalisation is particularly central in traditional immigration countries such as the USA or Canada.

Which groups are affected by _ethnic inequality_? 
---

In many late immigration countries, however, the children of immigrants are also categorised separately. This is particularly true in Germany, where an ethnically defined concept of nation prevailed for a long time and statistics differentiate according to the so-called _“migration background”_ as a personal attribute.

Because of the correspondence between the everyday understanding of belonging and the statistical definition, it is precisely that the concept of migration background is controversial, although it certainly represents progress compared to the differentiation between originals and foreigners (Diehl, 2024)[^1].

It is undisputable that sensitive and inclusion-oriented teachers need to be aware of the well-being of their students and families. Reflecting on social and ethnical inequality, actively, proactively and reactively avoiding discrimination is the task of inclusive pedagogy.

In the next section
----

In the following, we present the first of three case-vignettes, written, explored, and reflected by German Master students in a teacher education project seminar. 

[^1]:Diehl, C. (2024). Migration und ethnische Ungleichheiten. In Handbuch Sozialstrukturanalyse (pp. 1–25). Springer Fachmedien Wiesbaden. https://doi.org/10.1007/978-3-658-39759-3_47-1 

### 5.4 Case-vignette "Language"

Case-vignette “Language & Identiy”
Now, we now describe another case-vignette on the topic of migration and identity. Please take your time and remember: This is an exercise to reflect on your role as a teacher in different classrooms; it is not a test where you have to choose right or wrong answers! 

In Addition: If you are a person with an immigrant background, please imagine that the students (Hadil and Sol) presented in the following case have a different first language than you.

> __Case-vignette "Language" description__
> 
> You are a class teacher at a secondary school that has a high proportion of pupils with a migrant background, while the socio-cultural diversity of your colleagues is rather rare. On the whole, you have the impression that the new students’ transition to school is successful and that they are well integrated after the first year. However, the case of Hadil and Sol, 16-year-old twins, is different. They have been in their class for 10 months, but they still remain alone and do not participate in school activities. They do not speak in the school language, even though they attend the additional language course. They are also silent in English lessons, even though they had English lessons in their home country. They always use a translator for exercises in the classroom and at home and their performance is generally good. However, there is no verbal communication in class, neither with their peers nor with you or other teachers. This is a major problem for social inclusion and educational success. 


In the following, we present different fields of action. At first, you see some possible re-action with regard to your direct contact with Hadil and Sol. Please take your time and reflect on your role as a teacher in this situation. What would you do? Remember that this is not a test with right or wrong answers! 

__Your relation to Hadil and Sol:__

* I stay out of it and do not speak to Hadil and Sol.

* I use a translator to express my own opinion in Hadil and Sol's mother tongue and write to Hadil and Sol to ask them to change their behaviour.

* other re-action (Please use the feedback board at the end of our OER)

__Your relation to your colleagues and others:__

* I do not raise the issue with my colleagues.

* I tell my colleagues about Hadil and Sol and request that we develop a social inclusion plan as a team.

* I tell my family / friends about Hadil and Sol and reflecting the problem of inclusion.

* I get in touch with the social education worker.

* I get in touch with the school psychologist.

* other re-action (Please use the feedback board at the end of our OER)

__Classroom management:__ 

* I continue to use the usual social forms and methods.

* I try to use more co-operative social forms and multilingual activities that strengthen the class community.

* I make the class aware that Hadil and Sol should be included more ,addressing their social exclusion openly in front of the class.

* I follow the curriculum without explicitly addressing the topic of inclusion.

* In order to sensitise the class, I combine the topics of the curriculum with the topic of inclusion.

* other re-action (Please use the feedback board at the end of our OER)

__Your relation to the parents:__ 

* I stay out of it and do not seek contact with the parents. What happens at home is not my responsibility. The twins are old enough.

* I use a translator writing a letter and provide information about help centres.

* I seek dialogue with the parents and a professional interpreter.

* other re-action (Please use the feedback board at the end of our 
OER)



###	5.5 Function, Disability, and Health

It is natural-given that we as human differ in individual physical and cognitive abilities. However, some individuals are disadvantaged in everyday life deviating from the norm in special physical and/or cognitive functions and structures. Here, norm refers to a medically diagnosed condition; i.e., health versus disease/disability. 

International Classification of Function, Disability, and Health (ICF)
---

The _International Classification of Function, Disability, and Health (ICF)_, developed by the World Health Organization (WHO), is a code book that explains health and related conditions in an internationally standardised language. This enables worldwide communication about health and health care. 

The components are described from the perspective of the body, the individual and society in two main lists: 

1. Body functions and body structures 
2. Activities and participation 

accordingly, disability serves as a generic term for impairments of activity and participation. 

The ICF also lists environmental factors that interact with the aforementioned constructs. This enables the user to create useful profiles of a person's functioning, disability and health for different domains. Further, the ICF systematically groups different domains for a person with a specific health problem (e.g., what a person affected by disease actually can do).

<br>
<center>
![](https://euniwell.de.cool/wp-content/uploads/liascript/images/icf-model.jpg "ICF Model, Garro, F., Chiappalone, M., Buccelli, S., De Michieli, L., & Semprini, M. (2021) [^1]")
</center>

It is clear that a teacher’s awareness and sensitive according to the individual (dis)abilities and wellbeing on students is crucial. However, a general education teacher in mainstream schools is not an expert in medicine and special education diagnostic. Therefore, multiprofessional cooperation and interprofessional co-teaching are needed as well as an open, inclusive attitude and general knowledge about some diseases and disabilities. 

Last but not least, it is crucial to know, that we can find relevant information according to a special disease/disability in the [international version of the ICD-11 manual](https://icd.who.int/en). 
The manual offers basic knowledge in order to establish a common ground for the communication with special education teachers. 

In the following we provide an example for Autism-Spectrum-Disorders.


[^1]:Garro, F., Chiappalone, M., Buccelli, S., De Michieli, L., & Semprini, M. (2021). Neuromechanical Biomarkers for Robotic Neurorehabilitation. Frontiers in Neurorobotics, 15. https://doi.org/10.3389/fnbot.2021.742163



Autism-Spectrum-Disorders
===

Due to the variety and diversity of autistic symptoms, the technical term _autism spectrum disorders (ASD)_ is used; see code [6A02 in the ICD-11 Manual](https://icd.who.int/browse/2024-01/mms/en#437815624). The term “spectrum” shows the endeavour to do justice to the wide range of symptoms and typical characteristics as well as the different strengths and abilities, but also the impairments that the respective people with ASD can exhibit, see illustration below.

"Autism spectrum disorder is characterised by persistent deficits in the ability to initiate and to sustain reciprocal social interaction and social communication, and by a range of restricted, repetitive, and inflexible patterns of behaviour, interests or activities that are clearly atypical or excessive for the individual’s age and sociocultural context."[^1]

![](30c58399a08101c24f786dca8c004d57d224d127.png)

In the following section
---
Now we will look at a case vignette about "obesity".

[^1]: ICD-11 for Mortality and Morbidity Statistics. (n.d.). Retrieved November 18, 2024, from https://icd.who.int/browse/2024-01/mms/en#437815624



### 5.6 Case-vignette "Obesity"

Please, take your time and keep in your mind: This is an exercise to think about your role-taking as a teacher in diverse 
classroom settings; it is not a test for choosing right or wrong answers!

<center>![](https://euniwell.de.cool/wp-content/uploads/liascript/images/obesity.jpg "AI Image Gen generated image based on own prompt[^1]")</center>

> __"Obesity" case description__
>
> Andy is 13 years old and has been attending the school where you are his PE teacher for a year. Since changing schools, he has 
> put on a lot of weight and you are now very concerned about his health. In PE lessons, his body is more of a handicap than a 
> strength. You know that Andy is a passionate footballer, but he finds running difficult. In addition, he is increasingly excluded 
> by the other pupils and pushed into the goal at soccer. The class teacher is also worried and has recently had a meeting with his 
> parents. They know from her that the parents seem unconcerned and rejected the advice to seek a consultation with an adolescent 
> doctor. Apparently the mother is overweight herself and the daily routines in the family are hardly supportive for Andy.

Here, you can see some possible feelings and rections.
--- 

Please, think about your role as the teacher, your feeling and handling in this situation. Also, reflect why you prefer this or that as a first reaction? You can note other feelings and ideas for re-action on a separate note (sharing with us on the feedback board after finishing this OER).

__Do you often worry about Andy before the sports lesson? If so, how do you want to deal with it? (several options available) __

* Address the child's physical health directly 
* Talk to the parents
* Ignore it/let it come to you
* Talk to colleagues about experiences and methods 
* Talk about the case in your own private environment, seek advice

__Imagine the teams have been chosen and Andy has been picked last and reluctantly by a team. How do you feel as a teacher on a stress scale of 1-5?__

0. my well-being is unrestricted
1. very slightly stressed
2. slightly stressed
3. moderately stressed
4. quite stressed
5. very stressed

__Would you keep the team selection method in the future? __

* Yes, a different method would not change the situation for Andy, he will have to put up with it or fight back
* Yes, but I will reprimand the class
* No, I choose a different method? e.g. counting out, drawing lots, ...? 
* No, I avoid team games and only do individual exercises in class

__Imagine Andy is standing in the goal and is insulted by his classmates (“You fill the goal perfectly, very good that you are so fat!”) How do you feel as a teacher on a stress scale of 1-5?__

0. my well-being is unrestricted
1. very slightly stressed
2. slightly stressed
3. moderately stressed
4. quite stressed
5. very stressed 

__What feelings do you expect Andy to have when gym class is coming up? Sort the points on a scale according to their strength 0 = not present at all, 1 = very slightly present, .... 5 = very strongly present. __

* Anxiety
* Hope for friendships
* Insecurity
* Helplessness
* Anger that nobody takes him seriously in sports lessons 
* other

[^1]: Photorealistic image of 13 year-old overweight boy with a soccer ball, on a soccer field during PE class.". 


###	5.7 Gender Identity

Now, we focus on two popular models of psychology research that describe general structures and characteristics of human personality. Furthermore, we take a closer look on the construct of gender identity.

In general, gender refers to the attitudes, feelings, and behaviours that a given culture associates with a person's biological sex (APA, 2012)[^1]. The terms related to gender and sex are often conflated, and the language related to gender identity and sexual orientation has also evolved rapidly.

_Gender Identity_ is a component of gender that describes a person's psychological sense of their gender. Many people describe gender identity as a deeply felt, inherent sense of being a boy, a man, or male; a girl, a woman, or female; or a nonbinary gender (e.g., genderqueer, gender-nonconforming, gender-neutral, agender, gender-fluid) that may or may not correspond to a person's sex assigned at birth, presumed gender based on sex assignment, or primary or secondary sex characteristics.

Gender identity applies to all individuals and is not a characteristic only of _transgender_ or _gender-nonconforming_ individuals (APA, 2020)[^2]. The possible dimensions of gender identity are therefore an ongoing finding process.

Scholars in educational research have addressed the challenges of exclusion and marginalisation faced by teachers who identify as lesbian, gay, bisexual, transgender, queer, intersex and asexual (LGBTQIA+). This research could also find out more about the benefits of a diverse teaching body. Whether or not they are open about their orientation, their presence and efforts can have a constructive impact on students' education and development.

Lundin (2024)[^3] examined narratives of _LGBT_ teachers and related them to the general functions of education (i.e. qualification, socialisation, subjectification). It was found that teachers strive for development and change in order to break _heteronormativity_. 

That is, policy documents serve as a first step that requires additional comprehensive efforts in schools to address and implement negative attitudes among adults and in the student-teacher relationship. Below, the illustration presented shows the three functions of school education and __teachers’ narratives).

<center>
![](https://euniwell.de.cool/wp-content/uploads/liascript/images/lundin.png "Own illustration based on Lundin (2024)[^3].")
</center>

In the next section
---
In the following, the last case-vignettes describes a classroom situation with a transgender student. 

[^1]:American Psychological Association. (2012). Guidelines for psychological practice with lesbian, gay, and bisexual clients. The American Psychologist, 67(1), 10–42. https://doi.org/10.1037/a0024659

[^2]:Publication manual of the American Psychological Association (7th ed.) (Vol. 7). (2020). American Psychological Association. https://doi.org/10.1037/0000165-000 

[^3]:Lundin, M. (2024). Heteronormativity in Swedish schools: making a difference as an LGBT teacher. Teachers and Teaching, 1–18. https://doi.org/10.1080/13540602.2024.2381045


### 5.8 Case-vignette "Transgender"

Now, we describe a further, also the last on, case-vignette. Please, take your time and keep in your mind: This is an exercise to think about your role-taking as a teacher in diverse classroom settings; it is not a test for choosing right or wrong answers!

<center>![](https://euniwell.de.cool/wp-content/uploads/liascript/images/transgender.jpg "AI Image Gen generated image based on own prompt[^1]")</center>

> __"Transgender" case description:__
>
> You are a 9th grade teacher at a rural high school. It is the beginning of the school year. You join a new class and find out on the first day that one student (Markus) does not identify with his biological gender. He comes from a strictly religious family that does not accept transgender people. Despite this upbringing, Markus decided during the summer vacation that from now on he only wants to be addressed as Martina and the female pronouns. The parents do not accept their son's decision, so Markus/Martina not only has internal conflicts due to his religiousness, but also external family conflicts. 
>
> After the first few weeks of school together, you as a teacher notice that Martina is having difficulties in the class community and is withdrawing. You fear that Martina is overwhelmed by the situation. It is therefore important to regulate the internal conflicts caused by religion and family conflicts as well as conflicts with classmates in order to avoid further problems such as a drop in school performance.

Here, different fields of action are described. Please, think about your role as the teacher in this situation with Martina. Also, reflect why you prefer this or that as a first reaction? You can note other feelings and ideas for re-action on a separate note (sharing with us on the feedback board after finishing this OER).

__The first field of action concerns your dealings with Martina.__

Choose the option that suits you best. This is about your own assessment.

* I stay out of it and don't talk to Martina about her problems.
* In a conversation with Martina, I refer her to what I think are helpful sources or people to support her.
* I share my own opinion and experiences with Martina.
* Other approach [with text field]

__How do you behave towards Martina?__ 

* I make no active attempts to communicate with Martina.
* I set up a box in which the students can bring concerns to me without having to address me directly. Then I can approach them.
* I speak to Martina directly after the lesson.
* Other approach [with text box]

__How do you deal with other teachers who also teach Martina?__ 

* I don't tell any of my colleagues what I know about Martina's situation.
* I make my colleagues aware that there is a transgender person in the class without saying that it is Martina.
* I tell my colleagues about Martina and her situation.
* Other approach [with text field]

__What do you do regarding the class community?__

* I continue to use the usual social forms and methods.
* I try to use more cooperative social forms and activities that strengthen the class community.
* I ask the class to be more accepting of Martina.
* Other approach [with text field]

__What is your approach to your future teaching?__

* I follow the curriculum without explicitly addressing the topic of transgender.
* In order to sensitize the class, I combine the topics of the curriculum with the transgender issue.
* I openly discuss Martina's case in front of the class.
* Other approach [with text field]

__How do you deal with the parents?__

* I stay out of it and don't seek contact with the parents. What happens at home is not my responsibility.
* I offer myself in writing as a contact person and provide information about other sources of help.
* I seek direct contact with the parents.
* Other procedure [with text field]

[^1]: Thin teenage boy with long hair sitting in classroom, transition to female identiy.

### 5.9 Universal factors of personality structure

People are diverse in personality. Being a sensitive teacher, it is important to know about general personality structures. According to the characteristics, you could be similar to some students while different to the others.

Two models discribe the universal personality structures, the Big-5 and the HEXACO Model.

Big-5 Model
---
The _Big-5 Model_ is examined through an amount of international research. In the 1930s, the development of the model has started with lexical approach studies based on the view that personality traits are reflected in language and that all essential differences between people are already represented in the dictionary by corresponding terms. 

According to the five factors the model is also called the OCEAN-model: __(see Costa & McCrae, 1988; Costa et al., 2019)[^1][^2]

* __Openness:__ practical, prefers routine, comforting (low score); imaginative, prefers variety, independent (high score)

* __Conscientiousness:__ disorganized, careless, impulsive (low score); organized, careful, disciplined (high score)

* __Extraversion:__ retiring, sober, reserved (low score); sociable, affectionate, fun-loving (high score)

* __Agreeableness:__ ruthless, suspicious, uncooperative (low score); soft-hearted, trusting, helpful (high score)

* __Neuroticism:__ calm, secure, self-satisfied (low score); anxious, insecure, self-pitying (high score) 


HEXACO Model
---

The _HEXACO model_ is based on the work of Costa and McCrae's Big Five. However, a significant extension of the HEXACO model is the addition of the dimension Honesty-Modesty (Ashton & Lee, 2007; Lee & Ashton, 2008).[^3][^4]
It also based on international research with the lexical approach including several studies in European and Asia areas. 

The HEXACO-model includes six factors of human personality structures: 

* Honesty-Modesty
* Emotionality 
* Extraversion 
* Compatibility 
* Conscientiousness 
* Openness (to Experience)

The HEXACO questionnaire is availble in many different languages.[^5]

Model Comparison
---

The following illustration based on empirical findings shows a comparison (Iller et al., 2021).[^6]

<center>
![](https://euniwell.de.cool/wp-content/uploads/liascript/images/hexaco-model-en.png "HEXACO & Big-5 Model comparison llustration by Iller et al. (2021), Own translation.[^6].")
</center>



Try to be aware of your bias and reflect your attitude, because research showed that teacher personality treats effect student learning outcomes (e.g., Hattie, 2012)[^7].




[^1]:Costa, P. T., & McCrae, R. R. (1988). Personality in adulthood: A six-year longitudinal study of self-reports and spouse ratings on the NEO Personality Inventory. Journal of Personality and Social Psychology, 54(5), 853–863. https://doi.org/10.1037/0022-3514.54.5.853

[^2]:Costa, P. T., Jr, McCrae, R. R., & Löckenhoff, C. E. (2019). Personality across the life span. Annual Review of Psychology, 70(1), 423–448. https://doi.org/10.1146/annurev-psych-010418-103244

[^3]:Ashton, M. C., & Lee, K. (2007). Empirical, theoretical, and practical advantages of the HEXACO model of personality structure. Personality and Social Psychology Review: An Official Journal of the Society for Personality and Social Psychology, Inc, 11(2), 150–166. https://doi.org/10.1177/1088868306294907

[^4]:Lee, K., & Ashton, M. C. (2008). The HEXACO personality factors in the indigenous personality lexicons of English and 11 other languages. Journal of Personality, 76(5), 1001–1054. https://doi.org/10.1111/j.1467-6494.2008.00512.x

[^5]:Kibeom Lee, Ph.D., & Michael C. Ashton. (2009). THE HEXACO PERSONALITY INVENTORY - REVISED. Hexaco. https://hexaco.org/hexaco-inventory

[^6]:Iller, M.-L., Mäder, R., & Schreiber, M. (2021). Handbuch Fragebogen zur Erfassung der Persönlichkeit (HEXACO-PI-R1). Zürcher Hochschule für Angewandte Psychologie. https://laufbahndiagnostik.psychologie.zhaw.ch/downloads/de/Handbuch_HEXACO-PI-R1.pdf

[^7]:Hattie, John. (2012). Visible learning for teachers. Routledge. https://doi.org/10.4324/9780203181522

## 6. Final Quiz

## 7. Unconsious Bias (Add-on)

![](https://euniwell.de.cool/wp-content/uploads/liascript/images/bias.png)

Why fair decisions are so important in everyday school life 
---

Studies show that triggers of unconscious biases, such as a student’s name or gender, often flow unnoticed into assessment processes and lead to unfair results  (Malouff & Thorsteinsson, 2016).[^1] 

Such biases influence how we perceive and evaluate students - without us realizing it. But it doesn't have to stay that way! This chapter helps you to recognize and reduce these subtle influences so that your decisions remain fair and equitable.

You will expand your knowledge of biases and learn how to minimize them in your everyday school life. Whether you are a (future) teacher, principal or educational staff member - the tool provides practical strategies that you can implement straight away.

In four chapters, you will learn what bias is, where it occurs and how you can make your decision-making more conscious and fairer. Supplemented by practical exercises and reflection tasks, you can integrate what you have learned directly into your everyday teaching.

> __Learning goals__
> 
> * You will learn the basics of unconscious bias.
> * You will find out which biases occur in the school environment.
> * You will learn through practical examples how biases can be avoided.


[^1]:Malouff, J. M., & Thorsteinsson, E. B. (2016). Bias in grading: A meta-analysis of experimental research findings. Australian Journal of Education, 60(3), 245–256. https://doi.org/10.1177/0004944116664618



### 7.1 What ist Bias?

The term _bias_ refers to distortions in information processing that influence our perception and decisions. 

The three main categories of bias are:
---

* __Preference bias__ 

    This describes the favoring or disfavoring of certain groups, often based on stereotypes or prejudices (e.g. gender bias). In physics, men are favored, in the social sciences women (Bernstein et al., 2022)[^1]

* __Structural bias__ 

    These are institutional patterns that unintentionally promote discrimination. One example is medicine, where drugs are often tested on men, leading to inadequate results for women (Criado-Perez, 2019)[^2]

* __Cognitive bias__ 

    This comprises systematic errors in thinking that cloud our judgment, such as confirmation bias. 

    Cognitive biases influence the way in which information is perceived, processed and stored. They arise because our brain processes information selectively in order to make decisions efficiently (Gigerenzer & Brighton, 2009)[^3] 
    In doing so, it uses heuristics that are fast but often inaccurate.

    These cognitive biases are based on the dual process model of cognition (Kahneman, 2012)[^4]

    __Dual process model of cognition__

        * __System 1__ works unconsciously and quickly, but is prone to error.
    
    <center>
    ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/bias-system1-fast.jpg) </center>

    * __System 2__ thinks consciously and analytically, but requires more time and energy. 
    
    <center>
    ![](https://euniwell.de.cool/wp-content/uploads/liascript/images/bias-system2-slow.jpg) </center>

    > Bias often occurs in System 1, which processes this information intuitively, while System 2 is more cautious.

In the teaching context, such biases can influence the way teachers perceive and treat students.

In order to minimize biases, reflection and targeted training are necessary. Systematic analyses and organizational measures help to reduce preference and structural biases, while cognitive biases can be reduced through personal reflection and the conscious use of System 2.

[^1]:Bernstein, A. (2022). Gender Bias in Recommendation Letters for Academics. Journal of Social Psychology.
[^2]:Criado Perez, C. (2019). Invisible women: Exposing data bias in a world designed for men. Vintage Digital.
[^3]:Gigerenzer, G., & Brighton, H. (2009). Homo heuristicus: Why biased minds make better inferences. Topics in Cognitive Science, 1(1), 107–143. https://doi.org/10.1111/j.1756-8765.2008.01006.x
[^4]:Kahneman, D. (2012). Thinking, Fast and Slow. Penguin Books.

### 7.2 Bias in Information Uptake

Our senses are not perfect tools for perceiving reality. The brain decides which information it processes and blocks out others. In the following we present two examples where you can try it out for yourself 

_Motion induced blindness_
----
If you focus on the green dot in the graphic below for a few seconds, the yellow, static dots will disappear.

<br>
<center>
![](https://euniwell.de.cool/wp-content/uploads/liascript/images/motion-blindness.gif "Motion-induced blindness example[^2]")
</center>

_Peripheral Drift illusion_
----

Another example is the optical illusion of moving snakes. Although the image is static, it appears as if the shapes are moving:

<br>

<center>
![](https://euniwell.de.cool/wp-content/uploads/liascript/images/peripheral-drift-illusion.svg "Rotating snakes - Peripheral drift illusion example[^2]")
</center>


> These examples illustrate that our senses distort information, similar to how cognitive biases influence our decisions.

In the example of motion-induced blindness, our brain deliberately filters out information by ignoring static elements in order to emphasize the moving ones. In contrast, in the case of moving snakes, the brain invents additional movements that do not exist. 

These phenomena exemplify how our perception is distorted by neurological mechanisms. Our brain is limited in its processing capacity and makes quick, often erroneous decisions to prioritize and process information - an important insight when dealing with bias.


[^1]:Image by Cmglee, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=24513370
[^2]:Animation by Mlechowicz, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=17583267


### 7.3 Bias in Information Pocessing

In everyday school life, teachers make countless decisions every day - from assessing students' performance to evaluating their behavior. These decisions are often influenced by cognitive biases that we are not aware of. One of these biases is the confirmation bias. 

Confirmation bias
---

> Here, people tend to favor information that supports their pre-existing beliefs and opinions (Nickerson, 1998)[^1]. 

This can also happen at school when teachers have positive or negative expectations of a student. Instead of objectively checking whether these expectations are justified, we unconsciously look for information that 
confirms our view and may ignore evidence to the contrary.

A classic example in the school context would be the assessment of a student who is considered gifted in a particular subject. If this student performs mediocre, the confirmation bias could lead the teacher to interpret this performance as exceptional and continue to assume that the student is fundamentally strong in this subject. On the other hand, a student who the teacher believes to be weak in a particular subject could be judged more harshly even if they perform well.

Choice-supportive bias
---

In addition to the confirmation bias, there is also the choice-supportive bias (Lind et al., 2017)[^2], which supports decisions made in retrospect. 

> This means that we tend to positively reinforce decisions we have made - be it the assessment of students or the 
> choice of certain teaching methods - in retrospect. 

For example, after introducing a new teaching method, a teacher may be inclined to perceive this method as more successful than it actually was, simply because they have already chosen it. This can lead to inadequate methods or approaches being retained instead of being critically questioned and adapted.

In-group bias
---

Another important bias that plays a role in schools is the in-group bias (Taylor & Doria, 1981)[^3]. 

> Here, people tend to treat members of their own “group” better than outsiders. 

At school, this could lead to pupils who share similarities with the teacher - be it in terms of origin, interests or personality - being unconsciously favored. This can influence the assessment of performance, but also behavior towards students. Students who are perceived as “outsiders”, on the other hand, may be unconsciously disadvantaged.


Mere-exposure effect
---
There is also the mere-exposure effect. 

> Here, people evaluate other people or things that they encounter more frequently more positively (Serenko & Bontis, 2011)[^4].

In everyday school life, this could mean that teachers perceive students with whom they have more interaction more positively than those who are quieter or more reserved.

Summary
---

These biases are deeply rooted in the way we process information. They occur because our brains need to process complex information quickly and efficiently. Although these mental shortcuts, known as heuristics (Tversky & Kahneman, 1973), help us to cope with everyday life, they can lead to unfair judgments in specific situations - especially when it comes to assessing students. The challenge is to become aware of these biases and take action to minimize them. 

In the next section
----
To counteract these biases, teachers can use various strategies, which we explain in the next chapter.

[^1]:Nickerson, R. S. (1998). Confirmation bias: A ubiquitous phenomenon in many guises. Review of General Psychology: Journal of Division 1, of the American Psychological Association, 2(2), 175–220. https://doi.org/10.1037/1089-2680.2.2.175

[^2]:Lind, M., Visentini, M., Mäntylä, T., & Del Missier, F. (2017). Choice-supportive misremembering: A new taxonomy and review. Frontiers in Psychology, 8. https://doi.org/10.3389/fpsyg.2017.02062

[^3]:Taylor, D. M., & Doria, J. R. (1981). Self-serving and group-serving bias in attribution. The Journal of Social Psychology, 113(2), 201–211. https://doi.org/10.1080/00224545.1981.9924371

[^4]:Serenko, A., & Bontis, N. (2011). What’s familiar is excellent: The impact of exposure effect on perceived journal quality. Journal of Informetrics, 5(1), 219–223. https://doi.org/10.1016/j.joi.2010.07.005


### 7.4 Reducing Bias in Communication

The American Psychological Association (APA) has stated its commitment both to the advancement of science and to the fair treatment of individuals and groups:
As using inclusive language can foster the fair treatment of individuals and groups and the advancement of research, the American Psychological Association (APA) has made recommendations on bias-free language which are also of interest to educators:

>“It is unacceptable to use constructions that might imply prejudicial beliefs or perpetuate biased assumptions against persons on the basis of age, disability, gender, participation in research, racial or ethnic identity, sexual orientation, socioeconomic status, or some combination of these or other personal factors (e.g., marital status, immigration status, religion). Instead, authors should use affirming and inclusive language.” (APA, 2020, p.131)[^1].

Bias-free language guidelines
---

For this, the APA Editors have published “Bias-free language guidelines” that helps people around the world in psychology, social work, communications to education to achieve excellence in writing. With regard to bias-free language of teachers in verbal and written communication with students, parents, and other professionals, we assume some of the main ideas the APA (2020) described:

1. Talking about disability: Names of conditions such as “Asperger autism” and “Attention deficit disorder with hyperactivity” are more specific than “a student with disability” or “a student with special needs”.

2. Be sensitive to labels Respect the language people use to describe themselves; that is, call people what they call themselves. You may need to ask your students which designations they use. Also, accept that language changes over time and individuals within groups sometimes disagree about the designations they use.

3. Acknowledge people's humanity Ensuring that the individuality and humanity of people are respected. Avoid using adjectives as nouns to label people (e.g., "the gays," "the poor") or labels that equate people with their condition (e.g., "the learning disabled," "the autisms"). Use adjectival forms (e.g., gay men, older adults) or nouns with descriptive phrases (e.g., people living in poverty, people with learning disabilities).

Overall, using a sensitive, _bias-free language_ is important in direct and written communication as well as professional teaching and being a social role model.

[^1]:Publication manual of the American Psychological Association (7th ed.) (Vol. 7). (2020). American Psychological Association. https://psycnet.apa.org/doi/10.1037/0000165-000 

### 7.5 Minimize Bias in Decision-making

Although knowledge of bias is important, it is not enough to avoid these biases (Bezrukova et al., 2016; Devine & Ash, 2021)[^1][^2]. This is because bias is often automatically activated by our fast decision-making system, System 1. To minimize bias, it is important to consciously activate System 2, but this can be exhausting and time-consuming. 

Nevertheless, there are practical steps to reduce bias in decision-making - especially in the school context, where fair assessments of students are important.

Methods for bias reduction
---

One effective method is bias reduction, in which bias is systematically minimized through structured processes. Examples of this in everyday school life are

* __Anonymization of exams:__ 

    If teachers do not know the names of students, the halo or horn effect, where previous performance could influence the assessment, is reduced.

* __Elimination of irrelevant information:__

    When evaluating performance, irrelevant information such as personal bias should not be included. Avoiding bias due to characteristics such as origin or gender can reduce in-group bias.

* __Use clear evaluation criteria:__

    Structured and pre-defined criteria, such as for oral exams or project work, help to minimize subjective assessments. By defining clear benchmarks (e.g. on a scale from A to C or 1 to 6), it can be ensured that the assessment is more objective and that there is less room for bias.

Group decisions at school
----

Many important decisions in everyday school life - such as performance assessments or support measures - are made in groups. Such decisions are particularly susceptible to distortions such as social desirability bias or the influence of information cascades. These arise when influential group members express an opinion that others follow uncritically. 

In a meeting to finalise grades, the opinion of an experienced teacher could unconsciously influence everyone else and cause them to change their mind about the grade a student deserves. Kahneman et al. (2021)[^3] have coined the term _“decision hygiene”_, which describes strategies to reduce such biases in groups. This includes measures such as:

* __Independent judgments:__ 
    
    Group members should only express their opinions once they have made their decisions independently. This avoids cascading effects.

* __Anonymous voting:__

    To reduce social desirability bias, decisions should be made as anonymously as possible. This prevents individuals from changing their minds for social reasons just to suit the group.

* __Clear evaluation criteria and structured discussions:__ 

    To avoid group polarization, discussions should be clearly structured and moderated. Groups tend to reinforce their opinions in discussions, which can lead to more extreme decisions than originally planned.

Practical steps for everyday school life
---

To reduce bias in the school decision-making process, several steps are useful:

1. use pre-defined criteria: Criteria should be defined before a decision is made and only consider relevant aspects of student performance.

2. use assessment guidelines: Structured guides, especially for oral exams or project assessments, help to minimize subjective bias.

3. enable independent assessments: Individual assessments should be completed prior to group sharing to minimize the influence of social dynamics.

4. subsequent reflection: After making a decision, teachers should consciously take time to question their own decision and reflect on possible biases. This can be supported in peer groups or through coaching.

Conclusion
---
Bias in decision-making can be effectively minimized through structured processes, clear criteria and the reduction of social influence factors - an approach that ensures greater fairness both in individual performance and in group decisions in the school context.

[^1]:Bezrukova, K., Spell, C. S., Perry, J. L., & Jehn, K. A. (2016). A meta-analytical integration of over 40 years of research on diversity training evaluation. Psychological Bulletin, 142(11), 1227–1274. https://doi.org/10.1037/bul0000067

[^2]:Devine, P. G., & Ash, T. L. (2022). Diversity training goals, limitations, and promise: A review of the multidisciplinary literature. Annual Review of Psychology, 73(1), 403–429. https://doi.org/10.1146/annurev-psych-060221-122215

[^3]:Kahneman, D., Sibony, O., & Sunstein, C. R. (2022). Noise: A flaw in human judgment. Little Brown and Company.



### 7.6 Summary Quiz

<iframe src="https://euniwell.de.cool/wp-admin/admin-ajax.php?action=h5p_embed&id=38" width="958" height="298" frameborder="0" allowfullscreen="allowfullscreen" title="Unconcious Bias (Question Set)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>


## Your Feedback

We are committed to continuous improvement and welcome anonymous feedback on the [feedback wall](https://padlet.com/teacheredueuniwell/oerdiversityinclusion).

Feedback wall
-------------

<div class="padlet-embed" style="border:1px solid rgba(0,0,0,0.1);border-radius:2px;box-sizing:border-box;overflow:hidden;position:relative;width:100%;background:#F4F4F4"><p style="padding:0;margin:0"><iframe src="https://padlet.com/embed/t9twf0p8n7gd2wo3" frameborder="0" allow="camera;microphone;geolocation" style="width:100%;height:608px;display:block;padding:0;margin:0"></iframe></p><div style="display:flex;align-items:center;justify-content:end;margin:0;height:28px"><a href="https://padlet.com?ref=embed" style="display:block;flex-grow:0;margin:0;border:none;padding:0;text-decoration:none" target="_blank"><div style="display:flex;align-items:center;"><img src="https://padlet.net/embeds/made_with_padlet_2022.png" width="114" height="28" style="padding:0;margin:0;background:0 0;border:none;box-shadow:none" alt="Mit Padlet erstellt"></div></a></div></div>


## Bibliography

References
Abbott, K. (2014). Social justice. In Encyclopedia of Quality of Life and Well-Being Research (pp. 6115–6119). Springer Netherlands.

American Psychological Association. (2012). Guidelines for psychological practice with lesbian, gay, and bisexual clients. The American Psychologist, 67(1), 10–42. https://doi.org/10.1037/a0024659

Ashton, M. C., & Lee, K. (2007). Empirical, theoretical, and practical advantages of the HEXACO model of personality structure. Personality and Social Psychology Review: An Official Journal of the Society for Personality and Social Psychology, Inc, 11(2), 150–166. https://doi.org/10.1177/1088868306294907

Bell, L. A. (2007). Theoretical foundations for social justice education. In M. Adams (Ed.), Teaching for diversity and social justice (pp. 1–14). Routledge/Taylor & Francis Group.

Bernstein, A. (2022). Gender Bias in Recommendation Letters for Academics. Journal of Social Psychology.

Bezrukova, K., Spell, C. S., Perry, J. L., & Jehn, K. A. (2016). A meta-analytical integration of over 40 years of research on diversity training evaluation. Psychological Bulletin, 142(11), 1227–1274. https://doi.org/10.1037/bul0000067

Bronfenbrenner, U. (1977). Toward an experimental ecology of human development. The American Psychologist, 32(7), 513–531. https://doi.org/10.1037/0003-066x.32.7.513

Bronfenbrenner, U. (1979). The ecology of human development: Experiments by nature and design. Harvard University Press.

Brüderl, J. (2019). Vorlesung Sozialstrukturanalyse. https://www.ls3.soziologie.uni-muenchen.de/studium-lehre/lehrmaterialien/ws-2019-2020/vorlesung-sozialstruktur_19.pdf

Bührmann, A. (2018). Diversität. Socialnet Lexikon. https://www.socialnet.de/lexikon/6324

Costa, P. T., Jr, McCrae, R. R., & Löckenhoff, C. E. (2019). Personality across the life span. Annual Review of Psychology, 70(1), 423–448. https://doi.org/10.1146/annurev-psych-010418-103244

Costa, P. T., & McCrae, R. R. (1988). Personality in adulthood: A six-year longitudinal study of self-reports and spouse ratings on the NEO Personality Inventory. Journal of Personality and Social Psychology, 54(5), 853–863. https://doi.org/10.1037/0022-3514.54.5.853

Cramer, C., & Harant, M. (2014). Inklusion – Interdisziplinäre Kritik und Perspektiven von Begriff und Gegenstand. Zeitschrift fur Erziehungswissenschaft: ZfE, 17(4), 639–659. https://doi.org/10.1007/s11618-014-0584-4

Criado Perez, C. (2019). Invisible women: Exposing data bias in a world designed for men. Vintage Digital.

Del Gobbo, Daniela Frison, André Bresges, Donna J. Dawkins, Jan Springob, Juan Antonio Solis Becerra, Ibolya Túri, Magali Hersant, Giovanna. (2023). Sustainability, health care, well-being, and inclusion: toward new professional standards for the teachers of the future. Nuova Secondaria , 5, 146–154.

Deutsches Institut für Menschenrechte, & UN-Behindertenrechtskonvention, M.-S. (2023). Parallel report to the UN Committee on the Rights of Persons with Disabilities for Germany’s 2nd/3rd State Party review procedure. 59. https://www.ssoar.info/ssoar/handle/document/88647

Devine, P. G., & Ash, T. L. (2022). Diversity training goals, limitations, and promise: A review of the multidisciplinary literature. Annual Review of Psychology, 73(1), 403–429. https://doi.org/10.1146/annurev-psych-060221-122215

Diehl, C. (2024). Migration und ethnische Ungleichheiten. In Handbuch Sozialstrukturanalyse (pp. 1–25). Springer Fachmedien Wiesbaden.

Education and Disability: Analysis of data from 49 countries. (2018, March 22). Unesco.org. https://uis.unesco.org/en/news/education-and-disability-analysis-data-49-countries

Epp, A. (2017). Das ökosystemische Entwicklungsmodell als theoretisches Sensibilisierungs- und Betrachtungsraster für empirische Phänomene. https://doi.org/10.17169/fqs-19.1.2725

EUniWell. (n.d.). Our Alliance. European University for Well-Being. Retrieved November 19, 2024, from https://www.euniwell.eu/about/our-alliance

EUniWell. (2023). EUniWell Mission Statement. https://www.euniwell.eu/fileadmin/user_upload/Downloads/Key_documents/2023_EUniWell_Mission_Statement_-_updated.pdf

Fend, H. (2009). Neue Theorie der Schule. VS Verlag für Sozialwissenschaften.

Florian, L. (2017). Teacher education for the changing demographics of schooling: Inclusive education for each and every learner. In Teacher education for the changing demographics of schooling (pp. 9–20). Springer.

Frederick, A., & Katz, J. H. (2002). The Inclusion Breakthrough: Unleashing the Real Power of Diversity Miller. Berrett-Koehler Punlishers, Inc.

Friend, M., Cook, L., Hurley-Chamberlain, D., & Shamberger, C. (2010). Co-teaching: An illustration of the complexity of collaboration in special education. Journal of Educational and Psychological Consultation: The Official Journal of the Association for Educational and Psychological Consultants, 20(1), 9–27. https://doi.org/10.1080/10474410903535380

Garro, F., Chiappalone, M., Buccelli, S., De Michieli, L., & Semprini, M. (2021). Neuromechanical Biomarkers for Robotic Neurorehabilitation. Frontiers in Neurorobotics, 15. https://doi.org/10.3389/fnbot.2021.742163

Grosche, M. (2015). Was ist Inklusion? Ein Diskussions- und Positionsartikel zur Defi nition von Inklusion aus Sicht der empirischen Bildungsforschung. In P. Kuhl, P. Stanat, B. Lütje-Klose, C. Gresch, H. A. Pant, & M. Prenzel (Eds.), Inklusion von Schülerinnen und Schülern mit sonderpädagogischem Förderbedarf in Schulleistungserhebungen (pp. 17–39). Springer Fachmedien Wiesbaden. https://doi.org/10.1007/978-3-658-06604-8

Gigerenzer, G., & Brighton, H. (2009). Homo heuristicus: Why biased minds make better inferences. Topics in Cognitive Science, 1(1), 107–143. https://doi.org/10.1111/j.1756-8765.2008.01006.x

Handbook for Teachers on Inclusive Education. (2020). Central Board of Secondary Education, Acedemic Unit. https://cdnbbsr.s3waas.gov.in/s3kv011a846fe7a5fa4b4b6d1eca45b228/uploads/2024/02/2024020919.pdf

Hans, H. (1989). Intersubjektivität - Die Entwicklung des Werkes von G. Suhrkamp.

Hattie, J. (2012). Visible learning for teachers. Routledge. https://doi.org/10.4324/9780203181522

Helle, H. J. (2001). Theorie der symbolischen Interaktion: ein Beitrag zum verstehenden Ansatz in Soziologie und Sozialpsychologie.

Jurkowski, S., Ulrich, M., & Müller, B. (2023). Co-teaching as a resource for inclusive classes: teachers’ perspectives on conditions for successful collaboration. International Journal of Inclusive Education, 27(1), 54–71. https://doi.org/10.1080/13603116.2020.1821449

Kahneman, D. (2012). Thinking, Fast and Slow. Penguin Books.

Kahneman, D., Sibony, O., & Sunstein, C. R. (2022). Noise: A flaw in human judgment. Little Brown and Company.

Kibeom Lee, Ph.D., & Michael C. Ashton. (2009). THE HEXACO PERSONALITY INVENTORY - REVISED. Hexaco. https://hexaco.org/hexaco-inventory

Köpfer, A., Powell, J. J. W., & Zahnd, R. (2021). Handbuch Inklusion international / International Handbook of Inclusive Education (A. Köpfer, J. J. W. Powell, & R. Zahnd, Eds.). Verlag Barbara Budrich.

Lee, K., & Ashton, M. C. (2008). The HEXACO personality factors in the indigenous personality lexicons of English and 11 other languages. Journal of Personality, 76(5), 1001–1054. https://doi.org/10.1111/j.1467-6494.2008.00512.x

Lind, M., Visentini, M., Mäntylä, T., & Del Missier, F. (2017). Choice-supportive misremembering: A new taxonomy and review. Frontiers in Psychology, 8. https://doi.org/10.3389/fpsyg.2017.02062

Lundin, M. (2024). Heteronormativity in Swedish schools: making a difference as an LGBT teacher. Teachers and Teaching, 1–18. https://doi.org/10.1080/13540602.2024.2381045

Lütje-Klose, B., Wild, E., Grüter, S., Gorges, J., Neumann, P., Papenberg, A., & Goldan, J. (2024). Kooperation in inklusiven Schulen: Ein Praxishandbuch zur Zusammenarbeit in multiprofessionellen Teams und mit Eltern. transcript Verlag.

Malouff, J. M., & Thorsteinsson, E. B. (2016). Bias in grading: A meta-analysis of experimental research findings. Australian Journal of Education, 60(3), 245–256. https://doi.org/10.1177/0004944116664618

Mead, G. H. (1934). Geist, Identität und Gesellschaft: aus der Sicht des Sozialbehaviorismus. Suhrkamp.

Nickerson, R. S. (1998). Confirmation bias: A ubiquitous phenomenon in many guises. Review of General Psychology: Journal of Division 1, of the American Psychological Association, 2(2), 175–220. https://doi.org/10.1037/1089-2680.2.2.175

OECD. (2024). Education at a glance 2024: OECD indicators. OECD. https://doi.org/10.1787/c00cad36-en

Popkewitz, T. S. (2004). Educational standards: Mapping who we are and are to become. The Journal of the Learning Sciences, 13(2), 243–256.

Publication manual of the American Psychological Association (7th ed.) (Vol. 7). (2020). American Psychological Association. https://doi.org/10.1037/0000165-000

Riccomini, P., & Witzel, B. (2010). Response to Intervention in Math. Corwin Press.

Serenko, A., & Bontis, N. (2011). What’s familiar is excellent: The impact of exposure effect on perceived journal quality. Journal of Informetrics, 5(1), 219–223. https://doi.org/10.1016/j.joi.2010.07.005

Stichweh, R. (2007). Inklusion und Exklusion in der Weltgesellschaft – Am Beispiel der Schule und des Erziehungssystems. In Intention und Funktion (pp. 113–120). VS Verlag für Sozialwissenschaften.

Studienseminar Hannover für das Lehramt für Sonderpädagogik. (n.d.). Handreichungen zur Ausbildung im gemeinsamen Unterricht. https://lehrerfortbildung-bw.de/s_sueb/alle/fb1/6_mat/3_zusammen/11_lit/Handreichungen-zur-Ausbildung-im-gemeinsamen-Unterrich.pdf

Sturm, T., & Wagner-Willi, M. (Eds.). (2018). Handbuch schulische Inklusion. utb GmbH.

Taylor, D. M., & Doria, J. R. (1981). Self-serving and group-serving bias in attribution. The Journal of Social Psychology, 113(2), 201–211. https://doi.org/10.1080/00224545.1981.9924371

Thomas, G. (2013). A review of thinking and research about inclusive education policy, with suggestions for a new kind of inclusive thinking. British Educational Research Journal, 39(3), 473–490. https://doi.org/10.1080/01411926.2011.652070

UNESCO Global Education Monitoring Report Team, International Task Force on Teachers for Education. (2020). Inclusive teaching: preparing all teachers to teach all students. https://unesdoc.unesco.org/ark:/48223/pf0000374447

UNESCO. (2020). Global Education Monitoring Report 2020: Inclusion and education: All means all. Paris. UNESCO. https://doi.org/10.54676/jjnk6989

UNESCO. Assistant Director-General for Education, 2010-2018 (Qian Tang), & UNESCO. (2017). A Guide for ensuring inclusion and equity in education. UNESCO. https://doi.org/10.54675/mhhz2237

UNESCO, Institute for Statistics. (2018). Education and Disability: Analysis of Data from 49 Countries. https://uis.unesco.org/sites/default/files/documents/ip49-education-disability-2018-en.pdf

Universität Rostock. (n.d.). The Response-to-Intervention Approach. Universität Rostock. Retrieved October 7, 2024, from https://www.rim.uni-rostock.de/en/response-to-intervention-approach/the-response-to-intervention-approach/

V. Aichele, LL.M., S. Bernot, C. Hübner, S. Kroworsch, B.Leisering, P. Litschke, L. Palleit, K. Pöllmann, J. Striek. (2019). Wer Inklusion will, sucht Wege Zehn Jahre UN-Behindertenrechtskonvention in Deutschland. Deutsche Institut für Menschenrechte, Monitoring-Stelle UN-Behindertenrechtskonvention. https://www.institut-fuer-menschenrechte.de/fileadmin/Redaktion/Publikationen/Wer_Inklusion_will_sucht_Wege_Zehn_Jahre_UN_BRK_in_Deutschland.pdf

van der Gaag, R. J. (2010). S. L. Odom, R. H. Horner, M. E. Snell, & J. Blacher (Eds.) (2007). Handbook of developmental disabilities. New York/Londen: Guilford Press. 645 p., isbn 978 1 5938 5485 0, $ 95,-. Kind en adolescent, 31(2), 104–105. https://doi.org/10.1007/bf03089708

Waack, S. (n.d.). Hattie effect size list - 256 Influences Related To Achievement. VISIBLE LEARNING. Retrieved October 7, 2024, from https://visible-learning.org/hattie-ranking-influences-effect-sizes-learning-achievement/

Walgenbach, K. (2021). Erziehungswissenschaftliche Perspektiven auf Vielfalt, Heterogenität, Diversity / Diversität, Intersektionalität. Verlag Julius Klinkhardt. https://doi.org/10.25656/01:22247




## Author Credits and Contact Information

The content of this OER is provided by the University of Konstanz as part of the [EUniWell project](https://www.euniwell.eu/) funded by the European Union.

Authors: Dr. Manuela Ulrich, Sarah Roos, Michael Kowalczyk

Publication date:

Date of last update: 

E-mail: [teacheredu.euniwell@uni-konstanz.de](mailto:teacheredu.euniwell@uni-konstanz.de)

## Downloads

* OER Download

  * .md file, image files, h5p files in one zip.
  * SCORM 2004 zip file
  * Docx Documents
  * Media files
  * H5P files

## Temporary (to be removed)

### YT

<iframe style="width: 100%; aspect-ratio: 16 / 9; margin-top: 10px " src="https://www.youtube.com/embed/videoseries?si=_pLFHznqfxMOQz3O&amp;list=PLCDsTyftAA2D_buI_Rti5phLZ1DdFsAMc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


<iframe style="width: 100%; aspect-ratio: 16 / 9; margin-top: 10px " src="https://euniwell.de.cool/wp-content/uploads/liascript/h5p/1.html" title="H5P" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


| for students                                                           | for teachers |
| ---------------------------------------------------------------------- |:------------:|
| children are not feeling labeld and excluded, excluded, peer teaching, different strategies, flexible groups |     better understanding of the materials, flexible groups, different strategies,      |

### Admonition

<!-- class="admonition note" -->
> <!-- class="admonition-title" --> This is a test
>
> Foo
> bar
> sadsfasfd

---

> @admonition(warning,This is a test)
>
> Foo
> bar
> sadsfasfd

---

> @admonition(danger,This is a test)
>
> Foo
> bar
> sadsfasfd

---

<section class="admonition note">
<h5 class="admonition-title">NOTE</h5>
This is a note admonition
</section>
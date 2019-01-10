+++
date = "2019-01-09T21:05:33+05:30"
title = "About me"
+++

**Architect**, pastry chef and coffee lover. I´m currently living in Barcelona, and absolutely love the city. Never though I would be able to live in the same city as Gaudí. Would like to design as him, but for now I´m in the path of learning. And my path takes me to the world of interior design, which is where I´m focusing right now.

I´m currently collaborating with **RAUM studio** as a freelance architect. This studio specializes on retail design, focusing on branding, interior design and mobile design.

   ![This is me][1]




#### Education

**Postgraduate course: Projecting the hotel of the XXI century** 
by ESCOLA SERT -OF THE CATALUNYA SCHOOL OF ARCHITECTS-
Barcelona, Spain // Jan 2018 - Jul 2018 

**Architecture licenciate** 
by FRANCISCO MARROQUÍN UNIVERSITY
Guatemala city, Guatemala // 2013

**Architecture Lab: The link between history and contemporary Russian architecture** 
by FRANCISCO MARROQUÍN UNIVERSITY
Moscow, Russia - Saint Petersburg, Russia // July 2011

**Digital Fabrication (Fablab) by Prof. Axel Paredes of Paredes + Alemán arquitectos**
by FRANCISCO MARROQUÍN UNIVERSITY
Guatemala city, Guatemala // 2009


##### Complementary studies

**Master in hotel, restaurant, and F&B management** 
by OSTELEA SCHOOL OF TOURISM & HOSPITALITY
Barcelona, Spain // 2017

**Pastry chef**
by ESCUELA DE HOSTELERÍA HOFMANN
Barcelona, Spain // 2015-2016


#### Languages
**Spanish**  Maternal language        **English**  Advanced level

**French**   Basic Level              **Catalan**  Undestand common talk


[1]: /img/About 1.jpg

{{ if .Site.Data.skill.enable }}
{{"<!-- Skills -->" | safeHTML }}
<section id="team-skills" class="parallax-section section section-bg overly">
    <div class="container">
        <div class="row">
            {{"<!-- section title -->" | safeHTML }}
            <div class="col-md-12">
                <div class="title text-center">
                    <h2>{{ with .Site.Data.skill.heading}} {{ . }} {{ end }} <span class="color">{{ with .Site.Data.skill.headingSpan }} {{ . }} {{ end }}</span></h2>
                    <div class="border"></div>
                </div>
            </div>
            {{"<!-- /section title -->" | safeHTML }}
        </div>
        <div class="row">
            <div class="col-md-6">
                {{ with .Site.Data.skill.title }} <h2> {{ . }} </h2> {{ end }}
                {{ with .Site.Data.skill.content }} <p> {{ . }} </p> {{ end }}
                <img class="img-responsive" src="{{ .Site.Data.skill.image | absURL }}" alt="image">
            </div>
            <div class="col-md-6">
                <ul class="skill-bar">
                    {{ range .Site.Data.skill.skillItem }}
                    <li>
                        <p><span>{{ .itemNumber }}</span>{{ .itemName }}</p>
                        <div class="progress">
                            <div class="progress-bar" role="progressbar" aria-valuenow="70" aria-valuemin="0"
                                aria-valuemax="100" style="width:{{ .itemPercent }}">
                            </div>
                        </div>
                    </li>
                    {{ end }}
                </ul>
            </div>
        </div>
    </div>
</section>
{{"<!-- /skill -->" | safeHTML }}
{{ end }}


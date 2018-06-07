---
layout: category
title: project
permalink: /project/
---

<h1 class="page-title">{{ page.title | escape }}</h1>

<div class="section">
    <div style="background: #ddd">
        <div class="container last-post">
        <section>
            <h5>Project list</h5>
            {% assign category = page.category | default: page.title %} <!-- 같은 title 찾기 -->
            
            <ul class="collection">
             <li class="collection-item avatar">
                <div class="date-post">P_01</div>
                <span class="title"><a class="post-link" href="https://github.com/soyunni/psy_world">psy_world</a></span>
                <p>
                   Spring boot + mysql + jsp + jquery > 일반 게시판 
                </p>
                <a href="https://github.com/soyunni/psy_world" class="secondary-content"><i class="material-icons"></i></a>
              </li>
              
               <li class="collection-item avatar">
                  <div class="date-post">P_02</div>
                  <span class="title"><a class="post-link" href="https://github.com/soyunni/btw-project">btw-project</a></span>
                  <p>
                    config 하나로 view 설정 바꿔서 노출
                  </p>
                  <a href="https://github.com/soyunni/psy_world" class="secondary-content"><i class="material-icons"></i></a>
                </li>
            </ul>
        </section>
     </div>
</div>

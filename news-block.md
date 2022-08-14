---
layout: main
---
<div class="block-wrapper news-wrapper container-fluid">
    <div class="row-fluid">
        <div class="span12">
            <h2>NOTÍCIAS</h2> </div>
    </div>
    <div class="row-fluid">
        {% for post in site.posts limit:3 %}
            <div class="span4">
                <a href={{item.url}} target="_blank">
                    <div class="image-wrapper">
                    <div class="blue-overlay"></div>
                    <img alt="Noticia 1 Foto" src={{site.baseurl}}{{item.splash}}> </div>
                    <div class="date-wrapper">
                        <i class="icon-calendar"></i><span>{{post.date | date:"%b %d"}}</span>
                    </div>
                    <div class="lead3">{{post.title}}</div>
                    <div class="p2">{{post.excerpt}}</div>
                </a>
            </div>
        {% endfor %}
    </div>
    <!--<div class="row-fluid">
        <div class="pages-wrapper">
            <a href="javascript:void(0);"> <i class="icon-long-arrow-left"></i> </a>
            <a href="javascript:void(0);" style="margin-left: 30px;"> <i class="icon-long-arrow-right"></i> </a>
        </div>
    </div>-->
    <div class="row-fluid" style="margin: 35px 0 45px 0;">
        <div class="span12"> <a href="news.html" class="button button1">Ir para notícias</a> </div>
    </div>
</div>
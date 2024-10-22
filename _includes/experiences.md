
<div class="publications">
<ol class="bibliography">

<h2 style="margin:0 10px 0;">Experience</h2>

{% for experience in site.data.experiences%}
<li>
    <div class="pub-row">
        <!-- 左边的列，用于显示公司图标 -->
        <div class="col-sm-3" style="position: relative;padding-right: 15px;padding-left: 15px;">
            {% if experience.logo %} 
            <img src="{{ experience.logo }}" class="teaserexperience img-fluid z-depth-1" style="width=100;height=40%;">
            {% endif %}
        </div>
        <!-- 右边的列，用于显示实习的详细信息 -->
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
            <div class="title"><strong>{{ experience.company }}</strong></div>
            <div> Position: {{ experience.position }}</div>
<!--             <div>Topics: {{ experience.topics }}</div> -->
            <div>Advisor: {{ experience.advisors }}</div>
            {% if experience.topic %}
            <div>Topic: {{ experience.topic }}</div>
            {% endif %}
            <div>{{ experience.duration }}</div>
        </div>
    </div>
    <br>
</li>
{% endfor %}


</ol>
</div>

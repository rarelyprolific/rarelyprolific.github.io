---
layout: default
---
<section id="one" >
    <div class="container">
        {% for post in site.posts limit:1 %}
            <article>
                <header>
                    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
                    <h4>{{ post.date | date: "%b %-d, %Y" }} • <a href="http://www.rarelyprolific.co.uk{{ post.url }}#disqus_thread">0 Comments</a></h4>
                </header>
                <section class="post-content">
                    {{ post.excerpt }}
                </section>
                <section class="special">
                    <ul class="actions">
                        <li><a href="{{ site.baseurl }}{{ post.url }}" class="button special">Read More</a></li>
                    </ul>
                </section>
            </article>
        {% endfor %}
    </div>
</section>
<section>
    <div class="container">
        <div class="features">
        {% for post in site.posts offset:1 %}
            <article>
                <section class="excerpt">
                <header>
                    <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
                    <h4>{{ post.date | date: "%b %-d, %Y" }} • <a href="http://www.rarelyprolific.co.uk{{ post.url }}#disqus_thread">0 Comments</a></h4>
                </header>
                
                    {{ post.content | truncatewords: 30 | strip_html }}
                </section>
				<br />
                <footer>
                    <ul class="actions">
                        <li><a href="{{ site.baseurl }}{{ post.url }}" class="button">Read More</a></li>
                    </ul>
                </footer>
                <div class="clear"></div>
            </article>
        {% endfor %}
        </div>
    </div>
</section>
# frask-todo-app
# frask-todo-app

index.html 変更前
```
{% extends 'base.html' %}

{% block body %}
<h1>トップページ</h1>
<a href="/create" role="button">CREATE NEW TASK</a>
{% for post in posts %}
    <h2>タイトル : {{ post.title }}</h2>
    <p>期限 ： {{ post.due.date() }}</p>
    <a href="/detail/{{ post.id }}" role="button">Detail</a>
    <a href="/update/{{ post.id }}" role="button">Update</a>
    <a href="/delete/{{ post.id }}" role="button">Delete</a>
{% endfor %}
{% endblock %} 
```

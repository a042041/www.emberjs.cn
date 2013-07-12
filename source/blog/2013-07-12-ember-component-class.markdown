---
title: Ember.JS component
tags: 最近文章
---

随着Ember.JS升级到rc6，使原本已经拥有成熟API的Ember框架又多了新的成员--[Component](http://emberjs.com/api/classes/Ember.Component.html).

在'Ember.Component'下定义的View是完全独立的。如果某一template是此Viem的对象，它可以访问View的行为和控制contextual information的输入。对其他无关的则没有权限去访问

创建一个最简单的'Ember.Component'的应用是在template中。假设在template中有一个名为'controls/my-foo'的控件，那么就可以在任意的一个template中去引用'{{my-foo}}'来使用'controls/my-foo'.并且它会是一个可独立的控制实例。

也可以使用'yield'去自定义template的内容

可以为其本身自定义controller，用以处理events or
actions。使用implament实现以'Ember.Component'命名，控制的子类

Components在命名中必须要有'-'，以避免和HTML的内置控件元素发生冲突。


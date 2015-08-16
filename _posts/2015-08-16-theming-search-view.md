---
layout: post
title: Theming SearchView
---

This post will cover how to theme Android's `SearchView`.

1. You're using a `NoActionBar` theme.
2. You're using a dark color for the `Toolbar`s you're including in your layouts.
3. You're trying to style the `SearchView` so that the text color, text hint color, and icons to show your accent color.

Like this. Easy huh? 😎

![theming-search-view-1]({{ site.assets }}/images/theme-search-view-1.png "theming-search-view-1")
![theming-search-view-2]({{ site.assets }}/images/theme-search-view-2.png "theming-search-view-2")
![theming-search-view-3]({{ site.assets }}/images/theme-search-view-3.png "theming-search-view-3")

Let's take a look at the default theming, with the `colorPrimary`, `colorPrimaryDark` and `colorAccent` defined.

{% gist turbogunhawk/4046caa2a406c7d94e75 %}

First, let's remove the `Toolbar` from the theme by switching to a `NoActoinBar` theme, then add on the activity layout.

{% gist turbogunhawk/5d066ed78c5c850de515 %}

{% gist turbogunhawk/ea1656c1f014a89a1aea %}

{% gist turbogunhawk/2f41550019dc4d6d3768 %}

Switching to `NoActionBar` and moving the `Toolbar` to the layout results in this. _Gross._
![theming-search-view-4]({{ site.assets }}/images/theme-search-view-4.png "theming-search-view-4")

So what can we do? Let's start by adding some styles to the `Toolbar`.

{% gist turbogunhawk/e1e90636fcf449a111c1 %}

{% gist turbogunhawk/caef0db568599a498dbc %}

Adding the `ThemeOverlay` is a start but still a far cry.
![theming-search-view-5]({{ site.assets }}/images/theme-search-view-5.png "theming-search-view-5")

_I'm gonna commit this here and just see how it looks._

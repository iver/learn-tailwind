<div align="center">

![tailwind-css-logo](https://user-images.githubusercontent.com/194400/174442927-3476e0a5-eca7-43fd-b68c-5a3f3248e1f8.svg)

Learn 
**`Tailwind CSS`** 
to craft 
**pixel-perfect**
beautifully adaptive 
web apps/sites
in less time.

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dwyl/learn-tailwind/Elixir%20CI?label=build&style=flat-square)](https://github.com/dwyl/learn-tailwind/actions/workflows/ci.yml)
[![codecov.io](https://img.shields.io/codecov/c/github/dwyl/learn-tailwind/main.svg?style=flat-square)](http://codecov.io/github/dwyl/learn-tailwind?branch=main)
[![npm package version](https://img.shields.io/npm/v/tailwindcss.svg?style=flat-square)](https://www.npmjs.com/package/tailwindcss)
[![Hex.pm](https://img.shields.io/hexpm/v/phoenix?color=brightgreen&style=flat-square)](https://hex.pm/packages/phoenix)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)](https://github.com/dwyl/learn-tailwind/issues)
[![HitCount](http://hits.dwyl.com/dwyl/learn-tailwind.svg)](http://hits.dwyl.com/dwyl/learn-tailwind)


</div>
<br />

Use these links to skip stright to the section that interests you:

- [Why?](#why)
  - [Why _switch_ to `Tailwind`?](#why-switch-to-tailwind)
- [What?](#what)
  - [Key Advantages of **`Tailwind`**](#key-advantages-of-tailwind)
  - [`!important` `Tailwind` Eliminates the "Cascade"](#important-tailwind-eliminates-the-cascade)
  - [What about `Tachyons`?](#what-about-tachyons)
  - [What about `XYZ` Framework?](#what-about-xyz-framework)
  - [`Tailwind` in `Phoenix`](#tailwind-in-phoenix)
- [Who?](#who)
- [How?](#how)
  - [Part 1: `Try` _Before_ You `Commit`](#part-1-try-before-you-commit)
    - [Create `index.html`](#create-indexhtml)
  - [Part 2: `Tailwind` in `Phoenix`](#part-2-tailwind-in-phoenix)

# Why?

Many people consider 
[`CSS`](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)
difficult.

![family-guy-css-meme](https://user-images.githubusercontent.com/194400/174753363-aa63871c-97a0-456f-a24c-0c8c1b834602.gif)

> Plenty of memes:
> https://www.google.com/search?q=css+meme&tbm=isch

We think _everyone_ building web apps/sites
should **learn `CSS`**. <br />
However we _agree_ that it can feel frustrating 
and often overwhelming. <br />
Many software engineers/developers
feel they already have _enough_ to learn
with the rest of their chosen 
["stack"](https://github.com/dwyl/technology-stack),
so investing the time 
to perfect the _interface_ design & layout 
feels like too much.
We get it!


Learning **`Tailwind`** 
will not mean 
you don't need to learn/understand `CSS`.
But it will make it 
**a _lot_ easier**.


> We think the infamy of `CSS` is unjustified.
Like learning how to 
[juggle](https://en.wikipedia.org/wiki/Juggling),
you will get hit in the face 
by a few stray objects
in your quest to learn `CSS`.
If you invest the time 
to learn `CSS` from first principals,
you will have the skills
to avoid the frustration.
> As with most things,
it's usually just a matter of _making_ the time 
to learn/understand it.



## Why _switch_ to `Tailwind`? 

We have not taken the decision to "switch"
our UI library _lightly_.
As with all technology decisions,
we _must_ weigh the pros & cons _carefully_
because there is a substantial time investment required.

We feel that the benefits of switching
(outlined below)
justify the cost -
learning time, updating code & maintenance.

We encourage you to read through this doc
and make up your own mind
if `Tailwind` is a good fit 
for you and your team/project.

# What?

**`Tailwind` CSS** 
is a utility-first CSS framework 
that can be composed to build any design, 
directly in your markup. ~
[**tailwindcss.com**](https://tailwindcss.com/)

> Read through their landing page,
> it summarises the benefits very well.

**In-line styles** 
directly in a UI element
so you never have to hunt 
for a style definition across multiple files.
It means you don't suffer 
the change-one thing 
breaks many others pain
of traditional `CSS`.

This is a **_huge_ time saver** 
even in a modest sized project.

## Key Advantages of **`Tailwind`**

1. **_Declarative_ utility focussed `CSS`** classes
   that allow you to **_locally_ scope** 
   all presentation
   and avoid polluting the _global_ space.
2. **Built-in pre-processor bundles** 
   and **_minimises_ your styles**
   so you never ship bloated `CSS` again; 
   _especially_ important for larger projects.
3. **_Actively_ developed** by the original author 
   who is still passionate about the project,
   see: 
   [What's New in `Tailwind` 3](https://www.youtube.com/watch?v=nOQyWbPO2Ds&t=137s&ab_channel=TailwindLabs)
   where the creator 
   [Adam Wathan](https://adamwathan.me) 
   summarises recent improvements.
4. **_Thriving_ community** with _many_ contributors 
   and frequent improvements, 
   see: [github.com/tailwindlabs/tailwindcss](https://github.com/tailwindlabs/tailwindcss)
5. **UI Library** [not free but very reasonably priced!]
   which means there is a **_sustainable_ business model** 
   i.e: it wont cease to be maintained
   because the creator is getting paid to do it full-time.

## `!important` `Tailwind` Eliminates the "Cascade"

One of the most amazing and powerful features 
of `CSS` 
(["**_Cascading_ Style Sheets**"](https://en.wikipedia.org/wiki/CSS))
is also one of the greatest sources 
of _frustration_ when using it in _practice_.
When you have a "cascade",
styles can be applied globally 
to your web site/app
and thus you only have to change 
things in one place
for them to take effect _everwhere_.
In practice this only works when 
everyone editing the `CSS` 
is reasonably proficient 
and there is a clear _system_
for making the changes.

When all styles are **_globally_ scoped**,
making fine adjustments to the position
of a particular UI element becomes tedious
which leads to spagheti code 
full of specificity headaches.
If you see the word
[**`!important`**](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)
in `CSS` you know that
people have given up
on the _maintainability_.


## What about `Tachyons`?

[**`@dwyl`**](https://github.com/dwyl/learn-tachyons/issues/1)
we've been using 
[**`Taychyons`**](https://github.com/tachyons-css/tachyons/#docs)
(Functional CSS Library)
for the past **5 years**
and (as always) 
_comprehensively_
documented our learning in
[dwyl/**learn-tachyons**](https://github.com/dwyl/learn-tachyons)
and 
[dwyl/**tachyons-bootstrap**](https://github.com/dwyl/tachyons-bootstrap).
We still ❤️ it and will use it where it makes sense.
`Taychons` is lightweight (**`14kb`**)
and has _similar_ utility classes to `Tailwind`.

The key diference is `Tachyons` is _just_ the `CSS` 
(_which is great for anywhere 
you **don't want** to have 
build pipeline/process_)
whereas `Tailwind` is a `JavaScript` library
that includs parser/pre-processor.

The _advantage_ of having a `JS` library
means you can create your own
[Functions, Components and Directives](https://tailwindcss.com/docs/functions-and-directives)
that are immensely powerful 
and offer significant flexibility.

`JS` means you are _forced_ 
to have a build step in your dev/deployment pipeline
to use `Tailwind`.
However, given that `Tailwind` works with 
[**`esbuild`**](https://esbuild.github.io/)
(_which is **very fast** and reliable 
and already **included with `Phoenix`**_)
we feel that the trade-off is worth it. 

With `Tailwind` we get the "best of both worlds",
we get a utility-first CSS library,
that also has the flexibility/power 
of a customizable design system.


## What about `XYZ` Framework?

There is a **virtually _endless_ list**
of **`CSS` frameworks**, 
component libraries and pre-processors available. <br />
see: 
[github.com/troxler/**awesome-css-frameworks**](https://github.com/troxler/awesome-css-frameworks) 
... <br />
For a good _comparison_
read:
[athemes.com/collections/**best-css-frameworks**](https://athemes.com/collections/best-css-frameworks/)
or
[dev.to/samlan/**best-css-frameworks-for-2022**-1afm](https://dev.to/samlan/best-css-frameworks-for-2022-1afm)

Ultimately for _us_, 
we did our own research into the available alternatives
but kept an open mind.
We were 
[_guided_](https://github.com/dwyl/technology-stack/issues/94) 
by the 
**`Elixir` / `Phoenix` community** toward **`Tailwind`**
and we have not been disapointed.



## `Tailwind` in `Phoenix`

There are already _official_ instructions 
in the **`Tailwind` docs** for including it in **`Phoenix`**:
[tailwindcss.com/docs/guides/**phoenix**](https://tailwindcss.com/docs/guides/phoenix)

It looks likely **`Tailwind`** will be _included_
in a **_future_ `Phoenix` release** ... 🔮 <br />

At this point **`2022-06-21`** it is _speculation_,
because there is no 
[**`public` roadmap**](https://github.com/dwyl/product-roadmap)
for **`Phoenix`**. 🤷‍♀️ <br />
However given that 
[**Chris McCord**](https://github.com/chrismccord)
_creator_ of 
[**`Phoenix`**](https://www.phoenixframework.org/)
is _actively_
working on an **_official_
`Tailwind` package** for **`Phoenix`**:
[github.com/**phoenixframework/tailwind**](https://github.com/phoenixframework/tailwind)
and is _using_ it at his 
["day job"](https://github.com/dwyl/learn-devops/issues/72#issuecomment-917442712)
building the 
[Fli.io dashboard](https://github.com/dwyl/technology-stack/issues/87#issuecomment-1161649391),
we take this as very good sign.

Also, the fact that 
[Milligram](https://github.com/milligram/milligram),
the _current_ default `CSS` library
[included with `Phoenix@1.6.x`](https://github.com/phoenixframework/phoenix/blob/e0991bb3eea1fd397a898bc2640e3efd72b065c0/installer/templates/phx_static/phoenix.css#L5)
was 
[last updated **2 years** ago ...](https://github.com/dwyl/technology-stack/issues/94#issue-1261227465)
_suggests_ that it will be replaced at some point.

<br />


# Who?

This guide is aimed at anyone
that:

**A.** Wants to **_evaluate_ `Tailwind`** for themselves
or their team without the hype/noise. <br />
**B.** Needs to **learn `Tailwind`**
as **_fast_ as possible**
but without skipping any steps! <br />
**C.** Has to **_summarise_ & _share_**
their knowledge of `Tailwind`
with a team/community of people.

> If you find this useful,
please ⭐ on GitHub
to let us and others know. 
Thanks! 🙏

# How? 

If you just want to test
`Tailwind` with the least effort,
use the online playground:
[play.tailwindcss.com](https://play.tailwindcss.com/)

![tailwind-play-color-change](https://user-images.githubusercontent.com/194400/174629457-cda42165-8242-4f04-afe1-8d7c75da6c2b.gif)


Speed-read through the docs: 
[tailwindcss.com/**docs/utility-first**](https://tailwindcss.com/docs/utility-first)
and try a changing a few values,
e.g: start by changing color names.

## Part 1: `Try` _Before_ You `Commit` 

The _official_
[**get started guide**](https://tailwindcss.com/docs/installation)
instructs you to perform several setup (installation) steps 
***`before`***
you try the framework. 
But you can skip these steps
if you just want to _evaluate_ it.

### Create `index.html`

Create an `index.html` file 
on your computer 
with the following contents:

```html

```

> **Note**: 


<br />

## Part 2: `Tailwind` in `Phoenix`

To run the _finished_ version of our 
**`Tailwind` + `Phoenix` _Demo_**,
run:

```sh
git clone git@github.com:dwyl/learn-tailwind.git && cd learn-tailwind
mix setup
mix 
```


### Build Log


Create a _barebones_ Phoenix App:
```sh
mix phx.new app --no-mailer --no-dashboard --no-gettext --no-ecto
```

Install the dependencies.
Then open the project in your editor.

Run the app:
```
mix phx.server
```

You should see output similar to the following in your terminal:
```sh
Generated app app
[info] Running AppWeb.Endpoint with cowboy 2.9.0 at 127.0.0.1:4000 (http)
[info] Access AppWeb.Endpoint at http://localhost:4000
[debug] Downloading esbuild from https://registry.npmjs.org/esbuild-darwin-64/-/esbuild-darwin-64-0.14.29.tgz
[watch] build finished, watching for changes...
```

That's a good sign, `esbuild` was downloaded
and the assets were compiled successfully.

Visit 
[`localhost:4000`](http://localhost:4000) 
from your browser.

You should see something similar to the following 
(default `Phoenix` homepage):

![phoenix-default-homepage](https://user-images.githubusercontent.com/194400/174807257-34120dc5-723e-4b2c-9e8e-4b6f3aefca14.png)




We're already using `Tailwind` for our `Phoenix LiveView` Chat Example:
https://github.com/dwyl/phoenix-liveview-chat-example

![liveview-chat-with-tailwind-css](https://user-images.githubusercontent.com/194400/174119023-bb83f5f4-867c-4bfa-a005-26b39c700137.gif)

We think it's _siiiiiiick_!
So we'll be writing up our notes soon.
⭐ / 👀 the repo for updates. 

---
title: getLastChecked
slug: Mozilla/Add-ons/WebExtensions/API/captivePortal/getLastChecked
tags:
  - API
  - Add-ons
  - Extensions
  - Non-standard
  - Reference
  - WebExtensions
  - captivePortal
translation_of: Mozilla/Add-ons/WebExtensions/API/captivePortal/getLastChecked
---
<div>{{AddonSidebar()}}</div>

<p>Retourne le temps écoulé depuis que la dernière demande a été complétée.</p>

<h2 id="Syntaxe">Syntaxe</h2>

<pre class="brush: js">var state = browser.captivePortal.getLastChecked()
</pre>

<h3 id="Valeur_retournée">Valeur retournée</h3>

<p>Une <a href="/fr/docs/Web/JavaScript/Reference/Objets_globaux/Promise">Promise</a> qui est remplie avec un nombre entier représentant le temps en millisecondes.</p>

<p>{{WebExtExamples}}</p>

<h2 id="Compatibilité_du_navigateur">Compatibilité du navigateur</h2>

<p>{{Compat("webextensions.api.captivePortal.getLastChecked")}}</p>

<div class="hidden">
<pre>// Copyright 2015 The Chromium Authors. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * Neither the name of Google Inc. nor the names of its
// contributors may be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
</pre>
</div>
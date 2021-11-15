---
title: tabs.reload()
slug: Mozilla/Add-ons/WebExtensions/API/tabs/reload
tags:
  - API
  - Add-ons
  - Extensions
  - Méthode
  - Non-standard
  - Reference
  - WebExtensions
  - reload
  - tabs
translation_of: Mozilla/Add-ons/WebExtensions/API/tabs/reload
---
<div>{{AddonSidebar()}}</div>

<p>Rechargez un onglet, en contournant éventuellement le cache Web local.</p>

<p>C'est une fonction asynchrone qui renvoie une <code><a href="/fr/docs/Web/JavaScript/Reference/Objets_globaux/Promise">Promise</a></code>.</p>

<h2 id="Syntaxe">Syntaxe</h2>

<pre class="brush: js">var reloading = browser.tabs.reload(
  tabId,            // optional integer
  reloadProperties  // optional object
)
</pre>

<h3 id="Paramètres">Paramètres</h3>

<dl>
 <dt><code>tabId</code>{{optional_inline}}</dt>
 <dd><code>integer</code>. L'ID de l'onglet à recharger. Par défaut à l'onglet sélectionné de la fenêtre en cours.</dd>
 <dt><code>reloadProperties</code>{{optional_inline}}</dt>
 <dd><p><code>object</code>.</p>
 <dl>
  <dt><code>bypassCache</code>{{optional_inline}}</dt>
  <dd><code>boolean</code>. Contourner le cache web local. La valeur par défaut est <code>false</code>.</dd>
 </dl>
 </dd>
</dl>

<h3 id="Valeur_retournée">Valeur retournée</h3>

<p>Une <code><a href="/fr/docs/Web/JavaScript/Reference/Objets_globaux/Promise">Promise</a></code> qui sera remplie sans arguments lorsque l'onglet a été rechargé. Si une erreur se produit, la promesse sera rejetée avec un message d'erreur.</p>

<h2 id="Exemples">Exemples</h2>

<p>Recharger l'onglet actif de la fenêtre en cours :</p>

<pre class="brush: js">browser.tabs.reload();</pre>

<p>Rechargez l'onglet actif de la fenêtre en cours, en ignorant le cache :</p>

<pre class="brush: js">browser.tabs.reload({bypassCache: true});</pre>

<p>Rechargez l'onglet dont l'ID est 2, en ignorant le cache et en appelant un rappel lorsque vous avez terminé :</p>

<pre class="brush: js">function onReloaded() {
  console.log(`Reloaded`);
}

function onError(error) {
  console.log(`Error: ${error}`);
}

var reloading = browser.tabs.reload(2, {bypassCache: true});
reloading.then(onReloaded, onError);</pre>

<p>{{WebExtExamples}}</p>

<h2 id="Compatibilité_du_navigateur">Compatibilité du navigateur</h2>

<p>{{Compat("webextensions.api.tabs.reload")}}</p>

<div class="note"><p><strong>Note :</strong></p>

<p>Cette API est basée sur l’API <a href="https://developer.chrome.com/extensions/tabs#method-executeScript"><code>chrome.tabs</code></a> de Chromium. Cette documentation est dérivée de <a href="https://chromium.googlesource.com/chromium/src/+/master/chrome/common/extensions/api/tabs.json"><code>tabs.json</code></a> dans le code de Chromium code.</p>

<p>Les données de compatibilité relatives à Microsoft Edge sont fournies par Microsoft Corporation et incluses ici sous la licence Creative Commons Attribution 3.0 pour les États-Unis.</p>
</div>

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
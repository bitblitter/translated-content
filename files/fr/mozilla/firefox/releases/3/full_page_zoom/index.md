---
title: Zoom pleine page
slug: Mozilla/Firefox/Releases/3/Full_page_zoom
translation_of: Mozilla/Firefox/Releases/3/Full_page_zoom
original_slug: Zoom_pleine_page
---
<div>{{FirefoxSidebar}}</div><p>{{ Gecko_minversion_header(1.9) }}</p>

<p>Le zoom pleine page (ou fullZoom) est une nouvelle fonctionnalité qui sera probablement disponible dans <a href="fr/Firefox_3_pour_les_d%c3%a9veloppeurs">Firefox 3</a>. Elle peut être utilisée dans les compilations courantes du tronc depuis la version 1.9a7. Bien qu'il n'y ait actuellement aucune interface utilisateur visible, il est possible d'utiliser JavaScript et l'interface <a href="fr/XPCOM">XPCOM</a> <a href="http://www.xulplanet.com/references/xpcomref/ifaces/nsIMarkupDocumentViewer.html">nsIMarkupDocumentViewer</a>.</p>

<h3 id="Exemple_.28xul:browser.29">Exemple (xul:browser)</h3>

<p>L'exemple qui suit montre l'utilisation du zoom pour la fenêtre de navigation ayant actuellement le focus. C'est l'utilisation typique pour une extension Firefox.</p>

<pre>var zoom = 1.5;
var docViewer = getBrowser().mCurrentBrowser.markupDocumentViewer;
docViewer.fullZoom = zoom;
</pre>

<h3 id="Exemple_.28xul:iframe.29">Exemple (xul:iframe)</h3>

<p>Il est également possible d'utiliser la fonction fullZoom pour un xul:iframe. Cependant, comme un iframe n'a pas de propriété <code>markupDocumentViewer</code>, il faut d'abord obtenir cette valeur :</p>

<pre>var zoom = 1.5;
var iframe = document.getElementById("authorFrame");
var contViewer = iframe.docShell.contentViewer;
var docViewer = contViewer.QueryInterface(Components.interfaces.nsIMarkupDocumentViewer);
docViewer.fullZoom = zoom;
</pre>

<h3 id="R.C3.A9f.C3.A9rences">Références</h3>

<ul>
 <li>Extension Page zoom par Ted Mielczarek <a href="http://ted.mielczarek.org/code/mozilla/fullpagezoom.xpi">fullpagezoom.xpi</a> pour les dernières nightlies de Firefox 3.</li>
 <li>Le <a class="link-https" href="https://bugzilla.mozilla.org/show_bug.cgi?id=4821">bug</a> concernant fullZoom sur bugzilla.</li>
 <li>Documentation de l'interface <a href="http://www.xulplanet.com/references/xpcomref/ifaces/nsIMarkupDocumentViewer.html">nsIMarkupDocumentViewer</a> (ne mentionne pas fullZoom pour l'instant).</li>
</ul>
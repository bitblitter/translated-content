---
title: Firefox 1.5 pour les développeurs
slug: Mozilla/Firefox/Releases/1.5
tags:
  - Firefox
  - Firefox 1.5
translation_of: Mozilla/Firefox/Releases/1.5
original_slug: Mozilla/Firefox/Versions/1.5
---
<div>{{FirefoxSidebar}}</div><p>Firefox 1.5, basé sur le moteur <a href="/fr/Gecko">Gecko</a> 1.8, améliore son support des standards déjà de premier ordre et fournit de nouvelles opportunités de créer la prochaine génération d'applications Web. Firefox 1.5 propose un support amélioré de CSS2 et CSS3, des API pour des graphiques 2D scriptables et programmables grâce à <a href="/fr/SVG">SVG</a> 1.1 et <code>&lt;canvas&gt;</code>, les évènements <a href="/fr/XForms">XForms</a> et XML, ainsi que de nombreuses améliorations du DHTML, du JavaScript et du DOM.</p>

<h2 id="Outils_pour_d.C3.A9veloppeurs">Outils pour développeurs</h2>

<p>Plusieurs outils et extensions sont disponibles pour aider les développeurs à travailler avec Firefox 1.5.</p>

<ul>
 <li>L'<a href="/fr/Inspecteur_DOM">Inspecteur DOM</a>, un outil permettant aux développeurs d'examiner et de transformer les documents sans avoir à les modifier directement. L'inspecteur DOM est disponible lors de l'installation de Firefox 1.5 dans les options d'installation personnalisée, en choisissant les outils de développement.</li>
 <li>La console JavaScript, un outil permettant d'écrire et tester du code JavaScript, ainsi que d'afficher les erreurs JavaScript et CSS d'une page.</li>
 <li>L'affichage du code source d'une page avec coloration syntaxique et recherche intégrée.</li>
 <li>Des <a class="link-https" href="https://addons.mozilla.org/extensions/showlist.php?application=firefox&amp;category=Developer%20Tools">extensions</a> comme <a href="http://www.joehewitt.com/software/firebug/">Firebug</a>, <a href="/fr/Extension_Firefox_Web_Developer_(externe)">la barre d'outils Web Developer</a>, <a href="/fr/Live_HTTP_Headers_(externe)">Live HTTP Headers</a>, <a href="/fr/Validateur_HTML_en_français_(externe)">un validateur HTML</a>, <a href="/fr/Extension_Developer's_Extension_(externe)">une extension pour les développeurs d'extensions</a> et bien d'autres.</li>
</ul>

<p><strong>Note :</strong> Certaines extensions ne sont pas encore supportées par Firefox 1.5 et seront automatiquement désactivées.</p>

<h2 id="Fonctionnalit.C3.A9s">Fonctionnalités</h2>

<p>Voici certaines des nouvelles fonctionnalités de Firefox 1.5 :</p>

<h3 id="Site_Web_et_d.C3.A9veloppeurs_d.27applications">Site Web et développeurs d'applications</h3>

<dl>
 <dt><a href="/fr/Introduction_à_SVG_dans_HTML">Introduction à SVG dans HTML</a></dt>
 <dd>Apprenez à utiliser le SVG dans des pages XHTML et comment JavaScript et CSS sont utilisés pour manipuler une image comme vous le feriez avec le XHTML dans un script. Voir également <a href="/fr/SVG_dans_Firefox">SVG dans Firefox</a> pour connaître l'état et les problèmes connus de l'implémentation du SVG dans la version 1.5.</dd>
</dl>

<dl>
 <dt><a href="/fr/Dessiner_avec_canvas">Dessiner avec canvas</a></dt>
 <dd>Apprenez à utiliser la nouvelle balise <code>&lt;canvas&gt;</code> et comment dessiner des graphiques et d'autres objets dans Firefox.</dd>
</dl>

<dl>
 <dt><a href="/fr/Colonnes_CSS3">Colonnes CSS3</a></dt>
 <dd>Apprenez à utiliser le nouveau support de mise en page multi-colonnes automatiques comme proposé par CSS3.</dd>
</dl>

<dl>
 <dt><a href="/fr/Utilisation_du_cache_de_Firefox_1.5">Utilisation du cache de Firefox 1.5</a></dt>
 <dd>Découvrez <code>bfcache</code> et comment il accélère la navigation en arrière et en avant.</dd>
</dl>

<h3 id="XUL_et_d.C3.A9veloppeurs_d.27extension">XUL et développeurs d'extension</h3>

<dl>
 <dt><a href="/fr/Construire_une_extension">Construire une extension</a></dt>
 <dd>Ce tutoriel vous guidera par étape dans la création d'une extension très simple pour Firefox. Consultez également <a href="http://kb.mozillazine.org/Getting_started_with_extension_development">un autre tutoriel sur la base de connaissance de MozillaZine</a> qui montre comment il est encore plus simple de créer une nouvelle extension avec les nouvelles fonctionnalités du gestionnaire d'extensions dans 1.5.</dd>
</dl>

<dl>
 <dt><a href="/fr/XPCNativeWrapper">XPCNativeWrapper</a></dt>
 <dd><code>XPCNativeWrapper</code> est un moyen pour empaqueter un objet afin qu'il puisse <a href="/fr/Accès_sécurisé_au_contenu_DOM_depuis_le_chrome">accéder à des privilèges chrome</a>. Il peut être utilisé dans toutes les versions de Firefox bien que son comportement soit sensiblement différent au lancement de Firefox 1.5 (Gecko 1.8).</dd>
</dl>

<dl>
 <dt><a href="/fr/Système_de_préférences">Système de préférences</a></dt>
 <dd>Apprenez à utiliser les nouveaux composants graphiques qui vous permettront de créer des fenêtres d'options plus facilement en utilisant moins de code JavaScript.</dd>
</dl>

<dl>
 <dt><a href="/fr/Caractères_internationaux_dans_du_JavaScript_XUL">Caractères internationaux dans du JavaScript XUL</a></dt>
 <dd>Les fichiers JavaScript XUL peuvent maintenant contenir des caractères non-ASCII.</dd>
</dl>

<dl>
 <dt><a href="/fr/Modifications_du_composant_graphique_tree">Modifications de l'API Tree</a></dt>
 <dd>Les interfaces pour accéder aux éléments XUL <code>&lt;tree&gt;</code> ont été modifiées.</dd>
</dl>

<dl>
 <dt><a href="/fr/Modifications_XUL_pour_Firefox_1.5">Modifications XUL pour Firefox 1.5</a></dt>
 <dd>Résumé des modifications du XUL. Consultez également <a href="/fr/Adaptation_des_applications_XUL_pour_Firefox_1.5">Adaptation des applications XUL pour Firefox 1.5</a>.</dd>
</dl>

<h2 id="Nouvelles_fonctionnalit.C3.A9s_pour_l.27utilisateur">Nouvelles fonctionnalités pour l'utilisateur</h2>

<h3 id="Utilisation_courante">Utilisation courante</h3>

<ul>
 <li><strong>Navigation plus rapide</strong> avec une performance accrue des boutons permettant de reculer ou d'avancer d'une page.</li>
 <li><strong>Réorganisation des onglets par glisser-déposer.</strong></li>
 <li><strong>Le dictionnaire MediaDICO a été ajouté à la liste des moteurs de recherche</strong>.</li>
 <li><strong>Une meilleure prise en main</strong> avec des pages d'erreur descriptives, un menu d'options redessiné, la découverte automatique des fils RSS et un « mode sans échec » plus facile à utiliser.</li>
 <li><strong>Meilleur support de l'accessibilité</strong>, notamment pour les pages DHTML.</li>
 <li><strong>Assistant pour les sites Web non fonctionnels</strong> pour rapporter les sites Web qui ne fonctionnent pas avec Firefox.</li>
 <li><strong>Meilleur support de Mac OS X</strong> (10.2 et supérieur), avec la migration des profils de Safari et d'Internet Explorer pour Mac.</li>
</ul>

<h3 id="S.C3.A9curit.C3.A9_et_vie_priv.C3.A9e">Sécurité et vie privée</h3>

<ul>
 <li><strong>Mises à jour automatiques</strong> pour rationaliser les mises à niveau du navigateur. La notification d'une mise à jour est plus visible et les mises à jour de Firefox n'excèdent plus le demi méga-octet. La mise à jour des extensions a également été améliorée.</li>
 <li><strong>Améliorations du système de blocage de l'ouverture intempestive de fenêtres (popups).</strong></li>
 <li><strong>La fonctionnalité d'effacement des traces</strong> offre un accès simplifié et rapide pour supprimer toutes vos données personnelles via un menu ou un raccourci clavier.</li>
</ul>

<h3 id="Support_des_standards_Web_ouverts">Support des standards Web ouverts</h3>

<p>Le support des standards Web de Firefox garde une longueur d'avance avec des implémentations fonctionnelles et multiplateformes pour :</p>

<ul>
 <li>Hypertext Markup Language (<a href="/fr/HTML">HTML</a>) et Extensible Hypertext Markup Language (<a href="/fr/XHTML">XHTML</a>): <a href="http://www.w3.org/TR/html401/">HTML 4.01</a> et <a href="http://www.w3.org/TR/xhtml1/">XHTML 1.0/1.1</a></li>
 <li>Cascading Style Sheets (<a href="/fr/CSS">CSS</a>): <a href="http://www.w3.org/TR/REC-CSS1">CSS niveau 1</a>, <a href="http://www.w3.org/TR/REC-CSS2">CSS niveau 2</a> et quelques parties de <a href="http://www.w3.org/Style/CSS/current-work.html">CSS niveau 3</a></li>
 <li>Document Object Model (<a href="/fr/DOM">DOM</a>): <a href="http://www.w3.org/TR/2000/WD-DOM-Level-1-20000929/">DOM niveau 1</a>, <a href="http://www.w3.org/DOM/DOMTR#dom2">DOM niveau 2</a> et quelques parties de <a href="http://www.w3.org/DOM/DOMTR#dom3">DOM niveau 3</a></li>
 <li>Mathematical Markup Language: <a href="http://www.w3.org/Math/">MathML Version 2.0</a></li>
 <li>Extensible Markup Language (<a href="/fr/XML">XML</a>): <a href="http://www.w3.org/TR/REC-xml">XML 1.0</a>, <a href="http://www.w3.org/TR/REC-xml-names/">Espaces de nommage sous XML</a>, <a href="http://www.w3.org/TR/xml-stylesheet/">Feuilles de styles associées avec des documents XML 1.0</a>, <a href="http://lists.w3.org/Archives/Public/www-xml-linking-comments/2001AprJun/att-0074/01-NOTE-FIXptr-20010425.htm">Fragment Identifier for XML</a></li>
 <li>XSL Transformations (<a href="/fr/XSLT">XSLT</a>): <a href="http://www.w3.org/TR/xslt">XSLT 1.0</a></li>
 <li>XML Path Language (<a href="/fr/XPath">XPath</a>): <a href="http://www.w3.org/TR/xpath">XPath 1.0</a></li>
 <li>Resource Description Framework (<a href="/fr/RDF">RDF</a>): <a href="http://www.w3.org/RDF/">RDF</a></li>
 <li>Simple Object Access Protocol (SOAP): <a href="http://www.w3.org/TR/SOAP/">SOAP 1.1</a></li>
 <li><a href="/fr/JavaScript">JavaScript</a> 1.6, basé sur <a href="/fr/ECMAScript">ECMA-262</a>, révision 3 : <a href="http://www.ecma-international.org/publications/standards/Ecma-262.htm">ECMA-262</a></li>
</ul>

<p>Firefox 1.5 supporte un bon nombre de protocoles de transport de données (HTTP, FTP, SSL, TLS et d'autres), les caractères multi-langages (Unicode), plusieurs formats graphiques (GIF, JPEG, PNG, SVG et d'autres) et la dernière version du langage de script le plus populaire au monde, <a href="/fr/Nouveautés_dans_JavaScript_1.6">JavaScript 1.6</a>.</p>

<h2 id="Changements_depuis_Firefox_1.0">Changements depuis Firefox 1.0</h2>

<p>De nombreux changements ont été introduits dans Firefox depuis sa première sortie le 9 novembre 2004. Firefox a progressé avec beaucoup de nouvelles fonctions et de corrections de bogues. Une <a href="http://www.squarefree.com/burningedge/releases/1.5-comprehensive.html">liste détaillée des modifications</a> est disponible sur squarefree.com.</p>
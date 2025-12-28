Modern Ken Burns Galéria
Ez egy könnyen implementálható, reszponzív kép-galéria, amely folyamatos közelítő (Ken Burns) animációval és elegáns, "glassmorphism" stílusú feliratokkal teszi látványossá a weboldalt.

Jellemzők
Ken Burns Effekt: Automatikus, lassú zoom animáció az aktív képeken a dinamikus látványért.

Glassmorphism Design: Modern, áttetsző, elmosott hátterű (backdrop-filter) felirat-pirulák.

Teljesen Reszponzív: Mobilra optimalizált megjelenés és érintésvezérlés (Swipe támogatás).

Hardveres Gyorsítás: GPU-ra optimalizált CSS animációk a zökkenőmentes futásért.

Interaktív Navigáció: Kattintható nyilak és automatikus lapozás (8 másodpercenként).

Telepítés
Másold be a HTML kódot a weboldalad megfelelő részébe.

Illeszd be a <style> blokkot a CSS fájlodba vagy a HTML <head> részébe.

Helyezd el a <script> részt az oldal alján, a </body> tag előtt.

Testreszabás
Képek és Linkek cseréje
A galéria elemeit a gallery-slide osztályú div-ekben találod:

HTML

<div class="gallery-slide" onclick="window.location.href='IDE_JÖN_A_LINK'">
    <div class="zoom-wrapper">
        <img src="KEP_URL_CIME" alt="Leírás">
    </div>
    <div class="caption">FELIRAT SZÖVEGE</div>
</div>
Animáció sebessége
A JS kód végén az 8000 (ez 8 másodperc) érték átírásával módosíthatod az automata lapozást:

JavaScript

function startTimer() { autoPlayInterval = setInterval(nextSlide, 8000); }

Mobil optimalizálás
A kód tartalmaz egy @media lekérdezést, amely 480px alatti szélességnél automatikusan:

Csökkenti a galéria magasságát.

Kisebbé és középre igazítottá teszi a feliratokat a jobb olvashatóság érdekében.

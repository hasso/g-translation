Google Androidi rakenduste tõlked
=================================

Google'i Androidi binaarrakenduste tõlked eesti keelde. Need on kasutatavad ainult _root_ kasutaja õigustega seadmetes.

Nende tõlgete kasutamiseks tuleb teha järgmist:

1. Kopeeri seadmest `/data/app` (võibolla ka `/system/app`) kaustast vastava rakenduse apk fail arvutisse.

2. Paki apk lahti.

        apktools d google-rakendus-orig.apk

3. Asenda lahti pakitud rakenduses eesti keele failid selles repos olevatega ning paki rakendus uuesti kokku.

        apktools b google-rakendus-orig google-rakendus-tmp.apk

4. Võta oma zip failide mudimise lemmikrakendus ning liiguta `resources.arsc` fail `google-rakendus-tmp.apk` arhiivist
`google-rakendus-orig.apk` arhiivi (apk failid on tegelikult zip arhiivid).

5. Kopeeri `google-rakendus-orig.apk` tagasi seadmesse õigesse kohta.


Estonian translations for Google Android binary apps
====================================================

These are estonian translations for Google Android binary apps (ie the ones not distributed with AOSP).

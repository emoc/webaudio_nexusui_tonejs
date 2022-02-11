# Exemples web-audio avec NexusUI et Tone.js

NexusUI est une bibliothèque javascript d'éléments d'interfaces adaptés à la musique électronique (contrôle d'enveloppe, séquenceur, «potard», surface de contrôle 2D, etc.).  
Tone.js est un framework complet pour la synthèse et la composition musicale qui simplifie l'accès à la webaudio API.  

Cette série d'exemple met ces deux briques en pratique pour construire des instruments dans le navigateur.

Exemples réalisés avec NexusUI 2.1.6 et Tone.js 14.7.39

![Éléments de NexusUI](./assets/nexus_ui_elements.png?0)  
 ([elements_nexusui.html](./elements_nexusui.html))

## Description des exemples

**01_tone.html**  
_Tone.js, interface en HTML5._  
Exemple minimal!

**02_tone_osc_adsr.html**  
_Tone.js, interface en HTML5._  
Un slider pour varier la fréquence, un trigger pour déclencher la note.

**03_piano.html**  
_Tone.js, NexusUI.js._   
Un clavier type piano, utilisation des évènements de souris pour déclencher l'attaque et la relâche de la note.

**04_piano_polyphonie.html**  
_Tone.js, NexusUI.js._  
Un clavier type piano, polyphonique. N'importe quel synthé monophonique peut-être utilisé pour définir les différentes voix ((AMSynth, DuoSynth, FMSynth, MembraneSynth, MetalSynth, MonoSynth, Synth)). La polyphonie permet d'utiliser 32 voix simultanément maximum.  

**05_sequenceur.html**  
_Tone.js, NexusUI.js._  
Avec séquence préchargée et contrôle du BPM

![05_grains](./assets/05_sequenceur.png?1)

**06_sequenceur_avec_samples.html**  
_Tone.js, NexusUI.js._  
Séquence préchargée, samples et contrôle du BPM

**07_position.html**  
_Tone.js, NexusUI.js._  
Le Pad XY contrôle les paramètres du filtre.

**08_panoramique_mixage.html**  
_Tone.js, NexusUI.js._  
Utilisation de slider et pan pour placer deux sons dans l'espace stéréo.

**09_grains.html**  
_Tone.js, NexusUI.js._  
Lecture de petites boucles avec oscilloscope et spectrogramme.
![09_grains](./assets/09_grains.png?1)

**10_sequence.html**  
_Tone.js, interface en HTML5._
Composition musicale avec des sons de synthèse et des structures proposées par Tone.js

**accompagnement**  
_Tone.js, NexusUI.js._
COMPLETER AVEC VOLUME
Plusieurs éléments d'interface pour contrôler une application d'accompagnement (idée : [Christophe Corbi](http://brettl.fr)).
![accompagnement](./assets/accompagnement.png?1)

**webmidi_tone_nexus**  
_Tone.js, NexusUI.js, Webmidi.js._  
Adaptation vite-fait-mal-fait d'un exemple de l'API Tone.js pour utiliser un clavier connecté en webmidi.
![webmidi_tone_nexus](./assets/test_webmidi.png?0)  

**elements_nexusui.html**
_NexusUI.js, WebAudioAPI._  
Tous les éléments d'interface de NexusUI avec les données captées (visibles sur la console JS).  
(Image ci-dessus)

## Ressources

### Tone.js
  * Dépôt : https://github.com/Tonejs/Tone.js
  * Doc de l'API : https://tonejs.github.io/docs/
  * Exemples : https://tonejs.github.io/examples/
  * Notions : https://github.com/Tonejs/Tone.js/wiki
  * Presets : https://github.com/Tonejs/Presets
  * Echantillons : https://github.com/Tonejs/audio
  * Encore des échantillons! https://github.com/nbrosowsky/tonejs-instruments
  * https://github.com/scraggo/tone-rhythm

### NexusUI.js
  * Intro : http://nexus-js.github.io/ui/
  * Dépôt : https://github.com/nexus-js/ui/
  * API : http://nexus-js.github.io/ui/api/
  * D'autres exemples sont fournis avec le paquet du dépôt
  * Construction de l'interface par OSC : https://github.com/triss/duplex-nexus-osc

### Web Audio API
  * https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API
  * https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API/Using_Web_Audio_API
  * tous les exemples : https://github.com/mdn/webaudio-examples
  * support dans les navigateurs : https://caniuse.com/audio-api
  * specs : https://webaudio.github.io/web-audio-api/  /  https://www.w3.org/TR/webaudio/

### Web MIDI API
  * https://www.w3.org/TR/webmidi/
  * https://developer.mozilla.org/en-US/docs/Web/API/Web_MIDI_API
  * Webmidi.js : https://webmidijs.org/

**Des informations très techniques et cruciales sur l'utilisation des ressources par la web audio API :** http://padenot.github.io/web-audio-perf/

## Plus de ressources

### Exemples Tone.js + Nexus UI  
  * Tim Moore simple synth
    * https://timmoore.github.io/simple-synth/
    * https://github.com/TimMoore/simple-synth
  * Autotel MS Compose 95
    * code : https://github.com/autotel/MsCompose95
    * app : https://autotel.co/mscompose95/
  * deskJocki : https://github.com/bryanhclark/deskJocki synth / bass / drum sequencer
  * https://github.com/OceanSwift/ToneJsSynthTemplate synthé complet avec effets
  * https://github.com/anselbobrow/Tonejs-and-NexusUI visualisation de formes d'onde
  * https://github.com/mariobrubio/PUJSynth synthé classique
  * https://github.com/MikhaelOP9/WebAudioSynth synthé complet
  * https://github.com/nmwenz90/Nate-s-SoundBoard-Project soundboard, lecteur de sample avec oscillo

### Encore ?

Quelques liens d'autres exemples pour compléter

**Nexus UI + WebPD**  
  * https://github.com/taylorbf/NexusUI-WebPD
  * http://taylorbf.github.io/NexusUI-WebPD/basic/

**Ressources Tone.js**
  * https://www.guitarland.com/MusicTheoryWithToneJS/TonejsSetup.html
  * exemple très complet : https://github.com/nielsenjared/in-g
  * https://www.guitarland.com/MusicTheoryWithToneJS/TonejsSetup.html
  * http://sites.music.columbia.edu/cmc/courses/g6611/spring2018/week3/index.html
  * https://pdm.lsupathways.org/3_audio/
  * Web MIDI and Tone.js : https://codepen.io/Chmood/details/XKoPZq
  * https://github.com/tambien/Piano
  * https://groups.google.com/g/tonejs

**Musique algorithmique**
  * https://junshern.github.io/algorithmic-music-tutorial/
  * https://compform.net/music/

**Demo Tone.js**
  * https://www.maxlaumeister.com/tonematrix/
  * http://www.unseen-music.com/yume/ paysage + mix temps réel

**Tone.js + p5.js**
  * https://p5js.org/assets/p5_featured/maya-dulynoted/

**Émulation d'un Juno60**
  * https://pendragon-andyh.github.io/junox/
  * https://github.com/pendragon-andyh/junox




Février 2022.

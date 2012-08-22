イベントの伝播について
propagation

elem.addEventListener(***, ***, true);
にするとelem以下の子孫要素のイベントは全てこの処理に吸収される。

event.stopPropagation()でイベントの伝播を防ぐ
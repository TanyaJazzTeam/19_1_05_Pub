---
title: Block Zitate
syntax-id: Block Zitate
syntax-summary: "> Blockquote"
description: Um ein Blockzitat zu erstellen, fügen Sie vor einem Absatz ein „>“ ein.
examples:
  - markdown: "> Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses."
  html: "<blockquote><p>Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses.</p></blockquote>"
additional-examples:
  - name: Blockzitate mit mehreren Absätzen
  description: Blockzitate können mehrere Absätze enthalten. Fügen Sie in den Leerzeilen zwischen den Absätzen ein „>“ ein.
  markdown: |2

    > Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses.

    >

    > Die Hexe befahl ihr, die Töpfe und Kessel zu reinigen, den Boden zu fegen und das Feuer mit Holz zu versorgen.
  html: "<blockquote><p>Dorothy folgte ihr durch viele der schönen Räume ihres Schlosses.</p><p>Die Hexe befahl ihr, die Töpfe und Kessel zu reinigen, den Boden zu fegen und das Feuer mit Holz zu versorgen.</p ></blockquote>"
  - name: Verschachtelte Blockzitate
  description: Blockzitate können verschachtelt werden. Fügen Sie vor dem Absatz, den Sie verschachteln möchten, ein „>>“ ein.
  markdown: |2

    > Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses.

    >

    >> Die Hexe befahl ihr, die Töpfe und Kessel zu reinigen, den Boden zu fegen und das Feuer mit Holz zu versorgen.
  html: "<blockquote><p>Dorothy folgte ihr durch viele der schönen Räume ihres Schlosses.</p><blockquote><p>Die Hexe befahl ihr, die Töpfe und Kessel zu reinigen, den Boden zu fegen und das Feuer mit Holz zu versorgen. </p></blockquote></blockquote>"
  - name: Blockzitate mit anderen Elementen
  description: Blockquotes können andere Markdown-formatierte Elemente enthalten. Es können nicht alle Elemente verwendet werden – Sie müssen experimentieren, um herauszufinden, welche funktionieren.
  markdown: |2

    > ### Die Quartalsergebnisse sehen großartig aus!

    >

    >   - Der Umsatz lag außerhalb des Diagramms.

    >   - Die Gewinne waren höher als je zuvor.

    >

    > *Alles* läuft nach **Plan**.
  html: "<blockquote><h3>Die Quartalsergebnisse sehen großartig aus!</h3><ul><li>Der Umsatz war außergewöhnlich.</li><li>Die Gewinne waren höher als je zuvor.</li></ul>< p><em>Alles</em> läuft nach <strong>Plan</strong>.</p></blockquote>"
---

Um ein Blockzitat zu erstellen, fügen Sie vor einem Absatz ein `>` ein.

```
> Dorothy followed her through many of the beautiful rooms in her castle.
```

Die gerenderte Ausgabe sieht folgendermaßen aus:

> Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses.

### Blockzitate mit mehreren Absätzen

Blockzitate können mehrere Absätze enthalten. Fügen Sie in den Leerzeilen zwischen den Absätzen ein `>` ein.

```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

Die gerenderte Ausgabe sieht folgendermaßen aus:

> Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses.
>
> Die Hexe befahl ihr, die Töpfe und Kessel zu reinigen, den Boden zu fegen und das Feuer mit Holz zu versorgen.

### Verschachtelte Blockzitate

Blockzitate können verschachtelt werden. Fügen Sie vor dem Absatz, den Sie verschachteln möchten, ein `>>` ein.

```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

Die gerenderte Ausgabe sieht folgendermaßen aus:

> Dorothy folgte ihr durch viele der wunderschönen Räume ihres Schlosses.
>
> > Die Hexe befahl ihr, die Töpfe und Kessel zu reinigen, den Boden zu fegen und das Feuer mit Holz zu versorgen.

### Blockzitate mit anderen Elementen

Blockquotes können andere Markdown-formatierte Elemente enthalten. Es können nicht alle Elemente verwendet werden – Sie müssen experimentieren, um herauszufinden, welche funktionieren.

```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
```

Die gerenderte Ausgabe sieht folgendermaßen aus:

> <h4 class="no-anchor">Die Quartalsergebnisse sehen großartig aus!</h4>
>
> - Der Umsatz lag außerhalb des Diagramms.
> - Die Gewinne waren höher als je zuvor.
>
> *Alles* läuft nach **Plan** .

### Best Practices für Blockquotes

Fügen Sie aus Kompatibilitätsgründen Leerzeilen vor und nach Blockzitate ein.

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅ Tun Sie dies</th>
      <th>❌Tu das nicht</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
        Try to put a blank line before...&lt;br&gt;&lt;br&gt;
        &gt; This is a blockquote&lt;br&gt;&lt;br&gt;
        ...and after a blockquote.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        Without blank lines, this might not look right.&lt;br&gt;
        &gt; This is a blockquote&lt;br&gt;
        Don't do this!
        </code>
      </td>
    </tr>
  </tbody>
</table>

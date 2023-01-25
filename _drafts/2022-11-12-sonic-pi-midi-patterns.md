---
layout: post
title: Generating MIDI patterns with Sonic-Pi
category: audio
tags: sonic-pi linux-audio
date: '2022-11-12 13:16'
patat:
    wrap: false
    margins:
        left: 20
        right: 20
        top: 20
        bottom: 20
    incrementalLists: true
    theme:
      syntaxHighlighting:
        decVal: [rgb#b3122f]
      borders: [vividMagenta]
      definitionTerm: [vividRed]
      header: [vividGreen]
      codeBlock: [onDullWhite]
      imageText: [onDullWhite, vividRed]
    images:
      backend: kitty
    pandocExtensions:
      - patat_extensions
      - autolink_bare_uris
      - emoji
...

# spread

## something
```ruby
| x - - - | x - - - | x - - - | x - - - |

8.times do
  if spread(4, 8).tick
    midi 55, channel: 10, velocity: 80
  end
  sleep 0.5
end
```
. . .
```ruby
| x - - x | x - - x | x - - x | x - - x |

8.times do
  if spread(8, 8).tick
    midi 55, channel: 10, velocity: 80
  end
  sleep 0.5
end
```

. . .

`play 60`

# something
## Patterns

![](preloader.gif)



## Connecting midi ports

* connect midi-thru or rt-midi to hydrogen

# hydrogen

## configure midi input

## create drumkit

### samples

`tp-norm -t -6`

`ecafixdc`

# non-sequencer

# demo

## something
. . .

Legen

. . .

wait for it

. . .

Dary!

# last thing

## a picture

![](../../assets/images/site_header02.png)

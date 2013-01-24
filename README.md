About
=====

The sentences.txt file contains sentences and their translations to multiple languages.

My main focus is to have many Japanese sentences and their translations to English,
and then feed this file to applications that will help me and others learn Japanese.

This just means that there might be more sentences in English and Japanese than other languages.

However, the format of the file is unaware of which languages I know or want to learn,
so it can contain sentences in any language.

Also, the applications I will develop will also work with other languages whenever possible (some applications might be specific to Japanese learning).


Format
======

#### Example

```
JP: 明日、映画館に行くつもりです
EN: Tomorrow, I plan to go to the cinema

JP: 明日、映画を見に行きます
EN: Tomorrow, I will go see a movie
```

#### Formal explanation

A sentence group is a set of sentences where all sentences have the same meaning, independent of the language.

Every sentence in a group belongs in a single line. A blank line separates sentence groups.

Each sentence in a group begins with a language code (EN, JP, PT, etc.) followed by a colon `:`.
This language code tells which language the following sentence is written in.

The language code should have two characters exactly to improve readability.
However, applications shouldn't rely on this.

The order of the sentences in a group and the order of the groups is irrelevant.
Also, a group can have more than one sentence of a given language, as long as their meanings are the same.


Applications
============

There are currently no applications that use this file, but there will be some very soon.


Planned applications
====================

### Anki converter
Given two language codes, for example, JP and EN, converts the file into a Anki deck with each card containing a sentence, where the front of the card has the language from the first language code and the back of the card has the other language.

### Wanikani filter
Filter the file leaving only sentences in English and Japanese. If provided with the user's Wanikani API key, it will also filter sentences if the japanese version of the sentence contains kanji that the user has yet to learn in Wanikani.


Contributing
============

### With sentences

#### Rules

The only rule is, when adding sentences to the file, please be careful where you got them from.
If you just invented them in your head, all's good!
If you took them from a book or the web, please make sure the book/site allows you to use their sentences this way.

For example, if you're thinking of taking sentences from a Japanese learning website,
please ask them whether they allow it, because probably they won't since they had to come up with those sentences
themselves and their business model might depend on those sentences being restricted to their site.

#### How

The preferred method to contribute to the sentences file is to fork this repository,
make the changes to the sentences.txt file, and make a pull request.
While this might look complicated, it is not, just keep reading.

First you have to create an account at github. I'll assume you can handle that without further help.

Do you have an account? Great! Now click the sentences.txt file in this page (scroll up, you should see it easily).
Now click the `Edit` button and start hacking at the file! When you're done write a small explanation of what you did
in the input box labeled `Commit summary` and if you feel the need add an `Extended description` below.

When you're done click `Propose File Change`, and in the next page click `Send pull request` and you're done!

I will then review the changes and add them if I see nothing wrong.
If I think they have a problem that is too cumbersome for me to solve I will refuse to apply the patch and tell you why,
but as long as the sentences and their translations are correct that should not happen.


If you feel this is too hard for you but you still want to contribute, 
you can send me an email with the sentences you want me to add, or the changes for me to make.

But that makes it harder for me to manage the changes,
so please give the former method a try before you send me an email.


### With applications

Anyone is free to implement applications that make use of the sentences.txt file without asking me for permission
or giving me any kind of credit (after all, the file is not just mine, it belongs to the community).

Still, if you write an application, you might want to let me know so I can link to it from this page.

You can also contribute to any application I develop since they all will be open source.
I'd recommend anyone creating applications to make them open source too in order to allow the community
to help in the development, but again, it's not required.

You can also implement applications from the `Planned Applications` section,
just tell me if you're going to do it so I don't repeat your work.
Oh, and again, please make them open source so I can contribute or fork.

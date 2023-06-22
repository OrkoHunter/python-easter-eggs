> Just when you thought, Python could not be more fun.

### 1. Hello World[^hello-world]

```py
>>> import __hello__
Hello World!
>>> import __phello__
Hello world!
```

Hello world for python >= 3.11

```py
>>> import __hello__
>>> __hello__.main()
Hello World!
>>> import __phello__
>>> __phello__.main()
Hello World!
```

### 2. The classic[^the-classic]
```
>>> import this

The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

### 3. The missing line from the classic[^missing-zen]

The Zen of Python was introduced in [PEP 20](https://www.python.org/dev/peps/pep-0020/#id2). It is supposed to be 20 aphorisms, but only 19 of which have been written down.


### 4. A simple life lesson[^import-this]
```py
>>> import this
...
>>> love = this
>>> this is love
True
>>> love is True
False
>>> love is False
False
>>> love is not True or False
True
>>> love is not True or False; love is love  # FML
True
```

### 5. Comics, yeah.[^antigravity]
```py
>>> import antigravity
```

### 6. It's not a choice, it defines who we are[^braces]
```py
>>> from __future__ import braces
  File "<stdin>", line 1
SyntaxError: not a chance
```

### 7. Origins[^origins]
The name Python has nothing to do with the type of Snake.

### 8. The confuscation[^this-py]
This is how the `this.py` module looks, which prints the Zen of Python.

```py
s = """Gur Mra bs Clguba, ol Gvz Crgref

Ornhgvshy vf orggre guna htyl.
Rkcyvpvg vf orggre guna vzcyvpvg.
Fvzcyr vf orggre guna pbzcyrk.
Pbzcyrk vf orggre guna pbzcyvpngrq.
Syng vf orggre guna arfgrq.
Fcnefr vf orggre guna qrafr.
Ernqnovyvgl pbhagf.
Fcrpvny pnfrf nera'g fcrpvny rabhtu gb oernx gur ehyrf.
Nygubhtu cenpgvpnyvgl orngf chevgl.
Reebef fubhyq arire cnff fvyragyl.
Hayrff rkcyvpvgyl fvyraprq.
Va gur snpr bs nzovthvgl, ershfr gur grzcgngvba gb thrff.
Gurer fubhyq or bar-- naq cersrenoyl bayl bar --boivbhf jnl gb qb vg.
Nygubhtu gung jnl znl abg or boivbhf ng svefg hayrff lbh'er Qhgpu.
Abj vf orggre guna arire.
Nygubhtu arire vf bsgra orggre guna *evtug* abj.
Vs gur vzcyrzragngvba vf uneq gb rkcynva, vg'f n onq vqrn.
Vs gur vzcyrzragngvba vf rnfl gb rkcynva, vg znl or n tbbq vqrn.
Anzrfcnprf ner bar ubaxvat terng vqrn -- yrg'f qb zber bs gubfr!"""

d = {}
for c in (65, 97):
    for i in range(26):
        d[chr(i+c)] = chr((i+13) % 26 + c)

print("".join([d.get(c, c) for c in s]))
```

The code for the Zen violates itself. It's not beautiful but ugly, not explicit but implicit.
This would probably be the *only* module to go against the spirit of what it says itself.
.

### 9. C/C++ anyone?[^c-c++]
From the Zen again,
```
There should be one-- and preferably only one --obvious way to do it.
```

### 10. Naming identifiers can be unspeakably cool[^identifiers]
Just when you thought that working in Python couldn't possibly *be* any more fun,
```py
>>> from math import pi
>>> π = pi
>>> area = π * r**2

>>> résumé = 'knows Python'
>>> 'Python' in résumé
True
```

### 11. Picking a place for meetup?[^geohash]
```py
>>> from antigravity import geohash
>>> # Your location, a date and that date's (or most recent) DJIA opening.
>>> geohash(37.421542, -122.085589, b'2005-05-26-10458.68')
37.857713 -122.544543
```
This can generate a GPS coordinate in a region which is 1 longitude long and 1
latitude wide based on your location.

### 12. The FLUFL - Friendly Language Uncle For Life from [PEP 401 -- BDFL Retirement](https://www.python.org/dev/peps/pep-0401)[^pep-401]
```py
>>> from __future__ import barry_as_FLUFL
>>> 1 <> 2
True
>>> 1 != 2
  File "<stdin>", line 1
    1 != 2
       ^
SyntaxError: invalid syntax
```
Recognized that the != inequality operator in Python 3.0 was a horrible, finger pain inducing mistake, the FLUFL reinstates the <> diamond operator as the sole spelling.

### 13. InPynite?[^inpynite]
```py
>>> infinity = float('infinity')
>>> hash(infinity)
314159
>>> hash(float('-inf'))
-314159
```
A hash is a fixed sized integer that identifies a particular value. On a closer look, the hash of infinity is 10^5 x pi. Interestingly, hash(float('-inf')) yields -10^5 x pi in python3, whereas -271828 i.e - 10^5 x e in python2.

### 14. types.CodeType -  Not for the faint of heart
If you start digging deep into Python's internals you will get a warning in `help` output for `types.CodeType`
```py
>>> import types
>>> help(types.CodeType)
...
Help on class code in module builtins:                                                    
                                                                                          
class code(object)                                                                        
 |  code(argcount, kwonlyargcount, nlocals, stacksize, flags, codestring,                 
 |        constants, names, varnames, filename, name, firstlineno,                        
 |        lnotab[, freevars[, cellvars]])                                                 
 |                                                                                        
 |  Create a code object.  Not for the faint of heart.                                    
 |                                                                                        
 |  Methods defined here:                                                                 
 |                                                                                                                                       
 ...
 ```

### 15. Python 3.9 PEG parser[^peg-parser]
`__peg_parser__` is a keyword in python 3.9, will throw a syntax error if used
```py
>>> __peg_parser__
  File "<stdin>", line 1
    __peg_parser__
    ^
SyntaxError: You found it!
```

[^hello-world]: Easiest hello world program in a language without calling any function
[^the-classic]: Each and every line is the philosophy of Python's design and is a supreme holy guide
[^missing-zen]: Maybe just to show that there always should be a new line at the end of a file!
[^import-this]: Not an easter egg, a joke in the interpreter
[^antigravity]: It opens this [xkcd comic](https://xkcd.com/353) which demonstrates how easy it is to do stuff with modules
[^braces]: This is to instantly close down any conversation about introducing curly braces to Python
[^origins]: Guido van Rossum is a big fan of [Monty Python's Flying Circus](https://en.wikipedia.org/wiki/Monty_Python%27s_Flying_Circus)
[^this-py]: It's a substitution cipher called [ROT13](https://en.wikipedia.org/wiki/ROT13)
[^c-c++]: In many languages there are two ways to do the same thing `--no` and `no--`. The message has a hidden example in itself
[^identifiers]: Support for unicode character set for naming identifiers was added in Python3. Though, it is not explicitly preferred while writing code, it adds flavour to working with scientific formulas
[^geohash]: The original code is [here](https://github.com/python/cpython/blob/master/Lib/antigravity.py) with the [xkcd comic](https://xkcd.com/426/) referenced, and maybe that's why this is also in the `antigravity` module
[^pep-401]: The [PEP 401](https://www.python.org/dev/peps/pep-0401/) is an April Fools' Joke - The PEP's number is 401, i.e. 4/01 or April 1st (April Fools' Day). The PEP states that Guido van Rossum is stepping down. The new title given to him would be pronounced "BDEVIL" (Benevolent Dictator Emeritus Vacationing Indefinitely from the Language) and Guido's successor will be Barry Warsaw, or as he is affectionately known, Uncle Barry. Uncle Barry's official title is "FLUFL" (Friendly Language Uncle For Life). There are in-jokes about the Parrot virtual machine and the "non-existent" Python Secret Underground (possibly a throw-back to ["TINC" on USENET](https://en.wikipedia.org/wiki/There_Is_No_Cabal)).
[^inpynite]: [Source](https://www.reddit.com/r/Python/comments/6wrd8t/nice_lil_easter_egg_i_suppose/).
[^peg-parser]: See [this answer](https://stackoverflow.com/a/65487013/14362510)

## Add more

Please feel free to create a PR and add more!

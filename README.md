## Know them all !
> Just when you thought, Python could not be more fun.

### 1. Hello World

```py
>>> import __hello__
Hello World!
```

### 2. The classic
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

### 3. The missing line from the classic

The Zen of Python was introduced in [PEP 20](https://www.python.org/dev/peps/pep-0020/#id2). It is supposed to be 20 aphorisms, but only 19 of which have been written down.


### 4. A simple life lesson
```
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

### 5. Comics, yeah.
```py
>>> import antigravity
```

### 6. It's not a choice, it defines who we are
```py
>>> from __future__ import braces
  File "<stdin>", line 1
SyntaxError: not a chance
```

### 7. Origins
The name Python has nothing to do with the type of Snake.

### 8. The confuscation
This is how the `this.py` module looks, which prints the Zen of Python.

```
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

### 9. C/C++ anyone?
From the Zen again,
```
There should be one-- and preferably only one --obvious way to do it.
```



## Notes
1. Easiest hello world program in a language without calling any function
2. Each and every line is the philosophy of Python's design and is a supreme holy guide
3. Maybe just to show that there always should be a new line at the end of a file!
4. Not an easter egg, a joke in the interpreter
5. It opens this [xkcd comic](https://xkcd.com/353) which demonstrates how easy it is to do stuff with modules
6. This is to instantly close down any conversation about introducing curly braces to Python
7. Guido van Rossum is a big fan of [Monty Python's Flying Circus](https://en.wikipedia.org/wiki/Monty_Python%27s_Flying_Circus)
8. It's a substitution cipher called [ROT13](https://en.wikipedia.org/wiki/ROT13)
9. In many languages there are two ways to do the same thing `--no` and `no--`. The message has a hidden example in itself

## Add more

Please feel free to create a PR and add more!
## Generate a password hash as produced by crypt (C)

![genSHA512 (crypt)](https://github.com/nicholashoule/cryptSHA512/workflows/genSHA512%20(crypt)/badge.svg?branch=master)

[![Run on Repl.it](https://repl.it/badge/github/nicholashoule/cryptSHA512)](https://repl.it/github/nicholashoule/cryptSHA512)

### Compatible with Linux crypt (c).

Crypt, as defined by POSIX, doesn't mandate a specific encryption algorithm hence OSX crypt() isn't compatible with this script.

##### Key derivation functions supported by crypt:

Ref: https://en.wikipedia.org/wiki/Crypt_(C)

| ID             | Schema            | Example                             |
|----------------|-------------------|-------------------------------------|
|  1             | MD5               | $1$etNnh7FA$OlM7eljE/B7F1J4XYNnk81  |
|  2, 2a, 2x, 2y | bcrypt            | $2a$10$VIhIOofSMqgdGlL4wzE//e.77dAQGqntF/1dT7bqCrVtquInWy2qi |
|  3             | NTHASH            | $3$$8846f7eaee8fb117ad06bdd830b7586c |
|  5             | SHA-256           | $5$9ks3nNEqv31FX.F$gdEoLFsCRsn/WRN3wxUnzfeZLoooVlzeF4WjLomTRFD |
|  6             | SHA-512           | $6$qoE2letU$wWPRl.PVczjzeMVgjiA8LLy2nOyZbf7Amj3qLIL978o18gb... |
| md5            | Solaris MD5       | $md5,rounds=5000$GUBv0xjJ$$mSwgIswdjlTY0YxV7HBVm0 |
| sha1           | PBKDF1 with SHA-1 | $sha1$40000$jtNX3nZ2$hBNaIXkt4wBI2o5rsi8KejSjNqIq |

##### python3:

Python 3.3+ includes mksalt in crypt.

##### Run the code:
https://repl.it/@NicholasHoule/pythongenSHA512

Application versioning 1.0.0
========

---

GNT Engineering, 2012
---

[wiki reference](http://en.wikipedia.org/wiki/Software_versioning)

---

Agenda
========
.notes: only for internal purpose
# Version Problems
# Versions - Show cases
# Proposed versioning standard
# Who will be involved?
# How it works?
# Some estimations
# Q&A

---

Version Problems
========

* change control and backward compatibility
* consistency for both internal and external sides
* standardized: all teams using the same method

---

Versions - Show cases
========

* Window 8
* HTML5
* Web 2.0
* iOS 5.1
* Zend 1.11.11
* Microsoft Office 2010
* Adobe Photoshop CS2
* TeX 3.1415926 

How we call Ipad 3: Ipad gen 3 or Ipad 2012?

---

Proposed versioning standard
========

a.b.c.[d]
.notes: 32 bits = 4 bytes

* a: major change: {new UI, change platform, OS, architecture}, external, range: 1-9, 4 bits
* b: minor change: {new feature, bug fixes, enhancements}, external, range: 0-9, 4 bits
* c: internal revision: {accumulated and derived from final build number}, internal, range: 0-9, 4 bits
* d: build number, internal, **not mandatory to display on product info**, svn final revision number, 20 bits

+ Starting point: 0.0.0.0
+ End point: 9.9.9.999999

---
Change attributes
========

* time decay: 6 months for upgrading to 2.0.0, PM/PO define in advance
* number of changes: how many fixes, enhancements, features
* weights/impact score: 1,2,4
* change type:
	* new function: develop new one
	* bug fixes: fix the existing one
	* enhancement: modify to improve one
	* other: none of all above
---
Who will be involved?
========
+ Dev: leader need to commit final build revision => part d
+ QA: check and increase number => parts b :: c :: a
+ PM: confirm parts a.b.c
+ PO: approve version a.b.c

---
How it works?
========

+ Developer subbmited final build version => d
+ Based on d, QA will reckon the c :: b :: a numbers

There are two cases:
* c over threshold 9 => increase b + 1, reset c = 0
* manual increase c

The alternative way for parts a and b.

From version a1.b1.c1, it's possible to jumpt to a2.b2.c2 in accordance to business owner 's request.
 
---
Some estimations
========
* a.b.c => 900 possibilities of release
* release period: 2 weeks

Hence, product version lasting in about ***9 years***.

---
Q&A
========

*Thank you and happy versioning!*

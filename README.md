Bookmarklet: Typogr
===================
This is a bookmarklet that uses components of [Typogr](https://github.com/ekalinin/typogr.js) to typographically enhance sites. All the actual work is done by functions copied straight from Typogr, so I suggest [checking it out](https://github.com/ekalinin/typogr.js)&mdash;it's great.

The functions were extracted into the bookmarklet to not have to load
the two script files (jQuery and Typogr) when running it, and because
we only need these specific goodies.

Usage
-----

Create a new bookmark with the following URL (I can't give you a drag-and-droppable link, because GitHub does not allow JavaScript links):

```
javascript:(function()%7B!function(e%2Ct)%7Bvar%20n%3D%2F%3C(%5C%2F)%3F(pre%7Ccode%7Ckbd%7Cscript%7Cmath%7Ctitle)%5B%5E%3E%5D*%3E%2Fi%3Bvar%20r%3Dfunction(e%2Ct)%7Breturn%20new%20RegExp(e%2Ct)%7D%3Bvar%20i%3Dfunction(e)%7Bvar%20t%3Ds(e)%2Cr%3D%5B%5D%2Ci%3D%5B%5D%2Cc%3D%22%22%2Ch%3D%22%22%2Cp%3Dfalse%2Cd%3D%22%22%2Cv%2Cm%3Bt.forEach(function(e)%7Bif(e.type%3D%3D%3D%22tag%22)%7Br.push(e.txt)%3Bif((h%3Dn.exec(e.txt))!%3D%3Dnull)%7Bc%3Dh%5B2%5D.toLowerCase()%3Bif(h%5B1%5D)%7Bif(i.length%3E0)%7Bif(c%3D%3D%3Di%5Bi.length-1%5D)%7Bi.pop()%7D%7Dif(i.length%3D%3D%3D0)%7Bp%3Dfalse%7D%7Delse%7Bi.push(c)%3Bp%3Dtrue%7D%7D%7Delse%7Bm%3De.txt%3Bv%3Dm.slice(-1)%3Bif(!p)%7Bm%3Do(m)%3Bm%3Du(m)%3Bm%3Da(m)%3Bm%3Df(m)%3Bswitch(m)%7Bcase%22'%22%3Aif(%2F%5CS%2F.test(d))%7Bm%3D%22%26%238217%3B%22%7Delse%7Bm%3D%22%26%238216%3B%22%7Dbreak%3Bcase'%22'%3Aif(%2F%5CS%2F.test(d))%7Bm%3D%22%26%238221%3B%22%7Delse%7Bm%3D%22%26%238220%3B%22%7Dbreak%3Bdefault%3Am%3Dl(m)%7D%7Dd%3Dv%3Br.push(m)%7D%7D)%3Breturn%20r.join(%22%22)%7D%3Bvar%20s%3Dfunction(e)%7Bvar%20t%3D%5B%5D%2Cn%3D0%2Cr%3D%2F(%5B%5E%3C%5D*)(%3C%5B%5E%3E%5D*%3E)%2Fgi%2Ci%3Bwhile((i%3Dr.exec(e))!%3D%3Dnull)%7Bvar%20s%3Di%5B1%5D%2Co%3Di%5B2%5D%3Bif(s)%7Bt.push(%7Btype%3A%22text%22%2Ctxt%3As%7D)%7Dt.push(%7Btype%3A%22tag%22%2Ctxt%3Ao%7D)%3Bn%3Dr.lastIndex%7Dif(r.lastIndex%3C%3De.length)%7Bif(e.slice(-1)%3D%3D%22.%22%26%26e.slice(-2)!%3D%22..%22)%7Bt.push(%7Btype%3A%22text%22%2Ctxt%3Ae.slice(n%2Ce.length-1)%7D)%3Bt.push(%7Btype%3A%22text%22%2Ctxt%3Ae.slice(-1)%7D)%7Delse%7Bt.push(%7Btype%3A%22text%22%2Ctxt%3Ae.slice(n)%7D)%7D%7Dreturn%20t%7D%3Bvar%20o%3Dfunction(e)%7Breturn%20e.replace(%2F%5C%5C%22%2Fg%2C%22%26%2334%3B%22).replace(%2F%5C%5C'%2Fg%2C%22%26%2339%3B%22).replace(%2F%5C%5C-%2Fg%2C%22%26%2345%3B%22).replace(%2F%5C%5C%5C.%2Fg%2C%22%26%2346%3B%22).replace(%2F%5C%5C%5C%5C%2Fg%2C%22%26%2392%3B%22).replace(%2F%5C%5C%60%2Fg%2C%22%26%2396%3B%22)%7D%3Bvar%20u%3Dfunction(e)%7Breturn%20e.replace(%2F---%2Fg%2C%22%26%238212%3B%22).replace(%2F--%2Fg%2C%22%26%238211%3B%22)%7D%3Bvar%20a%3Dfunction(e)%7Breturn%20e.replace(%2F%5C.%5C.%5C.%2Fg%2C%22%26%238230%3B%22).replace(%2F%5C.%20%5C.%20%5C.%2Fg%2C%22%26%238230%3B%22)%7D%3Bvar%20f%3Dfunction(e)%7Breturn%20e.replace(%2F%60%60%2Fg%2C%22%26%238220%3B%22).replace(%2F''%2Fg%2C%22%26%238221%3B%22)%7D%3Bvar%20l%3Dfunction(e)%7Bvar%20t%3D%22%5B!%5C%22%23%5C%5C%24%5C%5C%25%5C%5C'()*%2B%2C-.%5C%5C%2F%3A%3B%3C%3D%3E%3F%5C%5C%40%5C%5C%5B%5C%5C%5C%5C%5D%5C%5C%5E_%60%7B%7C%7D~%5D%22%2Cn%3D%22(%3F%3D%25s%5C%5CB)%22.replace(%22%25s%22%2Ct)%2Ci%3D%22%5B%5E%5C%5C%20%5C%5Ct%5C%5Cr%5C%5Cn%5C%5C%5B%5C%5C%7B%5C%5C(%5C%5C-%5D%22%2Cs%3D%22%26%238211%3B%7C%26%238212%3B%22%2Co%3Dr(%22(%22%2B%22%5C%5Cs%7C%22%2B%22%26nbsp%3B%7C%22%2B%22--%7C%22%2B%22%26%5Bmn%5Ddash%3B%7C%22%2Bs%2B%22%7C%22%2B%22%26%23x201%5B34%5D%3B%22%2B%22)%22%2B%22'%22%2B%22(%3F%3D%5C%5Cw)%22%2C%22g%22)%2Cu%3Dr(%22(%22%2Bi%2B%22)%22%2B%22'%22%2B%22(%3F!%5C%5Cs%20%7C%20s%5C%5Cb%20%7C%20%5C%5Cd)%22%2C%22g%22)%2Ca%3Dr(%22(%22%2Bi%2B%22)%22%2B%22'%22%2B%22(%3F!%5C%5Cs%20%7C%20s%5C%5Cb)%22%2C%22g%22)%2Cf%3Dr(%22(%22%2B%22%5C%5Cs%7C%22%2B%22%26nbsp%3B%7C%22%2B%22--%7C%22%2B%22%26%5Bmn%5Ddash%3B%7C%22%2Bs%2B%22%7C%22%2B%22%26%23x201%5B34%5D%3B%22%2B%22)%22%2B'%22'%2B%22(%3F%3D%5C%5Cw)%22%2C%22g%22)%2Cl%3Dr('%22(%3F%3D%5C%5Cs)'%2C%22g%22)%2Cc%3Dr(%22(%22%2Bi%2B')%22'%2C%22g%22)%3Breturn%20e.replace(r(%22%5E'%25s%22.replace(%22%25s%22%2Cn)%2C%22g%22)%2C%22%26%238217%3B%22).replace(r('%5E%22%25s'.replace(%22%25s%22%2Cn)%2C%22g%22)%2C%22%26%238221%3B%22).replace(%2F%22'(%3F%3D%5Cw)%2Fg%2C%22%26%238220%3B%26%238216%3B%22).replace(%2F'%22(%3F%3D%5Cw)%2Fg%2C%22%26%238216%3B%26%238220%3B%22).replace(%2F%5Cb'(%3F%3D%5Cd%7B2%7Ds)%2Fg%2C%22%26%238217%3B%22).replace(o%2C%22%241%26%238216%3B%22).replace(u%2C%22%241%26%238217%3B%22).replace(a%2C%22%241%26%238217%3B%242%22).replace(%22'%22%2C%22%26%238216%3B%22).replace(f%2C%22%241%26%238220%3B%22).replace(l%2C%22%26%238221%3B%22).replace(c%2C%22%241%26%238221%3B%22).replace('%22'%2C%22%26%238220%3B%22)%7D%3Bt.body.innerHTML%3Di(t.body.innerHTML)%3Balert(%22Dear%20Sir%2C%20I%20have%20typogrified.%20It%20was%20a%20great%20success.%22)%7D(window%2Cdocument)%7D)()
```

Alternatively, you may create your own bookmarklet from `bookmarklet.js`.
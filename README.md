#  Language Modeling with Neural Nets - Multi Layer perceptron

This project builds upon the ideas presented in Xgram to generate something more complex, and in theory, more effective. We are working on adding 1 and 2 layers to a multilayer perceptron to get better accuracy, lower loss, and more real sounding words.

---

##  1 Hidden Layer

Training the data gives us some pretty interesting results. The gradient descent isn't amazing as we tend to jump around a lot, but we are able to get the loss function to the low 2.0/1.9 area at times and upon further training on the test set, we were able to get an accuracy of test 2.2962729930877686! This is amazing loss for data that it was not trained on at all. These were the iterations and the loss (the optimization of the gradient descent is very poor but we are able to get down to a lower number than the bi and trigram models which is a great upgrade.


```
 0/20000: 2.3326010704040527
   1000/20000: 2.448707342147827
   2000/20000: 2.0864596366882324
   3000/20000: 2.294234037399292
   4000/20000: 2.0319528579711914
   5000/20000: 2.281989097595215
   6000/20000: 2.0325756072998047
   7000/20000: 2.071772575378418
   8000/20000: 2.432504415512085
   9000/20000: 2.0393221378326416
  10000/20000: 2.1370689868927
  11000/20000: 2.4032812118530273
  12000/20000: 2.1762139797210693
  13000/20000: 2.2088828086853027
  14000/20000: 2.1537275314331055
  15000/20000: 2.448063373565674
  16000/20000: 2.335707902908325
  17000/20000: 2.1529223918914795
  18000/20000: 2.1583235263824463
  19000/20000: 2.481691598892212
2.1162142753601074
```

Of course there really is no goal loss now. It is of course great to see that the loss is less than the perfect statistical one, but still interesting to see nonetheless. The words that were generated go as follow:


```
unbadid.
audhrinit.
actole.
umprotes.
tite.
fantunnimiolatisnece.
bam.
subeg.
soreb.
nacnongmocogchile.
mocresileaty.
trognenor.
noswuq.
myin.
gxeic.
ung.
brulyo.
nit.
monesud.
ter.
iolinmodetabharigint.
umonkartut.
metuad.
centing.
panminesburcocolionse.
canssph.
```

This is a HUGE improvement in the words. Although the loss function may not be a ton lower, it is great to see such a huge upgrade on this. Let's see if we can get any other upgrades with a second hidden layer or not.



##  2 Hidden Layers

Now we will create a second layer (for now just keeping it the same size) and seeing if we can find any improvements upon training and final generation. Upon runnning it and trying top optimize we got something along the lines of this: 


```
      90000/100000: 2.1761744022369385
  91000/100000: 2.6888418197631836
  92000/100000: 2.6372430324554443
  93000/100000: 2.307980537414551
  94000/100000: 2.062338352203369
  95000/100000: 2.319122076034546
  96000/100000: 2.1467628479003906
  97000/100000: 2.1012003421783447
  98000/100000: 2.377164602279663
  99000/100000: 2.1481876373291016
1.8713290691375732
```

The loss doesn't seem a whole lot better but perhaps because of the increase of neurons, the gradient descent is a lot more inconsistent and jumpy. Upon running this on a test set we were able to achieve: 


```
nuphorilirillist.
menesses.
iliet.
liresonest.
nabtoredililelesenesesesescilestiriletiresterisesterinescedes.
nocdesteresterediles.
undesiristeres.
nonessuredirecedenal.
edestoryslescedes.
nurysistololis.
tegectedal.
nopetestiles.
nurecestaredelin.
net.
ilesateress.
nupenes.
nat.
lamedat.
pet.
netysestedeste.
ratostersastir.
```

This is a HUGE improvement in the words. Although the loss function may not be a ton lower, it is great to see such a huge upgrade on this. Let's see if we can get any other upgrades with a second hidden layer or not.

---

---

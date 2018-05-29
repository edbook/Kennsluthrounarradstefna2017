Eiginleikar
===========

Viðbætur
--------

Stærðfræðitákn
~~~~~~~~~~~~~~

Það er auðvelt að setja inn stærðfræðitákn eins og :math:`e^{\cos(x)}` eða
heilar jöfnur

.. math::
    \frac{d}{dz} \cos(z) = \sum_{n\in \mathbb N} \frac {d}{dz}\, \frac{(-1)^n}{(2n)!} z^{2n}
    = \sum_{n\geq 1} \frac{(-1)^n}{(2n-1)!}z^{2n-1} = -\sin(z)

Hlekkir
~~~~~~~

Hægt að vísa beint í allar efnisgreinar (t.d. úr lausnum, Piazza og tölvupóstum).
Eins hægt að vísa innan efnisins milli efnisgreina, sjá :ref:`Tilgangur`.

Geogebra
~~~~~~~~

Geogebra (http://geogebra.org)  er frábært forrit til að útbúa gagnvirk smáforrit sem er svo hægt að setja inn í námsefnið.

.. ggb:: pCuJwqEE
    :width: 700
    :height: 400
    :img: ./03_undirogyfirsumma.png
    :imgwidth: 12cm

|

|

Sage
~~~~

Hægt er að nota Sage til þess að setja inn smáforrit skrifuð í 
Sage, Octave, R o.fl.

.. sagecell::

    var ('x y r n'); r = 1; inside = 0; points = []
    n = 100  ## Try changing this! This is the number of shots the estimate is based on
    ### Shoot randomly into the square:
    for i in range(0,n):
        [x,y]=[random(),random()]
        points.append([x,y])
        
    ### If a shot lands inside the circle, make a note of it
        if (y <= sqrt((r^2)-(x^2))):
            inside += 1
        
    ### Approximate pi based on the fraction of shots that landed in the circle
    ### Area of circle = pi*r^2; Area of square = (2*r)^2 = 4*r^2
    ### Shots in circle / Shots in square = (pi*r^2)/(4*r^20 = pi()/4
    piapprox = 4*(inside / n)
    estimate = "Með því að nota "
    estimate += str(n)
    estimate += " punkta, fæst að pi er um það bil "
    estimate += str(piapprox.n())
    show(estimate)
    ### Graph the solution
    circle = []
    for i in range(0,1000):
        x = i/1000
        y = sqrt((r^2)-(i/1000)^2)
        circle.append([x,y])
    graph = list_plot(points)
    graph += list_plot(circle,color='red',figsize=[5,4],plotjoined=true)
    show(graph)


|

|

Panopto
~~~~~~~

Auðvelt er að greypa inn myndbönd af Youtube eða Panopto (http://rec.hi.is)

.. panopto:: f624b32e-178d-41cc-8ccb-a559712471d7
    :width: 720
    :height: 405

|

|

Annað
-----

* `Atriðaorðaskrá <https://edbook.hi.is/stae104g/genindex.html>`_.

* Hægt að fá þýðingar á tilteknum orðum í stærðfræði, 
  til dæmis :hover:`heiltala`.

* Þýðingum er safnað saman í `orðaskrá <https://edbook.hi.is/stae104g/ordaskra.html>`_. 
  Þýðingar er fengnar úr Orðaskrá Íslenska stærðfræðafélagsins (http://stae.is/os).

* Hægt að fylgjast með notkun gegnum netþjón, Google Analytics og Panopto.




Text Data Augmentation for Vietnamese
===============
Installing
============

.. code-block:: bash

    pip install --upgrade vitextaug

============
Down load VTA folder from

.. code-block:: bash

    https://drive.google.com/file/d/1hwmSz8WYv8x6N-Ncj51ZNGyhjrkMzGu_/view?usp=share_link
    
Usage
=====

.. code-block:: bash

    >>> from vitextaug.augmentor import LexicalReplacement, WordEmbeddingReplacement
    >>> text = "Sau cơn lũ quét qua, bản Hòa Sơn tan hoang, nhiều nhà cửa, tài sản của người dân bị nước lũ cuốn trôi. "
    >>> lr = LexicalReplacement(path="/home/longnt/VTA/",
                                replacement_rate=0.9)

    >>> print(lr.augment(text))
    'sau cơn lũ quét , bản hoà sơn tan hoang , nhiều nhà cửa , đồng tiền bạc của người dân quê hương bị lũ cuốn đi .'

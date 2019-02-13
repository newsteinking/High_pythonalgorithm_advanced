chapter 1: Array
=======================================


26. Remove Duplicated From Sorted Array
---------------------------------------------
Given a sorted array nums, remove the duplicates in-place such that each element appear only once and
return the new length.

Do not allocate extra space for another array, you must do this by modifying the input array in-place with O(1)
extra memory.

Example 1:

Given nums = [1,1,2],

Your function should return length = 2, with the first two elements of nums being 1 and 2 respectively.

It doesn't matter what you leave beyond the returned length.
Example 2:

Given nums = [0,0,1,1,1,2,2,3,3,4],

Your function should return length = 5, with the first five elements of nums being modified to 0, 1, 2, 3,

and 4 respectively.

It doesn't matter what values are set beyond the returned length.


.. code-block:: python

    #! /usr/bin/env python
    # -*- coding: utf-8 -*-


    class Solution(object):
        def removeDuplicates(self, nums):
            """
            :type nums: List[int]
            :rtype: int
            """
            if not nums:
                return 0

            removed_end = 0
            for i in range(1, len(nums)):
                if nums[i] != nums[removed_end]:
                    removed_end += 1
                    nums[removed_end] = nums[i]

            return removed_end + 1

    """
    []
    [1,1,2,2,3]
    [1,3,5,8,9,9,9]
    """



27. Remove Element
---------------------------------


.. code-block:: python




31. Next Permutation
---------------------------------

.. code-block:: python




41. First Missing Positive
---------------------------------



.. code-block:: python





54. Spiral Matrix
---------------------------------

.. code-block:: python




57. Insert Interval
---------------------------------

.. code-block:: python





59. Spiral Matrix 2
---------------------------------

.. code-block:: python





73. Set Matrix Zeroes
---------------------------------

.. code-block:: python



118. Pascal Triange
---------------------------------

.. code-block:: python




119. Pascal Triangel 2
---------------------------------

.. code-block:: python




164. Maximum Gap
---------------------------------

.. code-block:: python



189. Rotate Array
---------------------------------

.. code-block:: python




228. Summary Ranges
---------------------------------

.. code-block:: python




283. Move Zeroes
---------------------------------

.. code-block:: python



289. Game of Life
---------------------------------

.. code-block:: python
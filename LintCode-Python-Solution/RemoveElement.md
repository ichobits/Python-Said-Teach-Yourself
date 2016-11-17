##删除元素
###描述

给定一个数组和一个值，在原地删除与值相同的数字，返回新数组的长度。

元素的顺序可以改变，并且对新的数组不会有影响。
 
###测试用例：
给出一个数组A, [0,4,4,0,0,2,4,4]，和elem的值:4

返回 4 并且4个元素的新数组为[0,0,0,2]
 
###思路：
 Python中实现方案有很多，对人言我想到的最方便的代码就是下面这样的，代码如下：

    def removeElement(A, elem):
        try:
            while(True):
                A.remove(elem)
        except ValueError:
            return len(A)
    
该算法时间复杂度为`<`O(n<sup>2</sup>)，相当于等差数列前n项和。考虑时空效率时应该还有更好的算法，感兴趣的同学可以再深挖一下。
学习笔记
贪心算法：
一、基本概念：
     所谓贪心算法是指，在对问题求解时，总是做出在当前看来是最好的选择。也就是说，不从整体最优上加以考虑，他所做出的仅是在某种意义上的局部最优解。
     贪心算法没有固定的算法框架，算法设计的关键是贪心策略的选择。
     必须注意的是，贪心算法不是对所有问题都能得到整体最优解，选择的贪心策略必须具备无后效性，即某个状态以后的过程不会影响以前的状态，只与当前状态有关。
    所以对所采用的贪心策略一定要仔细分析其是否满足无后效性。

二、贪心算法的基本思路：
    1.建立数学模型来描述问题。
    2.把求解的问题分成若干个子问题。
    3.对每一子问题求解，得到子问题的局部最优解。
    4.把子问题的解局部最优解合成原来解问题的一个解。

三、贪心算法适用的问题
      贪心策略适用的前提是：局部最优策略能导致产生全局最优解。
      实际上，贪心算法适用的情况很少。一般，对一个问题分析是否适用于贪心算法，可以先选择该问题下的几个实际数据进行分析，就可做出判断。
      贪心算法的证明围绕着：整个问题的最优解一定由在贪心策略中存在的子问题的最优解得来的。


二分查找：
二分查找算法思想

有序的序列，每次都是以序列的中间位置的数来与待查找的关键字进行比较，每次缩小一半的查找范围，直到匹配成功。


一个情景：将表中间位置记录的关键字与查找关键字比较，如果两者相等，则查找成功；
                否则利用中间位置记录将表分成前、后两个子表，如果中间位置记录的关键字大于查找关键字，则进一步查找前一子表，否则进一步查找后一子表。
                重复以上过程，直到找到满足条件的记录，使查找成功，或直到子表不存在为止，此时查找不成功。

二分查找优缺点


优点是比较次数少，查找速度快，平均性能好；

其缺点是要求待查表为有序表，且插入删除困难。

因此，折半查找方法适用于不经常变动而查找频繁的有序列表。


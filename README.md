# avltree.h
Here STL is written in AVL Tree and compared with the STL by GNU which is written in Red-Black-Trees.\
\
It all started while knowing about why Set's Operations like Insertion takes O(1) and came to know it is implemented using Balanced Trees and using Red-Black-Trees, I wanted to create my own container like Hash-Set and I saw this Repository of STL in Red-Black-Tree containers(https://github.com/frozenca/CLRS/blob/main/core/rbtree.h). I quickly took help from Chat-GPT and few functions written by me of STL using AVLTree containers. The reason I didn't write using B-Tree is, there is already a Google Open Source Blog on this(https://opensource.googleblog.com/2013/01/c-containers-that-save-memory-and-time.html?m=1) and I did compared both STL's and recorded the observations\
\
Observations - \
\
Balanced binary search tree demo\
frozenca::hard::TreeSet<int> test\
Time to insert  50000 elements:\
Average : 26733.1562 us,\
Stdev   : 11149.6426 us,\
95%     : 48692.4336 us,\
99%     : 57536.4609 us,\
99.9%   : 65042.8633 us,\
\
Time to find  50000 elements:\
Average : 19758.7656 us,\
Stdev   :  9610.9668 us,\
95%     : 40658.7344 us,\
99%     : 47869.8672 us,\
99.9%   : 53613.1094 us,\
\
Time to erase  50000 elements:\
Average : 30502.7344 us,\
Stdev   : 13465.8848 us,\
95%     : 58316.6172 us,\
99%     : 65425.8164 us,\
99.9%   : 83249.9844 us,\
\
frozenca::hard::AVLTreeSet<int> test\
Time to insert  50000 elements:\
Average : 28428.4961 us,\
Stdev   : 12163.4414 us,\
95%     : 53065.8203 us,\
99%     : 64068.2031 us,\
99.9%   : 95926.4531 us,\
\
Time to find  50000 elements:\
Average : 19861.9648 us,\
Stdev   : 10665.3408 us,\
95%     : 38907.1016 us,\
99%     : 47714.2930 us,\
99.9%   : 121964.1719 us,\
\
Time to erase  50000 elements:\
Average : 32485.6992 us,\
Stdev   : 14607.7715 us,\
95%     : 59458.1992 us,\
99%     : 84706.0547 us,\
99.9%   : 135156.2812 us,\
\
std::set<int> test\
Time to insert  50000 elements:\
Average : 29837.6582 us,\
Stdev   :  8727.2793 us,\
95%     : 47202.6680 us,\
99%     : 62070.0664 us,\
99.9%   : 116624.7344 us,\
\
Time to find  50000 elements:\
Average : 18689.8281 us,\
Stdev   :  7408.6602 us,\
95%     : 30420.7617 us,\
99%     : 48766.2500 us,\
99.9%   : 80909.3750 us,\

Time to erase  50000 elements:
Average : 34131.6836 us,
Stdev   : 10945.4082 us,
95%     : 55325.1250 us,
99%     : 85706.6562 us,
99.9%   : 119719.9375 us,

Credits - https://github.com/frozenca/CLRS/blob/main/core/rbtree.h

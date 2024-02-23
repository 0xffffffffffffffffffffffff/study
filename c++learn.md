[TOC]
# STL
## algorithm 里面有哪些函数
1. **排序算法：**
    - `sort()`：对范围内的元素进行排序。
    ```c++
    //升序
    sort(nums.begin(), nums.end());
    ```
    ```c++
    //降序
    sort(nums.rbegin(), nums.rend());
    ```

    - `stable_sort`：对范围内的元素进行稳定排序。
    ```c++
    stable_sort(nums.begin(), nums.end());
    ```

    - `partial_sort`：对范围内的元素进行部分排序。
    ```c++
    // 使用 partial_sort 对前三个最小的元素进行排序
    partial_sort(nums.begin(), nums.begin() + 3, nums.end());
    ```

    - `nth_element`：对范围内的元素进行部分排序，使得第 n 个元素处于正确的位置。
    ```c++
    // 使用 nth_element 将第三个最小的元素放在正确的位置
    nth_element(nums.begin(), nums.begin() + 2, nums.end());
    ```

2. **查找算法：**
    - `find`：在范围内查找指定值的元素。
    ```c++
    // 使用 find 查找值为 9 的元素
    auto it = find(nums.begin(), nums.end(), 9);
    // 检查是否找到
    if (it != nums.end()) {
      //找到了
    } else {
      //没找到
    }
    ```

    - `find_if`：在范围内查找满足指定条件的元素。
    ```c++
    // 使用 Lambda 表达式作为谓词函数，查找第一个大于 5 的元素
    auto it = find_if(nums.begin(), nums.end(), [](int value) {return value>5;});
    // 检查是否找到
    if (it != nums.end()) {
      //找到了
    } else {
      //没找到
    }
    ```
    
    - `binary_search`：在有序范围内进行二分查找。
    ```c++
    // 使用 binary_search 判断值 5 是否存在
    bool result = binary_search(nums.begin(), nums.end(), 5);
    ```
    
    - `lower_bound`：在有序范围内查找第一个不小于某个值的元素。
    ```c++
    // 使用 lower_bound 查找第一个不小于 5 的元素的位置
    auto it = lower_bound(nums.begin(), nums.end(), 5);
    // 输出结果
    if (it != nums.end()) {
      //找到了
    } else {
      //没找到
    }
    ```
    
    - `upper_bound`：在有序范围内查找第一个大于某个值的元素。
    ```c++
    // 使用 upper_bound 查找第一个大于 5 的元素的位置
    auto it = upper_bound(nums.begin(), nums.end(), 5);
    // 输出结果
    if (it != nums.end()) {
      //找到了
    } else {
      //没找到
    }
    ```
    
    - `equal_range`：在有序范围内查找等值范围。
    ```c++
    // 使用 equal_range 查找值为 4 的元素的范围
    auto range = equal_range(nums.begin(), nums.end(), 4);
    // 查找结果为 [range.first, range.second]
    ```
    

3. **合并和操作范围：**
    - `merge`：将两个有序序列合并为一个有序序列。
    ```c++
    // 使用 merge 合并两个有序序列，将arr1和arr2合并为result
    merge(arr1.begin(), arr1.end(), arr2.begin(), arr2.end(), result.begin());
    ```
    
    - `set_union`、`set_intersection`、`set_difference`、`set_symmetric_difference`：对两个有序范围执行集合操作。
    ```c++
    ```
   
4. **计数操作：**
    - `count`：统计范围内某个元素出现的次数。
    ```c++
    count(nums.begin(), nums.end(), 2);
    ```
    - `max_element`：统计范围内的最大值。
    ```c++
    *max_element(nums.begin(), nums.end());
    ```
4. **算法操作：**
    - `copy`：将一个范围的元素复制到另一个范围。
    - `move`：将一个范围的元素移动到另一个范围。
    - `swap`：交换两个元素的值。
    - `rotate`：将范围内的元素循环右移。

5. **数值算法：**
    - `accumulate`：对范围内的元素进行累积。
    ```c++
    accumulate(nums.begin(), nums.end(), 0);
    ```
    - `inner_product`：计算两个范围的内积。
    - `partial_sum`：计算范围内的部分和。
    ```c++
    vector<int> sums(n,0);
    partial_sum(nums.begin(), nums.end(), sums.begin());
    ```
    - `iota`：生成一个范围的递增序列。

这只是 `<algorithm>` 头文件中一些常用函数的概览，实际上还有很多其他函数。具体的使用方法和详细说明可以参考 C++ 标准库的文档或其他参考资料。
# 单链表
1. **头插法建立单链表：**
2. **尾插法建立单链表：**
    ```c++
    ListNode* tailCreate(const vector<int>& values) {
        ListNode* head = nullptr;  // 头指针
        ListNode* tail = nullptr;  // 尾指针
        for (int value : values) {
            ListNode* newNode = new ListNode(value);
            // 如果链表为空，新节点即为头节点
            if (head == nullptr) {
                head = newNode;
                tail = newNode;
            } else {
                // 否则，将新节点连接到尾部，并更新尾指针
                tail->next = newNode;
                tail = newNode;
            }
        }
        return head;
    }
    ```
3. **获取链表节点值到vector：**
4. **释放单链表内存：**
    ```c++
    void deleteLinkedList(ListNode* head) {
        while (head != nullptr) {
            ListNode* temp = head;
            head = head->next;
            delete temp;
        }
    }
    ```

# 堆
1. **`priority_queue`：优先队列，可以当做一个自动维护的堆。**
    - 大顶堆
    ```c++
    priority_queue<int> q;
    priority_queue<int> q(nums.begin(), nums.end());
    priority_queue<int, vector<int>> q;
    priority_queue<int,vector<int>,less<int>> q;
    ```
    - 小顶堆
    ```c++
    priority_queue<int, vector<int>, greater<int>> q(nums.begin(), nums.end());
    ```
    - 自定义堆
    ```c++
    //以字符的map值为依据建立大顶堆
    //写法1：
    unordered_map<char,int> mp;
    struct rule{   //按照结构体中y从大到大
      bool operator()(char a,char b){
        return mp[a] > mp[b];
      }
    };
    priority_queue<char,vector<char>,rule>q;

    //写法2：lambda表达式 
    unordered_map<char, int> mp；
    auto rule = [&mp](char a, char b) {
      return mp[a] > mp[b];
    };
    priority_queue<char, vector<char>, decltype(rule)> q(rule);

    //以pair的第二个元素为依据建立小顶堆
    vector<pair<int,int>>groups;
    struct rule{
      bool operator()(pair<int,int> a,pair<int,int> b){
        return a.second < b.second;
      }
    };
    priority_queue<pair<int,int>, vector<pair<int,int>>, rule> q;
    ```
    - 成员函数
    ```c++
    q.empty();   // 如果优先队列为空，则返回真 
    q.size();    //返回优先队列中拥有的元素的个数 
    q.top();     //返回优先队列中有最高优先级的元素 
    q.pop();     // 删除第一个元素 
    q.push(num); // 加入一个元素 
    ```
    **数组原地堆化：**
    原地堆化的数组依然可以使用`vector`的方法和成员函数。
    - 大顶堆
    ```c++
    make_heap(nums.begin(), nums.end());  //数组原地堆化
    pop_heap(nums.begin(), nums.end());   //将堆顶元素弹出，并放到末尾
    push_heap(nums.begin(), nums.end());  //只对末尾元素进行调整，时间O(logn)
    sort_heap(nums.begin(), nums.end());  //对整个堆进行调整，时间O(nlogn)
    ```
    - 小顶堆
    ```c++
    make_heap(nums.begin(), nums.end(), greater<int>);  //数组原地堆化
    pop_heap(nums.begin(), nums.end(), greater<int>);   //将堆顶元素弹出，并放到末尾
    push_heap(nums.begin(), nums.end(), greater<int>);  //只对末尾元素进行调整，时间O(logn)
    sort_heap(nums.begin(), nums.end(), greater<int>);  //对整个堆进行调整，时间O(nlogn)
    ```

# 单调栈

# 单调队列
1. **单调队列能够保证队内元素单调，以单调递减的单调队列为例：**
    - 每次入队时如果队尾元素是否小于待入队元素，会从将队尾元素踢出。
    - 出队操作同队列
    ```c++
    // 定义一个单调递减的单调队列
    template <typename T> class MonotonicQueue {
    private:
        std::deque<T> data; // 使用deque来实现单调队列
    public:
        // 构造函数
        MonotonicQueue() {}
        // 向队尾添加元素，确保队列单调递减
        void push(const T& value) {
            while (!data.empty() && value > data.back()) {
                data.pop_back();
            }
            data.push_back(value);
        }
        // 弹出队首元素，如果要弹出的元素等于队首元素，则弹出
        void pop() { data.pop_front(); }
        // 获取队首元素
        T front() const { return data.front(); }
        // 检查队列是否为空
        bool empty() const { return data.empty(); }
        // 获取队列中元素个数
        size_t size() const { return data.size(); }
        // 遍历队列元素
        void print() const {
            for (const T& element : data) {
                std::cout << element << " ";
            }
            std::cout << std::endl;
        }
    };
    ```

z函数
ST表
线段树
树状数组
GCD(a, b) * LCM(a, b) = |a * b|
对于任意正整数 a、b 和 c，有 GCD(a * c, b * c) = GCD(a, b) * c



这是欧几里德算法的一个重要性质。\[ \text{GCD}(a, b) = \text{GCD}(b - a, a) \]

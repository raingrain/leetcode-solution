# 线段树SegmentTree代码模板

## [2236. 判断根结点是否等于子结点之和](https://leetcode.cn/problems/root-equals-sum-of-children/)

> - **Question 1**
>   - 给你一个二叉树的根结点 `root` ，该二叉树由恰好 `3` 个结点组成：根结点、左子结点和右子结点。如果根结点值等于两个子结点值之和，返回 `true` ，否则返回 `false` 。
>   - **Tips**
>     - 树只包含根结点、左子结点和右子结点
>     - `-100 <= Node.val <= 100`

## [303. 区域和检索 - 数组不可变](https://leetcode.cn/problems/range-sum-query-immutable/)

## [307. 区域和检索 - 数组可修改](https://leetcode.cn/problems/range-sum-query-mutable/)

> - **Question 2**
>   - 给你一个数组 `nums` ，请你完成三类查询：
>     - 一类查询要求更新数组 `nums` 下标对应的值。
>     - 一类查询要求数组 `nums` 下标对应的值全部加上一个新的值。
>     - 一类查询要求返回数组 `nums` 中索引 `left` 和 `right` 之间（包含边界）的 `nums` 元素的和。
>   - 实现 `NumArray` 类（线段树的功能）：
>     - `NumArray(int[] nums)` 用整数数组 `nums` 初始化对象。
>     - `void update(int index, int val)` / `void update(int left, int right, int val)` 将对应区间内的值更新为 `val` 。
>     - `void add(int index, int val)` / `void add(int left, int right, int val)` 将对应区间内的值全部加上 `val` 。
>     - `int sumRange(int left, int right)` 返回数组 `nums` 中索引 `left` 和索引 `right` 之间的 `nums` 元素的和。
>   - **Tips**
>     - `1 <= nums.length <= 3 * 10^4`
>     - `-10^5 <= nums[i] <= 10^5`
>     - `0 <= index < nums.length`
>     - `-100 <= val <= 100`
>     - `0 <= left <= right < nums.length`
>     - 调用 `update` 和 `add` 和 `sumRange` 方法次数不大于 `3 * 10^4`

## [P3372 【模板】线段树 1](https://www.luogu.com.cn/problem/P3372)

> - **Question 3**
>   - 如题，已知一个数列，你需要进行下面两种操作：将某区间每一个数加上 `k` ；求出某区间每一个数的和。
>   - **输入描述**
>     - 第一行包含两个整数 `n, m`，分别表示该数列数字的个数和操作的总个数。
>     - 第二行包含 `n` 个用空格分隔的整数，其中第 `i` 个数字表示数列第 `i` 项的初始值。
>     - 接下来 `m` 行每行包含 `3` 或 `4` 个整数，表示一个操作，具体如下：
>       1. `1 x y k` ：将区间 `[x, y]` 内每个数加上 `k` 。
>       2. `2 x y` ：输出区间 `[x, y]` 内每个数的和。
>   - **输出描述**
>     - 输出包含若干行整数，即为所有操作 `2` 的结果。
>   - **Tips**
>     - `1 <= n, m <= 10^5`

## [P1253 扶苏的问题](https://www.luogu.com.cn/problem/P1253)

> - **Question 4**
>   - 给定一个长度为 `n` 的序列 `a` ，要求支持如下三个操作：
>     - 给定区间 `[l, r]` ，将区间内每个数都修改为 `x` 。
>     - 给定区间 `[l, r]` ，将区间内每个数都加上 `x` 。
>     - 给定区间 `[l, r]` ，求区间内的最大值。
>   - **输入描述**
>     - 第一行是两个整数，依次表示序列的长度 `n` 和操作的个数 `q` 。
>     - 第二行有 `n` 个整数，第 `i` 个整数表示序列中的第 `i` 个数 `ai` 。
>     - 接下来 `q` 行，每行表示一个操作。每行首先有一个整数 `op` ，表示操作的类型。
>       - 若 `op = 1` ，则接下来有三个整数 `l, r, x` ，表示将区间 `[l, r]` 内的每个数都修改为 `x` 。
>       - 若 `op = 2` ，则接下来有三个整数 `l, r, x` ，表示将区间 `[l, r]` 内的每个数都加上 `x` 。
>       - 若 `op = 3` ，则接下来有两个整数 `l, r` ，表示查询区间 `[l, r]` 内的最大值。
>   - **输出描述**
>     - 对于每个 `op = 3` 的操作，输出一行一个整数表示答案。
>   - **Tips**
>     - `1 <= n, q <= 10^6`
>     - `1 <= l, r <= n`
>     - `op = 1 or 2 or 3`
>     - `|ai|, |x| <= 10^9`

## [P2781 传教](https://www.luogu.com.cn/problem/P2781)

> - **Question 5**
>   - 一共有 `n` 个位置，编号从 `1 ~ n` ，一开始所有位置的值为 `0` 。
>   - 实现如下两个操作，一共会调用 `m` 次。
>     - 操作 `l r v` ：把 `l ~ r` 范围的每个数增加 `v` 。
>     - 操作 `l r` ：返回 `l ~ r` 范围的累加和。
>   - **Tips**
>     - `1 <= n <= 10^9`
>     - `1 <= m <= 10^3`

## [Gorgeous Sequence](https://acm.hdu.edu.cn/showproblem.php?pid=5306)

> - **Question 6**
>   - 给定一个长度为 `n` 的数组 `arr` ，实现支持以下三种操作的结构：
>     - `l r x` ：把 `arr[l...r]` 范围的每个数 `v` ，更新成 `min(v, x)` 。
>     - 操作 `1 l r` ：查询 `arr[l...r]` 范围上的最大值。
>     - 操作 `2 l r` ：查询 `arr[l...r]` 范围上的累加和。
>   - 三种操作一共调用 `m` 次，做到时间复杂度 `O(n * logn + m * logn)` 。

## 线段树范围增加操作 + 区间最值操作

> - **Question 7**
>   - 给定一个长度为 `n` 的数组 `arr` ，实现支持以下四种操作的结构
>     - 操作 `l r x` ：把 `arr[l...r]` 范围的每个数 `v` ，增加 `x` 。
>     - 操作 `l r x` ：把 `arr[l...r]` 范围的每个数 `v` ，更新成 `min(v, x)` 。
>     - 操作 `l r` ：查询 `arr[l...r]` 范围上的最大值。
>     - 操作 `l r` ：查询 `arr[l...r]` 范围上的累加和。

## [P6242 【模板】线段树 3（区间最值操作、区间历史最值）](https://www.luogu.com.cn/problem/P6242)

> - **Question 8**
>   - 给定两个长度都为 `n` 的数组 `A` 和 `B` ，一开始两个数组完全一样。
>   - 任何操作做完，都更新 `B` 数组 `B[i] = max(B[i], A[i])` 。
>   - 实现以下五种操作，一共会调用 `m` 次。
>     - 操作 `l r v` ： `A[l...r]` 范围上每个数加上 `v` 。
>     - 操作 `l r v` ： `A[l...r]` 范围上每个数 `A[i]` 变成 `min(A[i],v)` 。
>     - 操作 `l r` ：返回 `A[l...r]` 范围上的累加和。
>     - 操作 `l r` ：返回 `A[l...r]` 范围上的最大值。
>     - 操作 `l r` ：返回 `B[l...r]` 范围上的最大值。
>   - **Tips**
>     - `1 <= n、m <= 5 * 10^5`

## Java

> - **Question 1: 线段树每个节点的性质**
>   - 根节点代表区域和，左右子节点代表分区域和。

```java
class Solution {

    public boolean checkTree(TreeNode root) {
        return root.val == root.left.val + root.right.val;
    }

}
```

> - **Question 2: 数组实现线段树**
>   - 线段树用于处理左右半区获得的信息不用处理就可以加工出整个区域的正确信息的问题，如区间最值查询等。
>   - 线段树快的核心在于信息的懒处理。

```java
class NumArray {
    
    // 新数组长度
    private final int size;
    // 新数组
    private final int[] arr;
    // 对应区间的累加和
    // 线段树本体
    private final int[] sum;
    // add方法的懒加载信息
    // lazy[i]代表对应区间上每个数字要加的数
    private final int[] lazy;
    // change[i]指要change成的数
    private final int[] change;
    // 避免change[i]等于0的歧义，true表示要更新，false反之
    private final boolean[] isUpdate;
    
    public NumArray(int[] nums) {
        this.size = nums.length + 1;
        this.arr = new int[size];
        System.arraycopy(nums, 0, this.arr, 1, size - 1);
        // 算上各种不需要的节点树的所有层的满节点数不超过4N
        // 用来支持脑补概念中，某一个范围的累加和信息
        this.sum = new int[size * 4];
        // 用来支持脑补概念中，某一个范围沒有往下传递的累加任务
        this.lazy = new int[size * 4];
        // 用来支持脑补概念中，某一个范围有没有更新操作的任务
        this.change = new int[size * 4];
        // 用来支持脑补概念中，某一个范围更新任务，更新成了什么
        this.isUpdate = new boolean[size * 4];
        build(1, nums.length, 1);
    }
    
    private void getSum(int head) {
        sum[head] = sum[head * 2] + sum[head * 2 + 1];
    }
    
    // 在初始化阶段，先把sum数组，填好
    // 在arr[1 ~ arr.length - 1]范围上，去build sum数组，
    // head是这个范围在sum数组中的下标
    // int[] nums,
    private void build(int left, int right, int head) {
        if (left == right) {
            // sum[head] = nums[left - 1];
            sum[head] = arr[left];
            return;
        }
        int mid = (left + right) >> 1;
        build(left, mid, head * 2);
        build(mid + 1, right, head * 2 + 1);
        getSum(head);
    }
    
    // 懒信息推送
    // 之前的所有懒加载和懒更新，从父范围发给左右两个子范围
    private void pushDown(int head, int numOfLeftTree, int numOfRightTree) {
        // 更新的优先级高于加数
        if (isUpdate[head]) {
            // 把确定更新的信息推送到下一层
            isUpdate[head * 2] = true;
            isUpdate[head * 2 + 1] = true;
            // 把要更新成的数字推送到下一层
            change[head * 2] = change[head];
            change[head * 2 + 1] = change[head];
            // 因为需要更新，所以要add的数据直接被清空
            lazy[head * 2] = 0;
            lazy[head * 2 + 1] = 0;
            // 因为对应范围内全部都更新了，那么累加和自然就变成更新后的值乘以范围
            sum[head * 2] = change[head] * numOfLeftTree;
            sum[head * 2 + 1] = change[head] * numOfRightTree;
            isUpdate[head] = false;
        }
        // 需要对add数据进行懒更新
        // 刚更新完是不会有add数据存在的，在更新时都被清理了
        if (lazy[head] != 0) {
            // 懒加载信息被推送而来
            lazy[head * 2] += lazy[head];
            lazy[head * 2 + 1] += lazy[head];
            // 对应的区间和增加
            sum[head * 2] += lazy[head] * numOfLeftTree;
            sum[head * 2 + 1] += lazy[head] * numOfRightTree;
            // 懒加载信息已经推送到下一层，本层懒加载信息归0
            lazy[head] = 0;
        }
    }
    
    // 任务是在数组sum的L~R位置的数全部更新成val，当前来到的数组位置是head，其代表的区间范围是left~right
    private void update(int L, int R, int val, int left, int right, int head) {
        // 任务区间能把当前区间囊括住
        // 直接在这一层进行操作并更新懒信息
        if (L <= left && right <= R) {
            // 如果新老两个任务都能把当前区间囊括，就一起停在这一层
            isUpdate[head] = true;
            change[head] = val;
            sum[head] = val * (right - left + 1);
            lazy[head] = 0;
            return;
        }
        // 任务区间没能把当前区间囊括住
        int mid = (left + right) >> 1;
        // 新来的任务不能被head层拦截
        // 先把head层存下来的任务发到下一层
        // 然后再把新来的任务下发（因为新来的也不能被拦截）
        pushDown(head, mid - left + 1, right - mid);
        if (L <= mid) {
            update(L, R, val, left, mid, head * 2);
        }
        if (mid + 1 <= R) {
            update(L, R, val, mid + 1, right, head * 2 + 1);
        }
        getSum(head);
    }
    
    // 和update的含义一样，变成加上某个数
    private void add(int L, int R, int val, int left, int right, int head) {
        if (L <= left && right <= R) {
            sum[head] += val * (right - left + 1);
            lazy[head] += val;
            return;
        }
        int mid = (left + right) >> 1;
        pushDown(head, mid - left + 1, right - mid);
        if (L <= mid) {
            add(L, R, val, left, mid, head * 2);
        }
        if (mid + 1 <= R) {
            add(L, R, val, mid + 1, right, head * 2 + 1);
        }
        getSum(head);
    }
    
    // 查询区间和
    private int sumRange(int L, int R, int left, int right, int head) {
        // 任务区间能把当前区间囊括住
        // 直接查询累加和并返回
        if (L <= left && right <= R) {
            return sum[head];
        }
        int mid = (left + right) >> 1;
        pushDown(head, mid - left + 1, right - mid);
        int ans = 0;
        if (L <= mid) {
            ans += sumRange(L, R, left, mid, head * 2);
        }
        if (mid + 1 <= R) {
            ans += sumRange(L, R, mid + 1, right, head * 2 + 1);
        }
        return ans;
    }
    
    // 对外提供的方法的索引是原数组，要加1才能运用于线段树的相关数组

    public void update(int left, int right, int val) {
        update(left + 1, right + 1, val, 1, size - 1, 1);
    }
    
    public void update(int index, int val) {
        update(index + 1, index + 1, val, 1, size - 1, 1);
    }
    
    public void add(int left, int right, int val) {
        add(left + 1, right + 1, val, 1, size - 1, 1);
    }
    
    public void add(int index, int val) {
        add(index + 1, index + 1, val, 1, size - 1, 1);
    }
    
    // 查询指定区间累加和
    public int sumRange(int left, int right) {
        return sumRange(left + 1, right + 1, 1, size - 1, 1);
    }
    
}
```

> - **动态开点实现线段树**
>   - 有需要才创建

```java
class DynamicSegmentTree {
    
    // 节点与范围解耦，范围由函数控制
    private static class DynamicSegmentTreeNode {
        
        public int sum;
        public int lazy;
        public int change;
        public boolean update;
        public DynamicSegmentTreeNode left;
        public DynamicSegmentTreeNode right;
        
    }
    
    private final DynamicSegmentTreeNode root;
    private final int size;
    // private final int[] origin;
    
    public DynamicSegmentTree(int size) {
        root = new DynamicSegmentTreeNode();
        this.size = size;
        // this.origin = origin;
        // buildTree();
    }
    
    /*private void buildTree() {
        for (int i = 0; i < origin.length; i++) {
            add(root, 1, origin.length, i + 1, i + 1, origin[i]);
        }
    }*/
    
    private void getSum(DynamicSegmentTreeNode node) {
        node.sum = node.left.sum + node.right.sum;
    }
    
    private void pushDown(DynamicSegmentTreeNode node, int leftSize, int rightSize) {
        // 没有节点要创建，不然没法往下推送
        if (node.left == null) {
            node.left = new DynamicSegmentTreeNode();
        }
        if (node.right == null) {
            node.right = new DynamicSegmentTreeNode();
        }
        if (node.update) {
            node.left.update = true;
            node.right.update = true;
            node.left.change = node.change;
            node.right.change = node.change;
            node.left.lazy = 0;
            node.right.lazy = 0;
            node.left.sum = node.change * leftSize;
            node.right.sum = node.change * rightSize;
            node.update = false;
        }
        if (node.lazy != 0) {
            node.left.lazy += node.lazy;
            node.right.lazy += node.lazy;
            node.left.sum += node.lazy * leftSize;
            node.right.sum += node.lazy * rightSize;
            node.lazy = 0;
        }
    }
    
    private void update(DynamicSegmentTreeNode node, int left, int right, int start, int end, int value) {
        if (start <= left && right <= end) {
            node.update = true;
            node.change = value;
            node.sum = value * (right - left + 1);
            node.lazy = 0;
        } else {
            int mid = left + (right - left) / 2;
            pushDown(node, mid - left + 1, right - mid);
            if (start <= mid) {
                update(node.left, left, mid, start, end, value);
            }
            if (end >= mid + 1) {
                update(node.right, mid + 1, right, start, end, value);
            }
            getSum(node);
        }
    }
    
    private void add(DynamicSegmentTreeNode node, int left, int right, int start, int end, int value) {
        if (start <= left && right <= end) {
            node.sum += value * (right - left + 1);
            node.lazy += value;
        } else {
            int mid = left + (right - left) / 2;
            pushDown(node, mid - left + 1, right - mid);
            if (start <= mid) {
                add(node.left, left, mid, start, end, value);
            }
            if (end >= mid + 1) {
                add(node.right, mid + 1, right, start, end, value);
            }
            getSum(node);
        }
    }
    
    private int sumRange(DynamicSegmentTreeNode node, int left, int right, int start, int end) {
        if (start <= left && right <= end) {
            return node.sum;
        } else {
            int mid = left + (right - left) / 2;
            pushDown(node, mid - left + 1, right - mid);
            int ans = 0;
            if (start <= mid) {
                ans += sumRange(node.left, left, mid, start, end);
            }
            if (end >= mid + 1) {
                ans += sumRange(node.right, mid + 1, right, start, end);
            }
            return ans;
        }
    }
    
    // 以下传进来的全都是原始的
    // 单点更新
    public void update(int index, int value) {
        update(index, index, value);
    }
    
    // 区域更新
    public void update(int start, int end, int value) {
        update(root, 1, size, start + 1, end + 1, value);
    }
    
    // 单点加
    public void add(int index, int value) {
        add(index, index, value);
    }
    
    // 区域加
    public void add(int index, int end, int value) {
        add(root, 1, size, index + 1, end + 1, value);
    }
    
    // 区域查询
    public int sumRange(int start, int end) {
        return sumRange(root, 1, size, start + 1, end + 1);
    }
    
}

class NumArray {
    
    private final DynamicSegmentTree segmentTree;
    
    public NumArray(int[] nums) {
        segmentTree = new DynamicSegmentTree(nums.length);
        // 初始化线段树
        for (int i = 0; i < nums.length; i++) {
            segmentTree.add(i, nums[i]);
        }
    }
    
    public void update(int index, int val) {
        segmentTree.update(index, val);
    }
    
    public int sumRange(int left, int right) {
        return segmentTree.sumRange(left, right);
    }
    
}
```

> - **线段树所需空间**

```java
// 如果线段树的范围是1 ~ n，那么记录信息的数组，开多大才够用？4n！
// 范围1 ~ n，形成的满二叉树高度会达到(log2 n + 2)，log以2为底
// 那么这棵满二叉树节点数会达到，2^(log2 n + 2)次方，log以2为底
// 2^(log2 n + 2) = 4n
public class Solution {

    // 范围l~r，信息存在独立数组的i位置
    // 返回递归展开的过程中出现的最大编号
    public static int maxi(int l, int r, int i) {
        if (l == r) {
            return i;
        } else {
            int mid = (l + r) >> 1;
            return Math.max(maxi(l, mid, i << 1), maxi(mid + 1, r, i << 1 | 1));
        }
    }

    public static void main(String[] args) {
        int n = 10000;
        int a = 0;
        int b = 0;
        double t = 0;
        for (int i = 1; i <= n; i++) {
            int space = maxi(1, i, 1);
            double times = (double) space / (double) i;
            System.out.println("范围[1~" + i + "]，" + "需要空间" + space + "，倍数=" + times);
            if (times > t) {
                a = i;
                b = space;
                t = times;
            }
        }
        System.out.println("其中的最大倍数，范围[1~" + a + "]，" + "需要空间" + b + "，倍数=" + t);
    }

}
```

> - **Question 3: 范围增加、范围查询、维护累加和模板**
>   - 从本段开始后面的模板都是新写法。

```java
// 线段树维护的信息类型
// 父范围上的某个信息，可以用O(1)的时间，从子范围的信息加工得到
// 满足的信息比如：累加和、最大值、最小值；不满足的信息比如：某范围上出现次数最多的数

// 线段树的经典功能，如下操作单次调用的时间复杂度为O(log n)
// 1，范围查询，包括范围内累加和、最大值、最小值等等信息
// 2，范围修改，包括范围内每个数都增加、重置等等操作

// 线段树的范围修改功能，想做到单次调用时间复杂度为O(log n)的要求：
// 一段范围上统一进行了某种修改操作，可以用O(1)的时间，就把这段范围维护的信息加工出来
// 满足的情况，比如：这段范围所有数字都加v，累加和可以快速的加工出来
// 不满足的情况，比如：这段范围上每个数字都逆序，累加和不能快速的加工出来

// 线段树的组织，以最经典的累加和举例
// 1. 线段树开始下标可以为1，也可以为0，下标从1开始是最经典的设定
// 2. 线段树需要在初始化时，就指定范围的规模[1 ~ n]，一旦确定不能更改
// 3. 任何一个大范围[l ~ r]，严格从中点mid，拆分成左范围[l ~ mid]、右范围[mid+1 ~ r]
// 4. 每个范围的信息，填写在独立的、连续数组sum中，最大的范围[1 ~ n]，把信息填写在sum[1]
// 5. 如果父范围把信息填写在sum[i]，那么左范围填写在sum[i*2]，右范围填写在sum[i*2+1]
// 6. 范围[l ~ r]和i值的对应，是由公式限制死的，由递归参数维护，无需去记录对应关系
// 这种设定最为经典，并且为最佳实践
import java.io.*;

public class Main {

    public static int MAXN = 100001;

    public static long[] arr = new long[MAXN];

    public static long[] sum = new long[MAXN << 2];

    public static long[] add = new long[MAXN << 2];

    // 累加和信息的汇总
    public static void up(int i) {
        // 父范围的累加和 = 左范围累加和 + 右范围累加和
        sum[i] = sum[i << 1] + sum[i << 1 | 1];
    }

    // 子范围的懒更新信息，发生的时间一定早于父范围上的懒更新信息
    // 如果修改操作不是范围修改，而是单点修改
    // 那么懒更新的机制不需要建立，也不需要懒信息的下发
    // 每次修改都是一走到底，反而更简单

    // 懒信息的下发
    public static void down(int i, int ln, int rn) {
        // 现判断是否需有懒信息需要下发
        if (add[i] != 0) {
            // 发左
            lazy(i << 1, add[i], ln);
            // 发右
            lazy(i << 1 | 1, add[i], rn);
            // 父范围懒信息清空
            add[i] = 0;
        }
    }

    // 当前来到l~r范围，对应的信息下标是i，范围上数字的个数是n = r-l+1
    // 现在收到一个懒更新任务 : l~r范围上每个数字增加v
    // 这个懒更新任务有可能是任务范围把当前线段树范围全覆盖导致的
    // 也有可能是父范围的懒信息下发下来的
    // 总之把线段树当前范围的sum数组和add数组调整好
    // 就不再继续往下下发了，懒住了
    public static void lazy(int i, long v, int n) {
        sum[i] += v * n;
        add[i] += v;
    }

    // 建树
    public static void build(int l, int r, int i) {
        if (l == r) {
            sum[i] = arr[l];
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            // 更新
            up(i);
        }
        add[i] = 0;
    }

    // 范围修改
    // jobl ~ jobr范围上每个数字增加jobv
    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            // 囊括住了所有，先懒
            lazy(i, jobv, r - l + 1);
        } else {
            int mid = (l + r) >> 1;
            // 下发，把该范围上积攒的懒信息，往下只下发一层
            down(i, mid - l + 1, r - mid);
            // 然后决定当前任务是否要去往，左范围、右范围，继续调用子递归过程
            if (jobl <= mid) {
                add(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                add(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            // 更新，子递归完成后，利用左右范围的sum信息，把当前范围的sum[i]信息修改正确
            up(i);
        }
    }

    // 查询累加和
    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            // 囊括直接返回
            return sum[i];
        }
        int mid = (l + r) >> 1;
        // 下发
        down(i, mid - l + 1, r - mid);
        long ans = 0;
        if (jobl <= mid) {
            ans += query(jobl, jobr, l, mid, i << 1);
        }
        if (jobr > mid) {
            ans += query(jobl, jobr, mid + 1, r, i << 1 | 1);
        }
        return ans;
    }

    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StreamTokenizer in = new StreamTokenizer(br);
        PrintWriter out = new PrintWriter(new OutputStreamWriter(System.out));
        in.nextToken();
        int n = (int) in.nval;
        in.nextToken();
        int m = (int) in.nval;
        for (int i = 1; i <= n; i++) {
            in.nextToken();
            arr[i] = (long) in.nval;
        }
        build(1, n, 1);
        long jobv;
        for (int i = 1, op, jobl, jobr; i <= m; i++) {
            in.nextToken();
            op = (int) in.nval;
            if (op == 1) {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                in.nextToken();
                jobv = (long) in.nval;
                add(jobl, jobr, jobv, 1, n, 1);
            } else {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                out.println(query(jobl, jobr, 1, n, 1));
            }
        }
        out.flush();
        out.close();
        br.close();
    }

}
```

> - **范围增加、范围查询、维护最大值模板**

```java
public class Main {

    public static int MAXN = 100001;

    public static long[] arr = new long[MAXN];

    public static long[] max = new long[MAXN << 2];

    public static long[] add = new long[MAXN << 2];

    public static void up(int i) {
        max[i] = Math.max(max[i << 1], max[i << 1 | 1]);
    }

    public static void down(int i) {
        if (add[i] != 0) {
            lazy(i << 1, add[i]);
            lazy(i << 1 | 1, add[i]);
            add[i] = 0;
        }
    }

    public static void lazy(int i, long v) {
        // 不管最大值是多少，加上去就完事了
        max[i] += v;
        add[i] += v;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            max[i] = arr[l];
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        add[i] = 0;
    }

    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            lazy(i, jobv);
        } else {
            down(i);
            int mid = (l + r) >> 1;
            if (jobl <= mid) {
                add(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                add(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    // 查询换成查最大值即可
    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        }
        down(i);
        int mid = (l + r) >> 1;
        long ans = Long.MIN_VALUE;
        if (jobl <= mid) {
            ans = Math.max(ans, query(jobl, jobr, l, mid, i << 1));
        }
        if (jobr > mid) {
            ans = Math.max(ans, query(jobl, jobr, mid + 1, r, i << 1 | 1));
        }
        return ans;
    }

    // 对数器逻辑
    // 展示了线段树的建立和使用
    // 使用验证结构来检查线段树是否正常工作
    public static void main(String[] args) {
        System.out.println("测试开始");
        int n = 1000;
        int v = 2000;
        int t = 5000000;
        // 生成随机值填入arr数组
        randomArray(n, v);
        // 建立线段树
        build(1, n, 1);
        // 生成验证的结构
        long[] check = new long[n + 1];
        for (int i = 1; i <= n; i++) {
            check[i] = arr[i];
        }
        for (int i = 1; i <= t; i++) {
            // 生成操作类型
            // op = 0 增加操作
            // op = 1 查询操作
            int op = (int) (Math.random() * 2);
            // 下标从1开始，不从0开始，生成两个随机下标
            int a = (int) (Math.random() * n) + 1;
            int b = (int) (Math.random() * n) + 1;
            // 确保jobl <= jobr
            int jobl = Math.min(a, b);
            int jobr = Math.max(a, b);
            if (op == 0) {
                // 增加操作
                // 线段树、验证结构同步增加
                int jobv = (int) (Math.random() * v * 2) - v;
                add(jobl, jobr, jobv, 1, n, 1);
                checkAdd(check, jobl, jobr, jobv);
            } else {
                // 查询操作
                // 线段树、验证结构同步查询
                // 比对答案
                long ans1 = query(jobl, jobr, 1, n, 1);
                long ans2 = checkQuery(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            }
        }
        System.out.println("测试结束");
    }

    // 生成随机值填入arr数组
    // 为了验证
    public static void randomArray(int n, int v) {
        for (int i = 1; i <= n; i++) {
            arr[i] = (long) (Math.random() * v);
        }
    }

    // 验证结构的增加
    // 暴力增加
    // 为了验证
    public static void checkAdd(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] += jobv;
        }
    }

    // 验证结构的查询
    // 暴力查询
    // 为了验证
    public static long checkQuery(long[] check, int jobl, int jobr) {
        long ans = Long.MIN_VALUE;
        for (int i = jobl; i <= jobr; i++) {
            ans = Math.max(ans, check[i]);
        }
        return ans;
    }

}
```

> - **范围重置、范围查询、维护累加和模板**

```java
public class Main {

    public static int MAXN = 100001;

    public static long[] arr = new long[MAXN];

    public static long[] sum = new long[MAXN << 2];

    public static long[] change = new long[MAXN << 2];

    // 当update[i]为true时change[i]才有效
    public static boolean[] update = new boolean[MAXN << 2];

    public static void up(int i) {
        sum[i] = sum[i << 1] + sum[i << 1 | 1];
    }

    public static void down(int i, int ln, int rn) {
        // 需要重置
        if (update[i]) {
            lazy(i << 1, change[i], ln);
            lazy(i << 1 | 1, change[i], rn);
            // 当前失效
            // change[i]等于0无所谓了
            update[i] = false;
        }
    }

    public static void lazy(int i, long v, int n) {
        sum[i] = v * n;
        change[i] = v;
        update[i] = true;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            sum[i] = arr[l];
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        // 最开始时没有更新操作进入
        change[i] = 0;
        update[i] = false;
    }

    public static void update(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            lazy(i, jobv, r - l + 1);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                update(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                update(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        }
        int mid = (l + r) >> 1;
        down(i, mid - l + 1, r - mid);
        long ans = 0;
        if (jobl <= mid) {
            ans += query(jobl, jobr, l, mid, i << 1);
        }
        if (jobr > mid) {
            ans += query(jobl, jobr, mid + 1, r, i << 1 | 1);
        }
        return ans;
    }

    // 对数器逻辑
    // 展示了线段树的建立和使用
    // 使用验证结构来检查线段树是否正常工作
    public static void main(String[] args) {
        System.out.println("测试开始");
        int n = 1000;
        int v = 2000;
        int t = 5000000;
        // 生成随机值填入arr数组
        randomArray(n, v);
        // 建立线段树
        build(1, n, 1);
        // 生成验证的结构
        long[] check = new long[n + 1];
        for (int i = 1; i <= n; i++) {
            check[i] = arr[i];
        }
        for (int i = 1; i <= t; i++) {
            // 生成操作类型
            // op = 0 更新操作
            // op = 1 查询操作
            int op = (int) (Math.random() * 2);
            // 下标从1开始，不从0开始，生成两个随机下标
            int a = (int) (Math.random() * n) + 1;
            int b = (int) (Math.random() * n) + 1;
            // 确保jobl <= jobr
            int jobl = Math.min(a, b);
            int jobr = Math.max(a, b);
            if (op == 0) {
                // 更新操作
                // 线段树、验证结构同步更新
                int jobv = (int) (Math.random() * v * 2) - v;
                update(jobl, jobr, jobv, 1, n, 1);
                checkUpdate(check, jobl, jobr, jobv);
            } else {
                // 查询操作
                // 线段树、验证结构同步查询
                // 比对答案
                long ans1 = query(jobl, jobr, 1, n, 1);
                long ans2 = checkQuery(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            }
        }
        System.out.println("测试结束");
    }

    // 生成随机值填入arr数组
    // 为了验证
    public static void randomArray(int n, int v) {
        for (int i = 1; i <= n; i++) {
            arr[i] = (long) (Math.random() * v);
        }
    }

    // 验证结构的更新
    // 暴力更新
    // 为了验证
    public static void checkUpdate(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] = jobv;
        }
    }

    // 验证结构的查询
    // 暴力查询
    // 为了验证
    public static long checkQuery(long[] check, int jobl, int jobr) {
        long ans = 0;
        for (int i = jobl; i <= jobr; i++) {
            ans += check[i];
        }
        return ans;
    }

}
```

> - **范围重置、范围查询、维护最大值模板**

```java
public class Main {

    public static int MAXN = 100001;

    public static long[] arr = new long[MAXN];

    public static long[] max = new long[MAXN << 2];

    public static long[] change = new long[MAXN << 2];

    public static boolean[] update = new boolean[MAXN << 2];

    public static void up(int i) {
        max[i] = Math.max(max[i << 1], max[i << 1 | 1]);
    }

    public static void down(int i) {
        if (update[i]) {
            lazy(i << 1, change[i]);
            lazy(i << 1 | 1, change[i]);
            update[i] = false;
        }
    }

    public static void lazy(int i, long v) {
        // 最大值直接变成替换后的值即可
        max[i] = v;
        change[i] = v;
        update[i] = true;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            max[i] = arr[l];
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        change[i] = 0;
        update[i] = false;
    }

    public static void update(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            lazy(i, jobv);
        } else {
            down(i);
            int mid = (l + r) >> 1;
            if (jobl <= mid) {
                update(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                update(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        }
        down(i);
        int mid = (l + r) >> 1;
        // 先认为最大值最小，后面再分别比较即可
        long ans = Long.MIN_VALUE;
        if (jobl <= mid) {
            ans = Math.max(ans, query(jobl, jobr, l, mid, i << 1));
        }
        if (jobr > mid) {
            ans = Math.max(ans, query(jobl, jobr, mid + 1, r, i << 1 | 1));
        }
        return ans;
    }

    // 对数器逻辑
    // 展示了线段树的建立和使用
    // 使用验证结构来检查线段树是否正常工作
    public static void main(String[] args) {
        System.out.println("测试开始");
        int n = 1000;
        int v = 2000;
        int t = 5000000;
        // 生成随机值填入arr数组
        randomArray(n, v);
        // 建立线段树
        build(1, n, 1);
        // 生成验证的结构
        long[] check = new long[n + 1];
        for (int i = 1; i <= n; i++) {
            check[i] = arr[i];
        }
        for (int i = 1; i <= t; i++) {
            // 生成操作类型
            // op = 0 更新操作
            // op = 1 查询操作
            int op = (int) (Math.random() * 2);
            // 下标从1开始，不从0开始，生成两个随机下标
            int a = (int) (Math.random() * n) + 1;
            int b = (int) (Math.random() * n) + 1;
            // 确保jobl <= jobr
            int jobl = Math.min(a, b);
            int jobr = Math.max(a, b);
            if (op == 0) {
                // 更新操作
                // 线段树、验证结构同步更新
                int jobv = (int) (Math.random() * v * 2) - v;
                update(jobl, jobr, jobv, 1, n, 1);
                checkUpdate(check, jobl, jobr, jobv);
            } else {
                // 查询操作
                // 线段树、验证结构同步查询
                // 比对答案
                long ans1 = query(jobl, jobr, 1, n, 1);
                long ans2 = checkQuery(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            }
        }
        System.out.println("测试结束");
    }

    // 生成随机值填入arr数组
    // 为了验证
    public static void randomArray(int n, int v) {
        for (int i = 1; i <= n; i++) {
            arr[i] = (long) (Math.random() * v);
        }
    }

    // 验证结构的更新
    // 暴力更新
    // 为了验证
    public static void checkUpdate(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] = jobv;
        }
    }

    // 验证结构的查询
    // 暴力查询
    // 为了验证
    public static long checkQuery(long[] check, int jobl, int jobr) {
        long ans = Long.MIN_VALUE;
        for (int i = jobl; i <= jobr; i++) {
            ans = Math.max(ans, check[i]);
        }
        return ans;
    }

}
```

> - **范围增加、范围重置、范围查询、维护累加和模板**

```java
// 线段树常见方法一览
// void up(i...) : 根据子范围的查询信息，把父范围的查询信息更新正确
// void down(i...) : 父范围的懒信息，往下只下发一层，给左范围、右范围，然后父范围的懒信息清空
// void lazy(i...) : 当前范围被修改任务全覆盖时 或 父范围发下来的懒更新时，信息数组们如何修改
// void build(l, r, i)  : 建树
// void update(jobl, jobr, jobv, l, r, i) : 范围上数值的重置任务
// void add(jobl, jobr, jobv, l, r, i) : 范围上数值的增加任务
// int query(jobl, jobr, l, r, i) : 范围上的信息查询任务

public class Main {

    public static int MAXN = 1000001;

    public static long[] arr = new long[MAXN];

    public static long[] sum = new long[MAXN << 2];

    public static long[] add = new long[MAXN << 2];

    public static long[] change = new long[MAXN << 2];

    public static boolean[] update = new boolean[MAXN << 2];

    public static void up(int i) {
        sum[i] = sum[i << 1] + sum[i << 1 | 1];
    }

    // 多种修改操作之间的优先级整理
    public static void down(int i, int ln, int rn) {
        // 一段范围的更新操作会彻底取消之前的增加操作
        // 一段范围的增加操作不会取消之前的更新操作，而是在之前更新操作的基础上进行增加
        // 这两点在懒更新时需要得到体现
        if (update[i]) {
            updateLazy(i << 1, change[i], ln);
            updateLazy(i << 1 | 1, change[i], rn);
            update[i] = false;
        }
        if (add[i] != 0) {
            addLazy(i << 1, add[i], ln);
            addLazy(i << 1 | 1, add[i], rn);
            add[i] = 0;
        }
    }

    public static void updateLazy(int i, long v, int n) {
        sum[i] = v * n;
        // 覆盖掉所有add
        add[i] = 0;
        change[i] = v;
        update[i] = true;
    }

    public static void addLazy(int i, long v, int n) {
        sum[i] += v * n;
        add[i] += v;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            sum[i] = arr[l];
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        add[i] = 0;
        change[i] = 0;
        update[i] = false;
    }

    public static void update(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            updateLazy(i, jobv, r - l + 1);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                update(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                update(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            addLazy(i, jobv, r - l + 1);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                add(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                add(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        }
        int mid = (l + r) >> 1;
        down(i, mid - l + 1, r - mid);
        long ans = 0;
        if (jobl <= mid) {
            ans += query(jobl, jobr, l, mid, i << 1);
        }
        if (jobr > mid) {
            ans += query(jobl, jobr, mid + 1, r, i << 1 | 1);
        }
        return ans;
    }

    public static void main(String[] args) {
        System.out.println("测试开始");
        int n = 1000;
        int v = 2000;
        int t = 5000000;
        // 生成随机值填入arr数组
        randomArray(n, v);
        // 建立线段树
        build(1, n, 1);
        // 生成验证的结构
        long[] check = new long[n + 1];
        for (int i = 1; i <= n; i++) {
            check[i] = arr[i];
        }
        for (int i = 1; i <= t; i++) {
            // 生成操作类型
            // op = 0 增加操作
            // op = 1 更新操作
            // op = 2 查询操作
            int op = (int) (Math.random() * 3);
            // 下标从1开始，不从0开始，生成两个随机下标
            int a = (int) (Math.random() * n) + 1;
            int b = (int) (Math.random() * n) + 1;
            // 确保jobl <= jobr
            int jobl = Math.min(a, b);
            int jobr = Math.max(a, b);
            if (op == 0) {
                // 增加操作
                // 线段树、验证结构同步增加
                int jobv = (int) (Math.random() * v * 2) - v;
                add(jobl, jobr, jobv, 1, n, 1);
                checkAdd(check, jobl, jobr, jobv);
            } else if (op == 1) {
                // 更新操作
                // 线段树、验证结构同步更新
                int jobv = (int) (Math.random() * v * 2) - v;
                update(jobl, jobr, jobv, 1, n, 1);
                checkUpdate(check, jobl, jobr, jobv);
            } else {
                // 查询操作
                // 线段树、验证结构同步查询
                // 比对答案
                long ans1 = query(jobl, jobr, 1, n, 1);
                long ans2 = checkQuery(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            }
        }
        System.out.println("测试结束");
    }

    // 生成随机值填入arr数组
    // 为了验证
    public static void randomArray(int n, int v) {
        for (int i = 1; i <= n; i++) {
            arr[i] = (long) (Math.random() * v);
        }
    }

    // 验证结构的增加
    // 暴力增加
    // 为了验证
    public static void checkAdd(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] += jobv;
        }
    }

    // 验证结构的更新
    // 暴力更新
    // 为了验证
    public static void checkUpdate(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] = jobv;
        }
    }

    // 验证结构的查询
    // 暴力查询
    // 为了验证
    public static long checkQuery(long[] check, int jobl, int jobr) {
        long ans = 0;
        for (int i = jobl; i <= jobr; i++) {
            ans += check[i];
        }
        return ans;
    }

}
```

> - **Question 4: 范围增加、范围重置、范围查询、维护最大值模板**

```java
import java.io.*;

public class Main {

    public static int MAXN = 1000001;

    public static long[] arr = new long[MAXN];

    public static long[] max = new long[MAXN << 2];

    public static long[] add = new long[MAXN << 2];

    public static long[] change = new long[MAXN << 2];

    public static boolean[] update = new boolean[MAXN << 2];

    public static void up(int i) {
        max[i] = Math.max(max[i << 1], max[i << 1 | 1]);
    }

    public static void down(int i) {
        if (update[i]) {
            updateLazy(i << 1, change[i]);
            updateLazy(i << 1 | 1, change[i]);
            update[i] = false;
        }
        if (add[i] != 0) {
            addLazy(i << 1, add[i]);
            addLazy(i << 1 | 1, add[i]);
            add[i] = 0;
        }
    }

    public static void updateLazy(int i, long v) {
        max[i] = v;
        add[i] = 0;
        change[i] = v;
        update[i] = true;
    }

    public static void addLazy(int i, long v) {
        max[i] += v;
        add[i] += v;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            max[i] = arr[l];
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        add[i] = 0;
        change[i] = 0;
        update[i] = false;
    }

    public static void update(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            updateLazy(i, jobv);
        } else {
            int mid = (l + r) >> 1;
            down(i);
            if (jobl <= mid) {
                update(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                update(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            addLazy(i, jobv);
        } else {
            int mid = (l + r) >> 1;
            down(i);
            if (jobl <= mid) {
                add(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                add(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        }
        int mid = (l + r) >> 1;
        down(i);
        long ans = Long.MIN_VALUE;
        if (jobl <= mid) {
            ans = Math.max(ans, query(jobl, jobr, l, mid, i << 1));
        }
        if (jobr > mid) {
            ans = Math.max(ans, query(jobl, jobr, mid + 1, r, i << 1 | 1));
        }
        return ans;
    }

    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StreamTokenizer in = new StreamTokenizer(br);
        PrintWriter out = new PrintWriter(new OutputStreamWriter(System.out));
        in.nextToken();
        int n = (int) in.nval;
        in.nextToken();
        int m = (int) in.nval;
        for (int i = 1; i <= n; i++) {
            in.nextToken();
            arr[i] = (long) in.nval;
        }
        build(1, n, 1);
        long jobv;
        for (int i = 1, op, jobl, jobr; i <= m; i++) {
            in.nextToken();
            op = (int) in.nval;
            if (op == 1) {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                in.nextToken();
                jobv = (long) in.nval;
                update(jobl, jobr, jobv, 1, n, 1);
            } else if (op == 2) {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                in.nextToken();
                jobv = (long) in.nval;
                add(jobl, jobr, jobv, 1, n, 1);
            } else {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                out.println(query(jobl, jobr, 1, n, 1));
            }
        }
        out.flush();
        out.close();
        br.close();
    }

}
```

> - **Question 5: 开点线段树**

```java
// 开点线段树，可以支持很大的范围，一开始不为每个范围都分配空间，当真的需要开辟左侧、右侧的空间时，再临时申请，父范围的空间编号i，利用cnt自增给左右两侧申请的空间，记录在left[i]和right[i]里，除此之外和线段树再无区别
// 开点线段树适用的范围：需要支持的范围很大，但实际操作数量并不大，此时用开点线段树试试，俗称莽一把，使用空间约等于 : 操作数量 * 树高 * 2，适量调大即可
// 注意：测试通过的标准稍严，开点线段树很容易被卡，不过只有比赛才可能会卡，笔试一般不会卡
// 开点线段树的劣势：常数时间不好，相比其他方法还是比较浪费空间
// 开点线段树的优势：分析难度低，往往理解了开点线段树就很容易想到并轻易使用
// 大多数情况下都可以被其他方法替代，比如离散化、有序表、堆结构等等
// 如果数据量允许，莽一把能节省很多思考的时间，但是往往不是最优解，只是时间复杂度不差而已
// 注意：开点线段树不可被替代的用法是用于线段树的合并与分裂，但是这一话题和树链剖分结合比较紧密
import java.io.*;
import java.util.Arrays;

public class Main {

    // 范围1 ~ 10^9，线段树高度差不多30
    // 查询次数1000，每次查询都有左右两条边线
    // 所以空间占用差不多1000 * 30 * 2 = 60000
    // 适当调大即可
    public static int LIMIT = 80001;

    public static int cnt;

    public static int[] left = new int[LIMIT];

    public static int[] right = new int[LIMIT];

    public static long[] sum = new long[LIMIT];

    public static long[] add = new long[LIMIT];

    public static void up(int h, int l, int r) {
        sum[h] = sum[l] + sum[r];
    }

    public static void down(int i, int ln, int rn) {
        if (add[i] != 0) {
            // 懒更新任务下发
            // 那左右两侧的空间需要准备好
            if (left[i] == 0) {
                left[i] = ++cnt;
            }
            if (right[i] == 0) {
                right[i] = ++cnt;
            }
            lazy(left[i], add[i], ln);
            lazy(right[i], add[i], rn);
            add[i] = 0;
        }
    }

    public static void lazy(int i, long v, int n) {
        sum[i] += v * n;
        add[i] += v;
    }

    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            lazy(i, jobv, r - l + 1);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                // 不得不去左侧才会申请
                if (left[i] == 0) {
                    left[i] = ++cnt;
                }
                add(jobl, jobr, jobv, l, mid, left[i]);
            }
            if (jobr > mid) {
                // 不得不去右侧才会申请
                if (right[i] == 0) {
                    right[i] = ++cnt;
                }
                add(jobl, jobr, jobv, mid + 1, r, right[i]);
            }
            up(i, left[i], right[i]);
        }
    }

    public static long query(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        }
        int mid = (l + r) >> 1;
        down(i, mid - l + 1, r - mid);
        long ans = 0;
        if (jobl <= mid) {
            // 发现左侧申请过空间才有必要去查询
            // 如果左侧从来没有申请过空间那查询结果就是0
            if (left[i] != 0) {
                ans += query(jobl, jobr, l, mid, left[i]);
            }
        }
        if (jobr > mid) {
            // 发现右侧申请过空间才有必要去查询
            // 如果右侧从来没有申请过空间那查询结果就是0
            if (right[i] != 0) {
                ans += query(jobl, jobr, mid + 1, r, right[i]);
            }
        }
        return ans;
    }

    // 如果一次会执行多组测试数组
    // 那么每组测试完成后要clear空间
    public static void clear() {
        Arrays.fill(left, 1, cnt + 1, 0);
        Arrays.fill(right, 1, cnt + 1, 0);
        Arrays.fill(sum, 1, cnt + 1, 0);
        Arrays.fill(add, 1, cnt + 1, 0);
    }

    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StreamTokenizer in = new StreamTokenizer(br);
        PrintWriter out = new PrintWriter(new OutputStreamWriter(System.out));
        in.nextToken();
        int n = (int) in.nval;
        in.nextToken();
        int m = (int) in.nval;
        cnt = 1;
        long jobv;
        for (int i = 1, op, jobl, jobr; i <= m; i++) {
            in.nextToken();
            op = (int) in.nval;
            if (op == 1) {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                in.nextToken();
                jobv = (long) in.nval;
                add(jobl, jobr, jobv, 1, n, 1);
            } else {
                in.nextToken();
                jobl = (int) in.nval;
                in.nextToken();
                jobr = (int) in.nval;
                out.println(query(jobl, jobr, 1, n, 1));
            }
        }
        // 本题每组测试数据都单独运行
        // 可以不写clear方法
        // 但是如果多组测试数据串行调用
        // 就需要加上清空逻辑
        clear();
        out.flush();
        out.close();
        br.close();
    }

}
```

> - **Question 6: 吉如一线段树**
>   - 论文参考[线段树区间最值操作与历史最值问题](./references/线段树区间最值操作与历史最值问题-吉如一.pdf)。

```java
// 对数器验证
public class Main {

    public static int MAXN = 100001;

    // 假设初始数组中的值不会出现比LOWEST还小的值
    // 假设更新操作时jobv的数值也不会出现比LOWEST还小的值
    public static int LOWEST = -100001;

    // 原始数组
    public static int[] arr = new int[MAXN];

    // 累加和
    public static long[] sum = new long[MAXN << 2];

    // 最大值
    // 既是查询信息也是懒更新信息
    public static int[] max = new int[MAXN << 2];

    // 最大值个数
    public static int[] cnt = new int[MAXN << 2];

    // 严格次大值(second max)
    public static int[] sem = new int[MAXN << 2];

    public static void up(int i) {
        int l = i << 1;
        int r = i << 1 | 1;
        sum[i] = sum[l] + sum[r];
        max[i] = Math.max(max[l], max[r]);
        if (max[l] > max[r]) {
            cnt[i] = cnt[l];
            sem[i] = Math.max(sem[l], max[r]);
        } else if (max[l] < max[r]) {
            cnt[i] = cnt[r];
            sem[i] = Math.max(max[l], sem[r]);
        } else {
            cnt[i] = cnt[l] + cnt[r];
            sem[i] = Math.max(sem[l], sem[r]);
        }
    }

    public static void down(int i) {
        lazy(i << 1, max[i]);
        lazy(i << 1 | 1, max[i]);
    }

    // 一定是没有颠覆掉次大值的懒更新信息下发，也就是说：
    // 最大值被压成v，并且v > 严格次大值的情况下
    // sum和max怎么调整
    public static void lazy(int i, int v) {
        if (v < max[i]) {
            sum[i] -= ((long) max[i] - v) * cnt[i];
            max[i] = v;
        }
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            sum[i] = max[i] = arr[l];
            cnt[i] = 1;
            sem[i] = LOWEST;
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
    }

    public static void setMin(int jobl, int jobr, int jobv, int l, int r, int i) {
        if (jobv >= max[i]) {
            return;
        }
        if (jobl <= l && r <= jobr && sem[i] < jobv) {
            lazy(i, jobv);
        } else {
            // 1) 任务没有全包
            // 2) jobv <= sem[i]
            down(i);
            int mid = (l + r) >> 1;
            if (jobl <= mid) {
                setMin(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                setMin(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static int queryMax(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        }
        down(i);
        int mid = (l + r) >> 1;
        int ans = Integer.MIN_VALUE;
        if (jobl <= mid) {
            ans = Math.max(ans, queryMax(jobl, jobr, l, mid, i << 1));
        }
        if (jobr > mid) {
            ans = Math.max(ans, queryMax(jobl, jobr, mid + 1, r, i << 1 | 1));
        }
        return ans;
    }

    public static long querySum(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        }
        down(i);
        int mid = (l + r) >> 1;
        long ans = 0;
        if (jobl <= mid) {
            ans += querySum(jobl, jobr, l, mid, i << 1);
        }
        if (jobr > mid) {
            ans += querySum(jobl, jobr, mid + 1, r, i << 1 | 1);
        }
        return ans;
    }

    public static void main(String[] args) {
        System.out.println("测试开始");
        int n = 2000;
        int v = 5000;
        int t = 1000000;
        randomArray(n, v);
        int[] check = new int[n + 1];
        for (int i = 1; i <= n; i++) {
            check[i] = arr[i];
        }
        build(1, n, 1);
        for (int i = 1, op, a, b, jobl, jobr, jobv; i <= t; i++) {
            op = (int) (Math.random() * 3);
            a = (int) (Math.random() * n) + 1;
            b = (int) (Math.random() * n) + 1;
            jobl = Math.min(a, b);
            jobr = Math.max(a, b);
            if (op == 0) {
                jobv = (int) (Math.random() * v * 2) - v;
                setMin(jobl, jobr, jobv, 1, n, 1);
                checkSetMin(check, jobl, jobr, jobv);
            } else if (op == 1) {
                int ans1 = queryMax(jobl, jobr, 1, n, 1);
                int ans2 = checkQueryMax(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            } else {
                long ans1 = querySum(jobl, jobr, 1, n, 1);
                long ans2 = checkQuerySum(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            }
        }
        System.out.println("测试结束");
    }

    // 为了验证
    public static void randomArray(int n, int v) {
        for (int i = 1; i <= n; i++) {
            arr[i] = (int) (Math.random() * v * 2) - v;
        }
    }

    // 为了验证
    public static void checkSetMin(int[] check, int jobl, int jobr, int jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] = Math.min(check[i], jobv);
        }
    }

    // 为了验证
    public static int checkQueryMax(int[] check, int jobl, int jobr) {
        int ans = Integer.MIN_VALUE;
        for (int i = jobl; i <= jobr; i++) {
            ans = Math.max(ans, check[i]);
        }
        return ans;
    }

    // 为了验证
    public static long checkQuerySum(int[] check, int jobl, int jobr) {
        long ans = 0;
        for (int i = jobl; i <= jobr; i++) {
            ans += check[i];
        }
        return ans;
    }

}

// OJ

// 每个数字都增加的范围修改操作发生后，setMin暴力执行的势能增加多少？
// 增加幅度不超过(log n)平方规模，这个量很小
// setMin的懒更新只会削弱最大值，需要实现setMinLazy函数
// add的懒更新会增加所有数字的值，需要实现addLazy函数
// 代码层次的小优化：可以只实现一个lazy函数，设计最大值增加幅度、其他值增加幅度两个入参即可

import java.io.*;

public class Main {

    public static int MAXN = 1000001;

    public static int LOWEST = -1;

    public static long[] sum = new long[MAXN << 2];

    public static int[] max = new int[MAXN << 2];

    public static int[] cnt = new int[MAXN << 2];

    public static int[] sem = new int[MAXN << 2];

    public static void up(int i) {
        int l = i << 1;
        int r = i << 1 | 1;
        sum[i] = sum[l] + sum[r];
        max[i] = Math.max(max[l], max[r]);
        if (max[l] > max[r]) {
            cnt[i] = cnt[l];
            sem[i] = Math.max(sem[l], max[r]);
        } else if (max[l] < max[r]) {
            cnt[i] = cnt[r];
            sem[i] = Math.max(max[l], sem[r]);
        } else {
            cnt[i] = cnt[l] + cnt[r];
            sem[i] = Math.max(sem[l], sem[r]);
        }
    }

    public static void down(int i) {
        lazy(i << 1, max[i]);
        lazy(i << 1 | 1, max[i]);
    }

    // 一定是没有颠覆掉次大值的懒更新信息下发，也就是说：
    // 最大值被压成v，并且v > 严格次大值的情况下
    // sum和max怎么调整
    public static void lazy(int i, int v) {
        if (v < max[i]) {
            sum[i] -= ((long) max[i] - v) * cnt[i];
            max[i] = v;
        }
    }

    public static void build(int l, int r, int i) throws IOException {
        if (l == r) {
            // 不能生成原始数组然后build
            // 因为这道题空间非常极限
            // 生成原始数组然后build
            // 空间就是会超过限制
            // 所以build的过程直接从输入流读入
            // 一般情况下不会这么极限的
            in.nextToken();
            sum[i] = max[i] = (int) in.nval;
            cnt[i] = 1;
            sem[i] = LOWEST;
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
    }

    public static void setMin(int jobl, int jobr, int jobv, int l, int r, int i) {
        if (jobv >= max[i]) {
            return;
        }
        if (jobl <= l && r <= jobr && sem[i] < jobv) {
            lazy(i, jobv);
        } else {
            down(i);
            int mid = (l + r) >> 1;
            if (jobl <= mid) {
                setMin(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                setMin(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static int queryMax(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        }
        down(i);
        int mid = (l + r) >> 1;
        int ans = Integer.MIN_VALUE;
        if (jobl <= mid) {
            ans = Math.max(ans, queryMax(jobl, jobr, l, mid, i << 1));
        }
        if (jobr > mid) {
            ans = Math.max(ans, queryMax(jobl, jobr, mid + 1, r, i << 1 | 1));
        }
        return ans;
    }

    public static long querySum(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        }
        down(i);
        int mid = (l + r) >> 1;
        long ans = 0;
        if (jobl <= mid) {
            ans += querySum(jobl, jobr, l, mid, i << 1);
        }
        if (jobr > mid) {
            ans += querySum(jobl, jobr, mid + 1, r, i << 1 | 1);
        }
        return ans;
    }

    // 为了不生成原始数组
    // 让build函数可以直接从输入流拿数据
    // 所以把输入输出流定义成全局静态变量
    public static BufferedReader br = new BufferedReader(new InputStreamReader(System.in));

    public static StreamTokenizer in = new StreamTokenizer(br);

    public static PrintWriter out = new PrintWriter(new OutputStreamWriter(System.out));

    public static void main(String[] args) throws IOException {
        in.nextToken();
        int testCases = (int) in.nval;
        for (int t = 1; t <= testCases; t++) {
            in.nextToken();
            int n = (int) in.nval;
            in.nextToken();
            int m = (int) in.nval;
            build(1, n, 1);
            for (int i = 1, op, jobl, jobr, jobv; i <= m; i++) {
                in.nextToken();
                op = (int) in.nval;
                if (op == 0) {
                    in.nextToken();
                    jobl = (int) in.nval;
                    in.nextToken();
                    jobr = (int) in.nval;
                    in.nextToken();
                    jobv = (int) in.nval;
                    setMin(jobl, jobr, jobv, 1, n, 1);
                } else if (op == 1) {
                    in.nextToken();
                    jobl = (int) in.nval;
                    in.nextToken();
                    jobr = (int) in.nval;
                    out.println(queryMax(jobl, jobr, 1, n, 1));
                } else {
                    in.nextToken();
                    jobl = (int) in.nval;
                    in.nextToken();
                    jobr = (int) in.nval;
                    out.println(querySum(jobl, jobr, 1, n, 1));
                }
            }
        }
        out.flush();
        out.close();
        br.close();
    }

}
```

> - **Question 7**

```java
public class Main {

    public static int MAXN = 500001;

    public static long LOWEST = Long.MIN_VALUE;

    // 原始数组
    public static int[] arr = new int[MAXN];

    // 累加和信息(查询信息)
    public static long[] sum = new long[MAXN << 2];

    // 最大值信息(只是查询信息，不再是懒更新信息，懒更新功能被maxAdd数组替代了)
    public static long[] max = new long[MAXN << 2];

    // 最大值个数(查询信息)
    public static int[] cnt = new int[MAXN << 2];

    // 严格次大值(查询信息)
    public static long[] sem = new long[MAXN << 2];

    // 最大值的增加幅度(懒更新信息)
    public static long[] maxAdd = new long[MAXN << 2];

    // 除最大值以外其他数字的增加幅度(懒更新信息)
    public static long[] otherAdd = new long[MAXN << 2];

    public static void up(int i) {
        int l = i << 1;
        int r = i << 1 | 1;
        sum[i] = sum[l] + sum[r];
        max[i] = Math.max(max[l], max[r]);
        if (max[l] > max[r]) {
            cnt[i] = cnt[l];
            sem[i] = Math.max(sem[l], max[r]);
        } else if (max[l] < max[r]) {
            cnt[i] = cnt[r];
            sem[i] = Math.max(max[l], sem[r]);
        } else {
            cnt[i] = cnt[l] + cnt[r];
            sem[i] = Math.max(sem[l], sem[r]);
        }
    }

    public static void lazy(int i, int n, long maxAddv, long otherAddv) {
        sum[i] += maxAddv * cnt[i] + otherAddv * (n - cnt[i]);
        max[i] += maxAddv;
        sem[i] += sem[i] == LOWEST ? 0 : otherAddv;
        maxAdd[i] += maxAddv;
        otherAdd[i] += otherAddv;
    }

    public static void down(int i, int ln, int rn) {
        int l = i << 1;
        int r = i << 1 | 1;
        // 为什么拿全局最大值不写成 : tmp = max[i]
        // 因为父亲范围的最大值可能已经被懒更新任务修改过了
        // 现在希望拿的是懒更新之前的最大值
        // 子范围的max值没有修改过，所以写成 : tmp = Math.max(max[l], max[r])
        long tmp = Math.max(max[l], max[r]);
        if (max[l] == tmp) {
            lazy(l, ln, maxAdd[i], otherAdd[i]);
        } else {
            lazy(l, ln, otherAdd[i], otherAdd[i]);
        }
        if (max[r] == tmp) {
            lazy(r, rn, maxAdd[i], otherAdd[i]);
        } else {
            lazy(r, rn, otherAdd[i], otherAdd[i]);
        }
        maxAdd[i] = otherAdd[i] = 0;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            sum[i] = max[i] = arr[l];
            sem[i] = LOWEST;
            cnt[i] = 1;
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        maxAdd[i] = otherAdd[i] = 0;
    }

    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            lazy(i, r - l + 1, jobv, jobv);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                add(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                add(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static void setMin(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobv >= max[i]) {
            return;
        }
        if (jobl <= l && r <= jobr && sem[i] < jobv) {
            lazy(i, r - l + 1, jobv - max[i], 0);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                setMin(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                setMin(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static long querySum(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            long ans = 0;
            if (jobl <= mid) {
                ans += querySum(jobl, jobr, l, mid, i << 1);
            }
            if (jobr > mid) {
                ans += querySum(jobl, jobr, mid + 1, r, i << 1 | 1);
            }
            return ans;
        }
    }

    public static long queryMax(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            Long ans = Long.MIN_VALUE;
            if (jobl <= mid) {
                ans = Math.max(ans, queryMax(jobl, jobr, l, mid, i << 1));
            }
            if (jobr > mid) {
                ans = Math.max(ans, queryMax(jobl, jobr, mid + 1, r, i << 1 | 1));
            }
            return ans;
        }
    }

    public static void main(String[] args) {
        System.out.println("测试开始");
        int n = 2000;
        int v = 5000;
        int t = 1000000;
        randomArray(n, v);
        long[] check = new long[n + 1];
        for (int i = 1; i <= n; i++) {
            check[i] = arr[i];
        }
        build(1, n, 1);
        for (int i = 1, op, a, b, jobl, jobr, jobv; i <= t; i++) {
            op = (int) (Math.random() * 4);
            a = (int) (Math.random() * n) + 1;
            b = (int) (Math.random() * n) + 1;
            jobl = Math.min(a, b);
            jobr = Math.max(a, b);
            if (op == 0) {
                jobv = (int) (Math.random() * v * 2) - v;
                add(jobl, jobr, jobv, 1, n, 1);
                checkAdd(check, jobl, jobr, jobv);
            } else if (op == 1) {
                jobv = (int) (Math.random() * v * 2) - v;
                setMin(jobl, jobr, jobv, 1, n, 1);
                checkSetMin(check, jobl, jobr, jobv);
            } else if (op == 2) {
                long ans1 = queryMax(jobl, jobr, 1, n, 1);
                long ans2 = checkQueryMax(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            } else {
                long ans1 = querySum(jobl, jobr, 1, n, 1);
                long ans2 = checkQuerySum(check, jobl, jobr);
                if (ans1 != ans2) {
                    System.out.println("出错了!");
                }
            }
        }
        System.out.println("测试结束");
    }

    // 为了验证
    public static void randomArray(int n, int v) {
        for (int i = 1; i <= n; i++) {
            arr[i] = (int) (Math.random() * v * 2) - v;
        }
    }

    // 为了验证
    public static void checkAdd(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] += jobv;
        }
    }

    // 为了验证
    public static void checkSetMin(long[] check, int jobl, int jobr, long jobv) {
        for (int i = jobl; i <= jobr; i++) {
            check[i] = Math.min(check[i], jobv);
        }
    }

    // 为了验证
    public static long checkQueryMax(long[] check, int jobl, int jobr) {
        long ans = Long.MIN_VALUE;
        for (int i = jobl; i <= jobr; i++) {
            ans = Math.max(ans, check[i]);
        }
        return ans;
    }

    // 为了验证
    public static long checkQuerySum(long[] check, int jobl, int jobr) {
        long ans = 0;
        for (int i = jobl; i <= jobr; i++) {
            ans += check[i];
        }
        return ans;
    }

}
```

> - **Question 8: 线段树维护区间最值操作与区间历史最值模板**

```java
import java.io.*;

public class Main {

    public static int MAXN = 500001;

    public static long LOWEST = Long.MIN_VALUE;

    public static int[] arr = new int[MAXN];

    public static long[] sum = new long[MAXN << 2];

    public static long[] max = new long[MAXN << 2];

    public static int[] cnt = new int[MAXN << 2];

    public static long[] sem = new long[MAXN << 2];

    public static long[] maxAdd = new long[MAXN << 2];

    public static long[] otherAdd = new long[MAXN << 2];

    // 历史最大值
    public static long[] maxHistory = new long[MAXN << 2];

    // 最大值达到过的最大提升幅度(懒更新信息)
    public static long[] maxAddTop = new long[MAXN << 2];

    // 除最大值以外的其他数字，达到过的最大提升幅度(懒更新信息)
    public static long[] otherAddTop = new long[MAXN << 2];

    public static void up(int i) {
        int l = i << 1;
        int r = i << 1 | 1;
        maxHistory[i] = Math.max(maxHistory[l], maxHistory[r]);
        sum[i] = sum[l] + sum[r];
        max[i] = Math.max(max[l], max[r]);
        if (max[l] > max[r]) {
            cnt[i] = cnt[l];
            sem[i] = Math.max(sem[l], max[r]);
        } else if (max[l] < max[r]) {
            cnt[i] = cnt[r];
            sem[i] = Math.max(max[l], sem[r]);
        } else {
            cnt[i] = cnt[l] + cnt[r];
            sem[i] = Math.max(sem[l], sem[r]);
        }
    }

    // maxAddv   : 最大值增加多少
    // otherAddv : 其他数增加多少
    // maxUpv    : 最大值达到过的最大提升幅度
    // otherUpv  : 其他数达到过的最大提升幅度
    public static void lazy(int i, int n, long maxAddv, long otherAddv, long maxUpv, long otherUpv) {
        maxHistory[i] = Math.max(maxHistory[i], max[i] + maxUpv);
        maxAddTop[i] = Math.max(maxAddTop[i], maxAdd[i] + maxUpv);
        otherAddTop[i] = Math.max(otherAddTop[i], otherAdd[i] + otherUpv);
        sum[i] += maxAddv * cnt[i] + otherAddv * (n - cnt[i]);
        max[i] += maxAddv;
        sem[i] += sem[i] == LOWEST ? 0 : otherAddv;
        maxAdd[i] += maxAddv;
        otherAdd[i] += otherAddv;
    }

    public static void down(int i, int ln, int rn) {
        int l = i << 1;
        int r = i << 1 | 1;
        long tmp = Math.max(max[l], max[r]);
        if (max[l] == tmp) {
            lazy(l, ln, maxAdd[i], otherAdd[i], maxAddTop[i], otherAddTop[i]);
        } else {
            lazy(l, ln, otherAdd[i], otherAdd[i], otherAddTop[i], otherAddTop[i]);
        }
        if (max[r] == tmp) {
            lazy(r, rn, maxAdd[i], otherAdd[i], maxAddTop[i], otherAddTop[i]);
        } else {
            lazy(r, rn, otherAdd[i], otherAdd[i], otherAddTop[i], otherAddTop[i]);
        }
        maxAdd[i] = otherAdd[i] = maxAddTop[i] = otherAddTop[i] = 0;
    }

    public static void build(int l, int r, int i) {
        if (l == r) {
            sum[i] = max[i] = maxHistory[i] = arr[l];
            sem[i] = LOWEST;
            cnt[i] = 1;
        } else {
            int mid = (l + r) >> 1;
            build(l, mid, i << 1);
            build(mid + 1, r, i << 1 | 1);
            up(i);
        }
        maxAdd[i] = otherAdd[i] = maxAddTop[i] = otherAddTop[i] = 0;
    }

    public static void add(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            lazy(i, r - l + 1, jobv, jobv, jobv, jobv);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                add(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                add(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static void setMin(int jobl, int jobr, long jobv, int l, int r, int i) {
        if (jobv >= max[i]) {
            return;
        }
        if (jobl <= l && r <= jobr && sem[i] < jobv) {
            lazy(i, r - l + 1, jobv - max[i], 0, jobv - max[i], 0);
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            if (jobl <= mid) {
                setMin(jobl, jobr, jobv, l, mid, i << 1);
            }
            if (jobr > mid) {
                setMin(jobl, jobr, jobv, mid + 1, r, i << 1 | 1);
            }
            up(i);
        }
    }

    public static long querySum(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return sum[i];
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            long ans = 0;
            if (jobl <= mid) {
                ans += querySum(jobl, jobr, l, mid, i << 1);
            }
            if (jobr > mid) {
                ans += querySum(jobl, jobr, mid + 1, r, i << 1 | 1);
            }
            return ans;
        }
    }

    public static long queryMax(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return max[i];
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            Long ans = Long.MIN_VALUE;
            if (jobl <= mid) {
                ans = Math.max(ans, queryMax(jobl, jobr, l, mid, i << 1));
            }
            if (jobr > mid) {
                ans = Math.max(ans, queryMax(jobl, jobr, mid + 1, r, i << 1 | 1));
            }
            return ans;
        }
    }

    public static long queryHistoryMax(int jobl, int jobr, int l, int r, int i) {
        if (jobl <= l && r <= jobr) {
            return maxHistory[i];
        } else {
            int mid = (l + r) >> 1;
            down(i, mid - l + 1, r - mid);
            Long ans = Long.MIN_VALUE;
            if (jobl <= mid) {
                ans = Math.max(ans, queryHistoryMax(jobl, jobr, l, mid, i << 1));
            }
            if (jobr > mid) {
                ans = Math.max(ans, queryHistoryMax(jobl, jobr, mid + 1, r, i << 1 | 1));
            }
            return ans;
        }
    }

    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StreamTokenizer in = new StreamTokenizer(br);
        PrintWriter out = new PrintWriter(new OutputStreamWriter(System.out));
        in.nextToken();
        int n = (int) in.nval;
        in.nextToken();
        int m = (int) in.nval;
        for (int i = 1; i <= n; i++) {
            in.nextToken();
            arr[i] = (int) in.nval;
        }
        build(1, n, 1);
        long jobv;
        for (int i = 1, op, jobl, jobr; i <= m; i++) {
            in.nextToken();
            op = (int) in.nval;
            in.nextToken();
            jobl = (int) in.nval;
            in.nextToken();
            jobr = (int) in.nval;
            if (op == 1) {
                in.nextToken();
                jobv = (long) in.nval;
                add(jobl, jobr, jobv, 1, n, 1);
            } else if (op == 2) {
                in.nextToken();
                jobv = (long) in.nval;
                setMin(jobl, jobr, jobv, 1, n, 1);
            } else if (op == 3) {
                out.println(querySum(jobl, jobr, 1, n, 1));
            } else if (op == 4) {
                out.println(queryMax(jobl, jobr, 1, n, 1));
            } else {
                out.println(queryHistoryMax(jobl, jobr, 1, n, 1));
            }
        }
        out.flush();
        out.close();
        br.close();
    }

}
```

# 长度为k的所有子序列中字典序最大的

## 腾讯

> - **Question**
>   - 给定一个字符串 `str` ，和一个正数 `k` ，返回长度为 `k` 的所有子序列中，字典序最大的子序列。

## Java

> - **单调栈**

```java
class Solution {
    
    public static String maxString(String s, int k) {
        if (k <= 0 || s.length() < k) {
            return "";
        }
        char[] str = s.toCharArray();
        // 栈
        char[] stack = new char[str.length];
        // 栈的大小和栈顶下一个位置
        int size = 0;
        for (int i = 0; i < str.length; i++) {
            // 栈自底向上不严格递减，字典序从大到小
            // 相等的可以压入
            // 严格小的全部弹出，遇到大于等于停
            while (size > 0 && stack[size - 1] < str[i] && size + str.length - i > k) {
                size--;
            }
            // size + str.length - i > k 和 size + str.length - i == k是指后面剩下的字符加上栈里面的字符刚好是k个，这时候可以直接返回，不用找了
            // 贪心：这个时候因为前缀是最大的，所以字典序一定是最大的
            if (size + str.length - i == k) {
                return String.valueOf(stack, 0, size) + s.substring(i);
            }
            // 压入
            stack[size++] = str[i];
        }
        // 栈中可能有多个元素，去前k个即可
        return String.valueOf(stack, 0, k);
    }
    
    // 为了测试
    public static String test(String str, int k) {
        if (k <= 0 || str.length() < k) {
            return "";
        }
        TreeSet<String> ans = new TreeSet<>();
        process(0, 0, str.toCharArray(), new char[k], ans);
        return ans.last();
    }
    
    // 为了测试
    public static void process(int si, int pi, char[] str, char[] path, TreeSet<String> ans) {
        if (si == str.length) {
            if (pi == path.length) {
                ans.add(String.valueOf(path));
            }
        } else {
            process(si + 1, pi, str, path, ans);
            if (pi < path.length) {
                path[pi] = str[si];
                process(si + 1, pi + 1, str, path, ans);
            }
        }
    }
    
    // 为了测试
    public static String randomString(int len, int range) {
        char[] str = new char[len];
        for (int i = 0; i < len; i++) {
            str[i] = (char) ((int) (Math.random() * range) + 'a');
        }
        return String.valueOf(str);
    }
    
    public static void main(String[] args) {
        int n = 12;
        int r = 5;
        int testTime = 10000;
        System.out.println("测试开始");
        for (int i = 0; i < testTime; i++) {
            int len = (int) (Math.random() * (n + 1));
            String str = randomString(len, r);
            int k = (int) (Math.random() * (str.length() + 1));
            String ans1 = maxString(str, k);
            String ans2 = test(str, k);
            if (!ans1.equals(ans2)) {
                System.out.println("出错了！");
                System.out.println(str);
                System.out.println(k);
                System.out.println(ans1);
                System.out.println(ans2);
                break;
            }
        }
        System.out.println("测试结束");
    }
}
```

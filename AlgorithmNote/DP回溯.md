## 动态规划与回溯算法笔记

### 动态规划

#### 核心技巧
- 状态定义
- 状态转移方程
- 初始条件
- 结果输出

#### 解题四步骤
1. 定义状态：明确dp[i]或dp[i][j]表示什么
2. 状态转移：找出递推关系
3. 初始条件：确定边界值
4. 结果输出：确定最终答案位置

#### 高频题型
1. 爬楼梯
2. 01背包
3. 完全背包
4. 打家劫舍
5. 最小路径和
6. 最长递增子序列

#### 易错点
- 状态定义不清晰
- 状态转移方程错误
- 初始条件遗漏

### 回溯算法

#### 核心技巧
- 路径记录
- 选择列表
- 剪枝优化
- 回溯撤销

#### 高频题型
1. 子集
2. 组合
3. 全排列
4. 电话号码的字母组合
5. N皇后问题

#### 易错点
- 剪枝条件缺失
- 回溯忘记撤销选择
- 重复元素处理

### 模板代码
```java
// DP模板
public int climbStairs(int n) {
    if (n <= 2) return n;
    int[] dp = new int[n + 1];
    dp[1] = 1;
    dp[2] = 2;
    for (int i = 3; i <= n; i++) {
        dp[i] = dp[i - 1] + dp[i - 2];
    }
    return dp[n];
}

// 回溯模板
public void backtrack(List<Integer> path, int[] nums, int start) {
    result.add(new ArrayList<>(path));
    for (int i = start; i < nums.length; i++) {
        path.add(nums[i]);
        backtrack(path, nums, i + 1);
        path.remove(path.size() - 1);
    }
}
```

### 错题记录
| 题目 | 错误原因 | 修正方法 |
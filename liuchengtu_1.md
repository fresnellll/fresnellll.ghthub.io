# 我的 Mermaid 流程图

```mermaid
flowchart TD
    A[输入整数 m] --> B[初始化字符数组 a[33] 为 '0']
    B --> C[定义 mask = 0x00000001]
    C --> D[循环 i 从 31 到 0]
    D --> E[提取 m 的最低位并存入 a[i]，a[i] = (m & mask) + '0']
    E --> F[右移 m，m >>= 1]
    F --> G[循环继续，直到 i = 0]
    G --> H[循环结束]
    H --> I[循环 j 从 0 到 31]
    I --> J[输出 a[j]]
    J --> K[结束]
## Day 11 日志

### 今日完成

#### 算法刷题
- [ ] 题目1：LC23.合并K个排序链表  
        优先队列（最小堆）： PriorityQueue<ListNode> pq = new PriorityQueue<>((a,b) -> a.val-b.val);
        用于合并K个排序链表，每个链表的头节点加入优先队列，每次从优先队列中取出最小节点，将其加入结果链表，同时将其下一个节点加入优先队列。
- [ ] 题目2：
- [ ] 题目3：

#### 项目开发
- [ ] 任务1：三层架构
        Controller: 处理HTTP请求，调用Service层的方法，返回结果。
            @RestController: 标识为RESTful风格的Controller，将返回的对象包装为JSON格式的结果并返回。
            @GetMapping: 映射GET请求到方法上。
        Service: 处理业务逻辑，调用Mapper层的方法，返回结果。
        Mapper: 与数据库交互，执行SQL语句，返回结果。
- [ ] 任务2：后端Web实战（部门管理）
        @RequestMapping：(根据不同请求方法细分)
        {   
            @GetMapping
            @PostMapping
            @PutMapping
            @DeleteMapping

        }
        @RequestBody:将请求体中的JSON数据转换为Java对象(JSON数据的键名与方法形参对象的属性名相同)
        @Slf4j：用于日志记录，将日志信息记录到日志文件中。log.info("日志信息");
             日志输出级别  trace < debug < info < warn < error   
                        ALL = 全开      OFF = 关闭
#### 底层学习
- [ ] MySQL：
- [ ] Redis：
- [ ] 计网/OS：

### 遇到的问题
1. 
2. 

### 解决方案
1. 
2. 

### 明日计划
1. 
2. 
3.
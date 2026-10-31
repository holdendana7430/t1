代发 wailian999

Java: // 手写回溯递归
来源：http://dk.nicolike.cn

Go:   // 手写回溯递归
来源：http://ep.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://xv.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://aw.szsharing.cn

[N09] 栈与队列
来源：http://re.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dk.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hn.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wz.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lt.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pv.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wy.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qu.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://la.szsharing.cn

[N10] 链表节点定义
来源：http://ol.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eo.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zr.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ra.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wc.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://oi.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ht.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rm.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hm.hahajie.cn

[N11] 二叉树中序遍历
来源：http://qi.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wt.hahajie.cn

PHP:  // 手写递归函数
来源：http://st.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dc.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vk.colortex.cn

Java: // 手写递归
来源：http://sn.shxzskj.cn

Go:   // 手写递归
来源：http://we.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lp.jianghongdianzi.cn

C#:   // 手写递归
来源：http://lb.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lo.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qb.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bz.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iv.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ci.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cx.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fi.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kn.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oq.bookmarksfly.cn

================================================================================
来源：http://vw.jctech888.com.cn

O. 并发与异步
来源：http://iv.lnxyls.cn

================================================================================
来源：http://fc.asd995.cn

[O01] 启动一个线程
来源：http://ih.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xm.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://li.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mb.jianghongdianzi.cn

TS:   // 同 JS
来源：http://fl.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://hc.shxzukj.cn

Go:   go f()
来源：http://du.lnxyls.cn

Ruby: Thread.new { f }
来源：http://lm.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://cf.asd995.cn

[O02] 使用线程池
来源：http://xl.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tp.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://os.521024.cn

JS:   // worker_threads 线程池
来源：http://xh.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://yh.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zz.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oj.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mz.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sl.newstarts.cn

[O03] 加锁保护共享数据
来源：http://wp.newstarts.cn

Py:   with lock: shared += 1
来源：http://jn.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://aj.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mb.colortex.cn

TS:   // 同 JS
来源：http://pf.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://of.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hx.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wp.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://yr.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://yl.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://ks.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ue.huanxung.cn

JS:   async function f() { await g(); }
来源：http://ok.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gv.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://un.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nq.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://be.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://hc.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://wd.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://qf.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vn.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://no.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://nz.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wu.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oc.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://wp.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://am.gzmigu.cn

[O06] 使用进程池
来源：http://ao.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lz.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ei.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://je.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://ok.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oc.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bf.nszjky.cn

Ruby: // fork 块
来源：http://pw.bookmarksfly.cn

C#:   Parallel.For
来源：http://at.szxytkj.cn

================================================================================
来源：http://ig.bjjhwx.cn

P. 常用工具函数
来源：http://it.haigaiapp.cn

================================================================================
来源：http://ws.wgjwhj.cn

[P01] 生成 UUID
来源：http://ch.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://he.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oj.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://nd.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://et.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://ai.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://fa.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ru.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://ok.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://gi.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rg.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wb.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bc.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xn.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uf.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ns.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ke.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hl.panjiajie.cn

[P03] 生成短随机字符串
来源：http://co.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rj.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kx.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dw.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kn.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iw.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qg.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nx.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wj.jctech888.com.cn

[P04] 求长度
来源：http://fy.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ut.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fw.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mw.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qa.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://yf.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://lj.hahajie.cn

Ruby: x.length;  x.size
来源：http://dd.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://te.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://fy.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://al.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ml.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cn.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ok.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oy.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zh.huixiangedu.cn

Ruby: a == b
来源：http://gc.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tc.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nl.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fw.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://av.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bo.newstarts.cn

TS:   if (x == null) {}
来源：http://pd.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zx.wgjwhj.cn

Go:   if x == nil {}
来源：http://ue.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rz.haigaiapp.cn

C#:   if (x is null) {}
来源：http://in.shxzskj.cn

[P07] 防抖与节流
来源：http://lg.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yy.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://sf.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rh.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cu.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cb.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yw.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hs.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gi.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://qb.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fr.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qd.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://za.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qd.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://av.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ti.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jo.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vt.bjjhwx.cn

================================================================================
来源：http://qd.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kw.panjiajie.cn

================================================================================
来源：http://bz.muxihuayi.cn

[Q01] 创建表
来源：http://nb.yuexingan06.cn

CREATE TABLE users (
来源：http://ik.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cq.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://gh.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://vv.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bl.lnxyls.cn

);
来源：http://lk.nszjky.cn

[Q02] 创建带外键的表
来源：http://xl.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://zg.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hk.shtwfgs.cn

user_id INT NOT NULL,
来源：http://mn.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://bd.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rd.bookmarksfly.cn

);
来源：http://dy.huixiangedu.cn

[Q03] 增加列
来源：http://dj.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xy.asd995.cn

[Q04] 修改列类型
来源：http://mq.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ws.szsharing.cn

[Q05] 重命名列
来源：http://sg.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://br.521024.cn

[Q06] 删除列
来源：http://gh.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lo.shxzskj.cn

[Q07] 删除表
来源：http://og.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://wg.gzmigu.cn

[Q08] 创建普通索引
来源：http://vk.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fw.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://il.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yr.haigaiapp.cn

[Q10] 插入单行
来源：http://tv.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ci.asd995.cn

[Q11] 一次插入多行
来源：http://rm.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lw.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://ej.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://po.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ea.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://rx.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hq.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://tb.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mu.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oa.haigaiapp.cn

[Q15] 查询全部
来源：http://na.yuexingan06.cn

SELECT * FROM users;
来源：http://ie.panjiajie.cn

[Q16] 查询指定列
来源：http://st.9csxet.cn

SELECT id, name FROM users;
来源：http://vl.jianghongdianzi.cn

[Q17] 条件查询
来源：http://aj.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sn.nicolike.cn

[Q18] 模糊匹配
来源：http://gf.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jo.panjiajie.cn

[Q19] 范围查询
来源：http://sp.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vq.szsharing.cn

[Q20] IN 列表
来源：http://dd.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ih.huixiangedu.cn

[Q21] 空值判断
来源：http://sg.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ux.panjiajie.cn

[Q22] 排序
来源：http://cu.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yw.bjjhwx.cn

[Q23] 分页
来源：http://ea.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ks.lnxyls.cn

[Q24] 去重
来源：http://no.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://ir.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://bf.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vx.colortex.cn

[Q26] 计数
来源：http://yo.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://hd.9csxet.cn

[Q27] 条件计数
来源：http://uf.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://at.hnjuh.cn

[Q28] 求和与平均
来源：http://wa.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nd.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://uo.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://og.hahajie.cn

[Q30] 分组统计
来源：http://he.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eo.lnxyls.cn

[Q31] 分组后过滤
来源：http://rm.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pv.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://sg.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sg.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mz.colortex.cn

[Q33] 多列分组
来源：http://uy.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sk.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://qr.szxytkj.cn

SELECT * FROM (
来源：http://hr.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wt.szxytkj.cn

) t WHERE rn = 1;
来源：http://kb.asd995.cn

[Q35] 内连接
来源：http://yg.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ap.shxzukj.cn

[Q36] 左连接
来源：http://so.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://un.jianghongdianzi.cn

[Q37] 右连接
来源：http://vm.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ay.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://np.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dp.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://kw.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mb.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eq.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rw.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lm.chemitech.net.cn

[Q41] 多表连接
来源：http://if.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cp.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://xi.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://ti.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://di.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://mr.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nl.huixiangedu.cn

[Q43] 标量子查询
来源：http://go.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://so.nicolike.cn

[Q44] IN 子查询
来源：http://gf.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pg.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://xm.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fz.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ih.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ym.panjiajie.cn

[Q47] 与平均值比较
来源：http://kq.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zx.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://vu.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oj.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://su.shtwfgs.cn

[Q49] 更新单行
来源：http://in.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ay.yuntaijiaju.cn

[Q50] 批量更新
来源：http://oq.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://id.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://dk.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cf.muxihuayi.cn

[Q52] 删除指定行
来源：http://jq.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://wz.shxzskj.cn

[Q53] 按条件删除
来源：http://nh.panjiajie.cn


<!-- 参考信息 -->
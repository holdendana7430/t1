代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mq.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mi.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kk.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ac.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://se.shtwfgs.cn

[N10] 链表节点定义
来源：http://zv.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eh.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yt.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zl.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vn.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://an.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pe.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mq.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://in.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://vx.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rd.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://pu.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kh.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qk.hahajie.cn

Java: // 手写递归
来源：http://ex.jctech888.com.cn

Go:   // 手写递归
来源：http://rg.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uo.521024.cn

C#:   // 手写递归
来源：http://xc.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://to.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cu.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jr.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rz.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qw.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oc.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gf.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://si.wgjwhj.cn

================================================================================
来源：http://jd.haigaiapp.cn

O. 并发与异步
来源：http://dk.huixinmuqiang.cn

================================================================================
来源：http://cf.panjiajie.cn

[O01] 启动一个线程
来源：http://gv.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wq.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zb.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rv.huanxung.cn

TS:   // 同 JS
来源：http://dr.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://oq.shxzskj.cn

Go:   go f()
来源：http://zr.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://hs.colortex.cn

C#:   Task.Run(() => F());
来源：http://ll.chemitech.net.cn

[O02] 使用线程池
来源：http://kz.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zw.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sk.szsharing.cn

JS:   // worker_threads 线程池
来源：http://yl.nszjky.cn

TS:   // worker_threads 线程池
来源：http://rn.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cz.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fn.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://io.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xu.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://ki.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://hx.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://uf.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ij.szxytkj.cn

TS:   // 同 JS
来源：http://ag.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://ct.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ji.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wf.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://za.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://hp.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://tb.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://to.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://rq.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rf.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pq.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ia.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bh.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://cp.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://td.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://yt.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fg.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://xq.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://ph.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://by.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yj.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ol.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yx.asd995.cn

[O06] 使用进程池
来源：http://do.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vs.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fy.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://sa.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://xo.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vo.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pc.yuexingan06.cn

Ruby: // fork 块
来源：http://xw.hnjuh.cn

C#:   Parallel.For
来源：http://oi.hahajie.cn

================================================================================
来源：http://au.huixinmuqiang.cn

P. 常用工具函数
来源：http://pr.shxzskj.cn

================================================================================
来源：http://fw.521024.cn

[P01] 生成 UUID
来源：http://yo.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://fl.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yy.newstarts.cn

JS:   crypto.randomUUID()
来源：http://il.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://pn.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://ek.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://sa.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://ni.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ln.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://vj.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uc.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jj.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zi.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://na.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fi.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pj.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zd.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://en.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://hi.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hs.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iz.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ba.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mf.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ay.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rq.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xu.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://km.shxzukj.cn

[P04] 求长度
来源：http://tm.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ts.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wm.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uc.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gu.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://sj.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://ew.521024.cn

Ruby: x.length;  x.size
来源：http://wu.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pi.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://pu.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oa.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bj.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ok.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xl.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vk.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ku.yuexingan06.cn

Ruby: a == b
来源：http://cp.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tm.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ra.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ua.asd995.cn

PHP:  if (empty($x)) {}
来源：http://pa.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fl.shtwfgs.cn

TS:   if (x == null) {}
来源：http://ly.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iy.bookmarksfly.cn

Go:   if x == nil {}
来源：http://bj.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vg.shxzukj.cn

C#:   if (x is null) {}
来源：http://iv.shxzukj.cn

[P07] 防抖与节流
来源：http://wr.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tm.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://na.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mc.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://em.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ji.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yk.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://st.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://pg.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wy.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bk.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ms.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xg.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://za.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rd.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ro.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yt.9csxet.cn

================================================================================
来源：http://bi.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://me.newstarts.cn

================================================================================
来源：http://rm.shxzukj.cn

[Q01] 创建表
来源：http://ew.jianghongdianzi.cn

CREATE TABLE users (
来源：http://ar.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ms.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://fr.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://ix.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jp.bjjhwx.cn

);
来源：http://uj.colortex.cn

[Q02] 创建带外键的表
来源：http://zt.haigaiapp.cn

CREATE TABLE orders (
来源：http://bz.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yb.hahajie.cn

user_id INT NOT NULL,
来源：http://ay.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://na.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mp.nszjky.cn

);
来源：http://ic.szsharing.cn

[Q03] 增加列
来源：http://pv.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://di.bookmarksfly.cn

[Q04] 修改列类型
来源：http://mp.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ok.colortex.cn

[Q05] 重命名列
来源：http://dw.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mk.szsharing.cn

[Q06] 删除列
来源：http://sl.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://se.nszjky.cn

[Q07] 删除表
来源：http://fv.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://ai.huanxung.cn

[Q08] 创建普通索引
来源：http://ht.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://la.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://zl.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vr.shtwfgs.cn

[Q10] 插入单行
来源：http://he.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xv.chemitech.net.cn

[Q11] 一次插入多行
来源：http://ft.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bq.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://ch.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jl.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oy.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://vp.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sw.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://wb.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ed.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vr.haigaiapp.cn

[Q15] 查询全部
来源：http://hj.nicolike.cn

SELECT * FROM users;
来源：http://zs.szxytkj.cn

[Q16] 查询指定列
来源：http://kx.bjjhwx.cn

SELECT id, name FROM users;
来源：http://oh.shxzskj.cn

[Q17] 条件查询
来源：http://iu.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bq.jctech888.com.cn

[Q18] 模糊匹配
来源：http://bv.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ut.bjjhwx.cn

[Q19] 范围查询
来源：http://hc.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xu.huixiangedu.cn

[Q20] IN 列表
来源：http://hx.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eo.gzmigu.cn

[Q21] 空值判断
来源：http://fd.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rm.huanxung.cn

[Q22] 排序
来源：http://io.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://er.lnxyls.cn

[Q23] 分页
来源：http://hc.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zh.asd995.cn

[Q24] 去重
来源：http://fk.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://mw.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://ss.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rb.szsharing.cn

[Q26] 计数
来源：http://iq.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ah.521024.cn

[Q27] 条件计数
来源：http://ne.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hk.gzmigu.cn

[Q28] 求和与平均
来源：http://mi.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xh.shtwfgs.cn

[Q29] 最大最小值
来源：http://cz.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oe.bookmarksfly.cn

[Q30] 分组统计
来源：http://yf.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zo.panjiajie.cn

[Q31] 分组后过滤
来源：http://rf.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xc.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://vb.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://he.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bn.hahajie.cn

[Q33] 多列分组
来源：http://xk.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oc.chemitech.net.cn

[Q34] 每组取第一条
来源：http://dk.9csxet.cn

SELECT * FROM (
来源：http://ep.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nj.szxytkj.cn

) t WHERE rn = 1;
来源：http://wn.shtwfgs.cn

[Q35] 内连接
来源：http://iw.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ip.chemitech.net.cn

[Q36] 左连接
来源：http://ig.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pr.hahajie.cn

[Q37] 右连接
来源：http://tk.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hs.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hi.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fv.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://hn.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zq.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cl.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://on.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wo.9csxet.cn

[Q41] 多表连接
来源：http://bm.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uw.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://ib.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://eq.asd995.cn

[Q42] 连接条件附加过滤
来源：http://ai.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://gz.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bk.lnxyls.cn

[Q43] 标量子查询
来源：http://zj.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://np.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://ab.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ip.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://kw.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xw.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://da.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ef.shxzukj.cn

[Q47] 与平均值比较
来源：http://wr.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rl.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://sn.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vx.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://iu.panjiajie.cn

[Q49] 更新单行
来源：http://tp.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ok.asd995.cn

[Q50] 批量更新
来源：http://xu.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xs.wgjwhj.cn

[Q51] 用子查询更新
来源：http://xf.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://na.hnjuh.cn

[Q52] 删除指定行
来源：http://fx.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://wd.szsharing.cn

[Q53] 按条件删除
来源：http://pq.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sz.shxzskj.cn

[Q54] 清空表
来源：http://vd.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://tn.521024.cn

[Q55] 排名（并列占位）
来源：http://dp.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yq.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://ci.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tc.hahajie.cn

[Q57] 行号
来源：http://kl.hnjuh.cn


<!-- 参考信息 -->
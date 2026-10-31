代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ao.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://ih.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zw.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oi.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ez.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qz.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://pc.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rd.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mq.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eu.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://qm.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zn.szxytkj.cn

PHP:  // 手写递归函数
来源：http://mr.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ce.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hl.huanxung.cn

Java: // 手写递归
来源：http://ai.gzmigu.cn

Go:   // 手写递归
来源：http://ds.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bq.nicolike.cn

C#:   // 手写递归
来源：http://px.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xh.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yk.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://te.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hc.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ok.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ov.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://am.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wl.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rj.muxihuayi.cn

================================================================================
来源：http://xe.nszjky.cn

O. 并发与异步
来源：http://se.521024.cn

================================================================================
来源：http://yg.huanxung.cn

[O01] 启动一个线程
来源：http://du.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://my.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ab.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yd.shxzukj.cn

TS:   // 同 JS
来源：http://yf.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://sy.hahajie.cn

Go:   go f()
来源：http://cu.9csxet.cn

Ruby: Thread.new { f }
来源：http://ld.9csxet.cn

C#:   Task.Run(() => F());
来源：http://pu.shxzukj.cn

[O02] 使用线程池
来源：http://xa.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://we.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pi.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://gj.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://wf.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fz.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wi.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gc.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xe.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://ps.szxytkj.cn

Py:   with lock: shared += 1
来源：http://yv.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://ev.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ig.panjiajie.cn

TS:   // 同 JS
来源：http://fv.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://mv.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vh.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zx.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://kr.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://yv.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ls.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oi.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://au.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cq.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eh.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pz.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fe.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://qs.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://bg.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://ol.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zn.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ut.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://ya.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yq.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lh.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://cx.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zh.shxzukj.cn

[O06] 使用进程池
来源：http://rl.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://of.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ut.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://vo.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://uh.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jz.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kj.wgjwhj.cn

Ruby: // fork 块
来源：http://uo.hahajie.cn

C#:   Parallel.For
来源：http://yy.bookmarksfly.cn

================================================================================
来源：http://ad.szxytkj.cn

P. 常用工具函数
来源：http://gu.muxihuayi.cn

================================================================================
来源：http://fb.bookmarksfly.cn

[P01] 生成 UUID
来源：http://qk.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://da.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cs.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://bb.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://af.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://pt.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://qm.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://qo.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://nt.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://xd.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fo.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kt.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ee.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ne.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qr.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kl.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ej.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gd.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://zk.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fj.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xw.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ts.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uk.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gh.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kb.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tk.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mb.yuntaijiaju.cn

[P04] 求长度
来源：http://lj.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yk.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ih.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tk.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xs.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://lw.newstarts.cn

Go:   len(arr);  len(m)
来源：http://vj.szsharing.cn

Ruby: x.length;  x.size
来源：http://ra.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://py.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://qz.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cf.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rz.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fa.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mz.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uk.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yc.gzmigu.cn

Ruby: a == b
来源：http://ba.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rv.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tf.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wk.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://dn.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mb.shxzskj.cn

TS:   if (x == null) {}
来源：http://mk.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gn.bookmarksfly.cn

Go:   if x == nil {}
来源：http://io.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aq.yuexingan06.cn

C#:   if (x is null) {}
来源：http://fv.asd995.cn

[P07] 防抖与节流
来源：http://ii.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jq.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://ea.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vr.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ul.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qh.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ty.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vy.521024.cn

[P08] 处理浮点精度问题
来源：http://vn.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fr.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ur.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dg.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jk.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hd.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lc.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iz.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lw.asd995.cn

================================================================================
来源：http://ga.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ww.nicolike.cn

================================================================================
来源：http://qp.9csxet.cn

[Q01] 创建表
来源：http://gy.huanxung.cn

CREATE TABLE users (
来源：http://hq.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iy.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://nv.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://hq.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nt.bjjhwx.cn

);
来源：http://za.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://ym.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://nx.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sj.szsharing.cn

user_id INT NOT NULL,
来源：http://rb.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://jr.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tw.hnjuh.cn

);
来源：http://ov.hahajie.cn

[Q03] 增加列
来源：http://qn.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eu.colortex.cn

[Q04] 修改列类型
来源：http://wr.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vm.huixiangedu.cn

[Q05] 重命名列
来源：http://cs.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lh.shxzukj.cn

[Q06] 删除列
来源：http://ga.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xn.muxihuayi.cn

[Q07] 删除表
来源：http://gq.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://aq.asd995.cn

[Q08] 创建普通索引
来源：http://kv.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tw.hnjuh.cn

[Q09] 创建唯一索引
来源：http://gp.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xs.szxytkj.cn

[Q10] 插入单行
来源：http://qq.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://at.nicolike.cn

[Q11] 一次插入多行
来源：http://qw.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mv.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://ps.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hh.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tf.gzmigu.cn

[Q13] 忽略重复插入
来源：http://um.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qo.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://gs.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uh.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://we.haigaiapp.cn

[Q15] 查询全部
来源：http://tk.shxzskj.cn

SELECT * FROM users;
来源：http://mx.lnxyls.cn

[Q16] 查询指定列
来源：http://af.szsharing.cn

SELECT id, name FROM users;
来源：http://yc.wgjwhj.cn

[Q17] 条件查询
来源：http://mm.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cq.gzmigu.cn

[Q18] 模糊匹配
来源：http://sr.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vv.huanxung.cn

[Q19] 范围查询
来源：http://cn.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gh.jctech888.com.cn

[Q20] IN 列表
来源：http://is.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dj.jianghongdianzi.cn

[Q21] 空值判断
来源：http://es.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ub.lnxyls.cn

[Q22] 排序
来源：http://po.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://it.bookmarksfly.cn

[Q23] 分页
来源：http://ej.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qo.gzmigu.cn

[Q24] 去重
来源：http://dm.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://rc.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://gl.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://id.hahajie.cn

[Q26] 计数
来源：http://qu.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://nd.asd995.cn

[Q27] 条件计数
来源：http://va.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cn.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://kc.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wr.shtwfgs.cn

[Q29] 最大最小值
来源：http://fa.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sp.shxzukj.cn

[Q30] 分组统计
来源：http://hg.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fm.521024.cn

[Q31] 分组后过滤
来源：http://xb.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oy.hahajie.cn

[Q32] 分组拼接字符串
来源：http://rs.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dx.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wz.huanxung.cn

[Q33] 多列分组
来源：http://ny.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oe.nszjky.cn

[Q34] 每组取第一条
来源：http://sw.hnjuh.cn

SELECT * FROM (
来源：http://qv.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ln.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://eh.haigaiapp.cn

[Q35] 内连接
来源：http://ht.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qc.hahajie.cn

[Q36] 左连接
来源：http://gc.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iy.haigaiapp.cn

[Q37] 右连接
来源：http://cb.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ku.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kq.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aq.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://fi.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://so.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ye.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://em.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ci.shtwfgs.cn

[Q41] 多表连接
来源：http://ho.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://py.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://hg.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://kc.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://mi.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://cg.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mu.bookmarksfly.cn

[Q43] 标量子查询
来源：http://ww.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lb.521024.cn

[Q44] IN 子查询
来源：http://af.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kf.521024.cn

[Q45] EXISTS 判断存在
来源：http://jv.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rw.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ms.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jy.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://vo.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qp.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://by.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://la.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://wg.bookmarksfly.cn

[Q49] 更新单行
来源：http://oh.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ug.jianghongdianzi.cn

[Q50] 批量更新
来源：http://eh.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lt.521024.cn

[Q51] 用子查询更新
来源：http://nf.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ik.huixiangedu.cn

[Q52] 删除指定行
来源：http://cd.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://px.asd995.cn

[Q53] 按条件删除
来源：http://pk.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gu.yuexingan06.cn

[Q54] 清空表
来源：http://qt.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://nb.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://hv.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rq.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://sk.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gv.huixiangedu.cn

[Q57] 行号
来源：http://eu.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://be.newstarts.cn

[Q58] 累计求和
来源：http://po.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hf.bookmarksfly.cn

[Q59] 分组内累计
来源：http://qd.shxzskj.cn


<!-- 参考信息 -->
代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bo.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ni.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jf.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xh.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://do.nicolike.cn

[N10] 链表节点定义
来源：http://lk.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ck.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tj.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://te.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://so.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://oc.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ov.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uh.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ki.szsharing.cn

[N11] 二叉树中序遍历
来源：http://dm.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vr.shxzskj.cn

PHP:  // 手写递归函数
来源：http://jz.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zu.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zo.521024.cn

Java: // 手写递归
来源：http://sc.huixiangedu.cn

Go:   // 手写递归
来源：http://az.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zb.shxzskj.cn

C#:   // 手写递归
来源：http://yf.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jp.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://am.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zb.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nw.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xk.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tz.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://op.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tm.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mm.lnxyls.cn

================================================================================
来源：http://ze.jianghongdianzi.cn

O. 并发与异步
来源：http://oo.panjiajie.cn

================================================================================
来源：http://tt.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://kd.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ja.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://us.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qh.panjiajie.cn

TS:   // 同 JS
来源：http://mp.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://ok.jianghongdianzi.cn

Go:   go f()
来源：http://wk.newstarts.cn

Ruby: Thread.new { f }
来源：http://np.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://lo.bjjhwx.cn

[O02] 使用线程池
来源：http://yi.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yn.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mo.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://dr.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://qd.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ab.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ed.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pl.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ip.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://fa.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://fj.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://ix.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ij.szxytkj.cn

TS:   // 同 JS
来源：http://bm.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://tg.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xa.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ay.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://fy.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://pr.521024.cn

Py:   async def f():⏎    await g()
来源：http://jd.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ro.newstarts.cn

JS:   async function f() { await g(); }
来源：http://oq.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qh.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wc.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ok.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qo.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://hl.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://cw.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://ck.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sb.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://ha.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://ca.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ir.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eo.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://dm.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sm.asd995.cn

[O06] 使用进程池
来源：http://la.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tt.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xp.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://tw.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://oo.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uf.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fk.huanxung.cn

Ruby: // fork 块
来源：http://xp.newstarts.cn

C#:   Parallel.For
来源：http://yu.colortex.cn

================================================================================
来源：http://fp.huanxung.cn

P. 常用工具函数
来源：http://ed.hahajie.cn

================================================================================
来源：http://bb.szxytkj.cn

[P01] 生成 UUID
来源：http://my.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://yx.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ye.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://cl.521024.cn

TS:   crypto.randomUUID()
来源：http://vj.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://hx.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://jr.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://tk.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://ar.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://ip.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xr.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://he.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uo.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://se.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tt.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lu.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ph.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gw.hahajie.cn

[P03] 生成短随机字符串
来源：http://dh.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://al.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fr.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xh.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rz.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xy.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ug.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qd.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qp.muxihuayi.cn

[P04] 求长度
来源：http://wd.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rk.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jf.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cs.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tf.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://xs.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://ip.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ht.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rg.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://za.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hc.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://se.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ud.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cc.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eb.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ka.bjjhwx.cn

Ruby: a == b
来源：http://vq.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rj.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sq.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jv.521024.cn

PHP:  if (empty($x)) {}
来源：http://qf.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pw.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://on.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zf.wgjwhj.cn

Go:   if x == nil {}
来源：http://da.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bj.asd995.cn

C#:   if (x is null) {}
来源：http://rv.huixiangedu.cn

[P07] 防抖与节流
来源：http://cu.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qh.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://jr.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://co.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cr.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cw.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hw.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vz.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://ag.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lk.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uk.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fi.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jd.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pu.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bi.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tl.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tf.wgjwhj.cn

================================================================================
来源：http://hj.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gp.szxytkj.cn

================================================================================
来源：http://un.yuexingan06.cn

[Q01] 创建表
来源：http://vy.jctech888.com.cn

CREATE TABLE users (
来源：http://uc.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vs.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://jj.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://ea.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dg.muxihuayi.cn

);
来源：http://qg.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://kg.shtwfgs.cn

CREATE TABLE orders (
来源：http://tr.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mq.gzmigu.cn

user_id INT NOT NULL,
来源：http://xc.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://hx.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lo.huixinmuqiang.cn

);
来源：http://bb.wgjwhj.cn

[Q03] 增加列
来源：http://bc.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yy.muxihuayi.cn

[Q04] 修改列类型
来源：http://xb.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yn.gzmigu.cn

[Q05] 重命名列
来源：http://ir.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://la.521024.cn

[Q06] 删除列
来源：http://rq.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tv.szsharing.cn

[Q07] 删除表
来源：http://ts.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://fv.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ss.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zc.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://te.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://td.jctech888.com.cn

[Q10] 插入单行
来源：http://zo.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qr.9csxet.cn

[Q11] 一次插入多行
来源：http://vi.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xc.521024.cn

[Q12] 插入后取自增 ID
来源：http://tq.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rq.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jk.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://qu.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oj.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://ud.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lo.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jb.shxzskj.cn

[Q15] 查询全部
来源：http://tm.521024.cn

SELECT * FROM users;
来源：http://ig.shxzskj.cn

[Q16] 查询指定列
来源：http://sy.muxihuayi.cn

SELECT id, name FROM users;
来源：http://cx.yuntaijiaju.cn

[Q17] 条件查询
来源：http://xp.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ss.chemitech.net.cn

[Q18] 模糊匹配
来源：http://cs.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jz.hnjuh.cn

[Q19] 范围查询
来源：http://gv.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nw.colortex.cn

[Q20] IN 列表
来源：http://nd.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tb.hahajie.cn

[Q21] 空值判断
来源：http://vr.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ck.haigaiapp.cn

[Q22] 排序
来源：http://jr.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bl.haigaiapp.cn

[Q23] 分页
来源：http://ee.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rt.jianghongdianzi.cn

[Q24] 去重
来源：http://dz.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://dm.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://lf.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://or.huixinmuqiang.cn

[Q26] 计数
来源：http://uh.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://zo.nszjky.cn

[Q27] 条件计数
来源：http://ag.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bi.9csxet.cn

[Q28] 求和与平均
来源：http://gj.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qs.gzmigu.cn

[Q29] 最大最小值
来源：http://ue.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://do.nszjky.cn

[Q30] 分组统计
来源：http://fx.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://st.9csxet.cn

[Q31] 分组后过滤
来源：http://sd.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://td.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://ac.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tx.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hn.yuntaijiaju.cn

[Q33] 多列分组
来源：http://az.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://do.asd995.cn

[Q34] 每组取第一条
来源：http://zu.huanxung.cn

SELECT * FROM (
来源：http://fy.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nq.huixiangedu.cn

) t WHERE rn = 1;
来源：http://xn.muxihuayi.cn

[Q35] 内连接
来源：http://si.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gk.huixiangedu.cn

[Q36] 左连接
来源：http://ga.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nj.bjjhwx.cn

[Q37] 右连接
来源：http://ve.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xd.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eh.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yi.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://em.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oy.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gt.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gi.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wp.9csxet.cn

[Q41] 多表连接
来源：http://xz.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gf.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://ho.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://yg.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://go.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://gi.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hl.nicolike.cn

[Q43] 标量子查询
来源：http://bb.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ko.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://wx.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kj.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://wo.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ym.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yu.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ah.nicolike.cn

[Q47] 与平均值比较
来源：http://dn.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ck.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://zq.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xd.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://yz.wgjwhj.cn

[Q49] 更新单行
来源：http://gr.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kd.jianghongdianzi.cn

[Q50] 批量更新
来源：http://no.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dt.jctech888.com.cn

[Q51] 用子查询更新
来源：http://ye.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qb.bookmarksfly.cn

[Q52] 删除指定行
来源：http://ck.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://ps.shxzukj.cn

[Q53] 按条件删除
来源：http://qf.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ln.shxzukj.cn

[Q54] 清空表
来源：http://ge.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://ww.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ei.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ou.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://ax.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uj.jianghongdianzi.cn

[Q57] 行号
来源：http://fb.jianghongdianzi.cn


<!-- 参考信息 -->
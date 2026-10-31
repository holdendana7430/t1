代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fx.9csxet.cn

[N10] 链表节点定义
来源：http://eq.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mu.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eq.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mc.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nw.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://mu.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gu.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pj.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zh.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://mr.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yl.521024.cn

PHP:  // 手写递归函数
来源：http://ko.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://in.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yq.huixiangedu.cn

Java: // 手写递归
来源：http://rg.muxihuayi.cn

Go:   // 手写递归
来源：http://fj.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ph.shxzukj.cn

C#:   // 手写递归
来源：http://zx.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gz.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pn.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dv.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vp.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wj.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xj.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zj.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zh.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zl.haigaiapp.cn

================================================================================
来源：http://xy.panjiajie.cn

O. 并发与异步
来源：http://kw.muxihuayi.cn

================================================================================
来源：http://sj.9csxet.cn

[O01] 启动一个线程
来源：http://fm.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ud.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cr.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wl.huanxung.cn

TS:   // 同 JS
来源：http://yo.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://qd.nicolike.cn

Go:   go f()
来源：http://ju.lnxyls.cn

Ruby: Thread.new { f }
来源：http://ms.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://ym.szxytkj.cn

[O02] 使用线程池
来源：http://si.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ir.9csxet.cn

JS:   // worker_threads 线程池
来源：http://qg.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://lk.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ni.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hv.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://so.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ms.nszjky.cn

[O03] 加锁保护共享数据
来源：http://cq.gzmigu.cn

Py:   with lock: shared += 1
来源：http://dr.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://sk.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ip.szsharing.cn

TS:   // 同 JS
来源：http://aq.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://se.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lm.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qm.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://uo.huanxung.cn

[O04] 定义异步函数并等待
来源：http://ks.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://so.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bc.asd995.cn

JS:   async function f() { await g(); }
来源：http://kp.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yy.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qa.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yq.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lt.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://cz.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://np.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://ww.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eu.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://iy.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://hx.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ni.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uc.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://fn.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fl.bjjhwx.cn

[O06] 使用进程池
来源：http://wp.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zt.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wl.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://wd.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://jf.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sx.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bv.lnxyls.cn

Ruby: // fork 块
来源：http://ug.nszjky.cn

C#:   Parallel.For
来源：http://wd.huixinmuqiang.cn

================================================================================
来源：http://aa.hahajie.cn

P. 常用工具函数
来源：http://da.newstarts.cn

================================================================================
来源：http://dj.colortex.cn

[P01] 生成 UUID
来源：http://mu.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://qr.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ua.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://le.colortex.cn

TS:   crypto.randomUUID()
来源：http://yq.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://ko.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://kn.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://hp.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://xx.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://wm.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cq.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oc.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vp.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jh.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sa.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gp.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://op.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ex.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://ls.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zu.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gx.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fk.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vv.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ld.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gi.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tn.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qq.shtwfgs.cn

[P04] 求长度
来源：http://ow.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rb.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ci.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://im.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://st.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://ey.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://lw.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://hv.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ro.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://nh.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://or.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mh.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oz.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oo.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://io.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cj.chemitech.net.cn

Ruby: a == b
来源：http://re.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://am.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lj.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cq.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://uw.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hi.wgjwhj.cn

TS:   if (x == null) {}
来源：http://pc.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nf.nszjky.cn

Go:   if x == nil {}
来源：http://tc.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vz.bjjhwx.cn

C#:   if (x is null) {}
来源：http://ua.haigaiapp.cn

[P07] 防抖与节流
来源：http://sv.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vs.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://zk.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zn.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nk.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xk.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ca.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nh.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xf.521024.cn

[P08] 处理浮点精度问题
来源：http://nv.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ak.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ns.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ou.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iu.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dq.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://we.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lu.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xj.yuexingan06.cn

================================================================================
来源：http://ls.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xp.huixinmuqiang.cn

================================================================================
来源：http://uc.jianghongdianzi.cn

[Q01] 创建表
来源：http://fk.nicolike.cn

CREATE TABLE users (
来源：http://kt.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pa.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://cg.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://cd.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rq.nicolike.cn

);
来源：http://ce.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://ae.asd995.cn

CREATE TABLE orders (
来源：http://om.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://og.newstarts.cn

user_id INT NOT NULL,
来源：http://ok.nicolike.cn

amount DECIMAL(10, 2),
来源：http://ia.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bf.jctech888.com.cn

);
来源：http://ug.521024.cn

[Q03] 增加列
来源：http://zk.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ag.shxzskj.cn

[Q04] 修改列类型
来源：http://eb.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vk.9csxet.cn

[Q05] 重命名列
来源：http://ia.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qg.chemitech.net.cn

[Q06] 删除列
来源：http://ww.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ez.hahajie.cn

[Q07] 删除表
来源：http://uh.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://us.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://sv.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zz.gzmigu.cn

[Q09] 创建唯一索引
来源：http://jv.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ii.huanxung.cn

[Q10] 插入单行
来源：http://lj.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ky.shxzskj.cn

[Q11] 一次插入多行
来源：http://cq.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gb.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://hw.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://to.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zs.nszjky.cn

[Q13] 忽略重复插入
来源：http://ew.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gf.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://gd.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gy.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hv.gzmigu.cn

[Q15] 查询全部
来源：http://eo.bookmarksfly.cn

SELECT * FROM users;
来源：http://wi.huanxung.cn

[Q16] 查询指定列
来源：http://sl.nszjky.cn

SELECT id, name FROM users;
来源：http://yb.huanxung.cn

[Q17] 条件查询
来源：http://vj.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wc.gzmigu.cn

[Q18] 模糊匹配
来源：http://ci.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xk.huixinmuqiang.cn

[Q19] 范围查询
来源：http://ci.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ty.yuntaijiaju.cn

[Q20] IN 列表
来源：http://na.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gu.colortex.cn

[Q21] 空值判断
来源：http://pm.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xn.nicolike.cn

[Q22] 排序
来源：http://hz.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://br.wgjwhj.cn

[Q23] 分页
来源：http://li.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hp.gzmigu.cn

[Q24] 去重
来源：http://rb.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://dl.hnjuh.cn

[Q25] 只取前 N 条
来源：http://kc.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://md.nszjky.cn

[Q26] 计数
来源：http://ci.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://ro.huanxung.cn

[Q27] 条件计数
来源：http://tp.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fo.bookmarksfly.cn

[Q28] 求和与平均
来源：http://ef.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hp.shxzskj.cn

[Q29] 最大最小值
来源：http://tw.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eg.hahajie.cn

[Q30] 分组统计
来源：http://iw.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pq.newstarts.cn

[Q31] 分组后过滤
来源：http://tr.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bl.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://jp.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qk.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nw.nicolike.cn

[Q33] 多列分组
来源：http://pp.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pj.huixiangedu.cn

[Q34] 每组取第一条
来源：http://gt.lnxyls.cn

SELECT * FROM (
来源：http://pj.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fg.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://pv.szxytkj.cn

[Q35] 内连接
来源：http://nb.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uq.panjiajie.cn

[Q36] 左连接
来源：http://ex.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nj.521024.cn

[Q37] 右连接
来源：http://nv.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kc.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ae.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://db.colortex.cn

[Q39] 自连接（查上下级）
来源：http://hv.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hn.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bh.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tj.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bw.lnxyls.cn

[Q41] 多表连接
来源：http://ga.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ie.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://yj.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://ep.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://sx.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://fa.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ma.colortex.cn

[Q43] 标量子查询
来源：http://mt.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mi.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://yd.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://om.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://qt.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vy.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qc.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bd.hahajie.cn

[Q47] 与平均值比较
来源：http://zs.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rm.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://zj.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ds.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://oh.9csxet.cn

[Q49] 更新单行
来源：http://wi.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mf.chemitech.net.cn

[Q50] 批量更新
来源：http://zo.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nk.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://vi.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xy.muxihuayi.cn

[Q52] 删除指定行
来源：http://eu.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://eq.jctech888.com.cn

[Q53] 按条件删除
来源：http://uz.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ix.panjiajie.cn

[Q54] 清空表
来源：http://cb.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://fq.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://em.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hq.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://ed.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qg.jctech888.com.cn

[Q57] 行号
来源：http://kq.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hv.szsharing.cn

[Q58] 累计求和
来源：http://ix.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://al.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://ds.szsharing.cn


<!-- 参考信息 -->
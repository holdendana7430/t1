代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ui.colortex.cn

[N10] 链表节点定义
来源：http://xl.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://da.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fr.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wu.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://is.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://wb.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gz.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jr.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xo.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://jd.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ih.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://kz.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cw.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xk.jianghongdianzi.cn

Java: // 手写递归
来源：http://jc.yuexingan06.cn

Go:   // 手写递归
来源：http://bq.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ek.wgjwhj.cn

C#:   // 手写递归
来源：http://om.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lg.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zg.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aw.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gl.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wx.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bf.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tm.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zc.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wf.shtwfgs.cn

================================================================================
来源：http://qh.shxzukj.cn

O. 并发与异步
来源：http://uv.chemitech.net.cn

================================================================================
来源：http://sx.bookmarksfly.cn

[O01] 启动一个线程
来源：http://mv.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kb.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zc.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gt.yuntaijiaju.cn

TS:   // 同 JS
来源：http://wg.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://nk.gzmigu.cn

Go:   go f()
来源：http://rr.colortex.cn

Ruby: Thread.new { f }
来源：http://ey.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://zq.szxytkj.cn

[O02] 使用线程池
来源：http://ic.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oz.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://da.521024.cn

JS:   // worker_threads 线程池
来源：http://mf.9csxet.cn

TS:   // worker_threads 线程池
来源：http://dm.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xa.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vl.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jt.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wf.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://pl.panjiajie.cn

Py:   with lock: shared += 1
来源：http://nv.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://xb.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://da.newstarts.cn

TS:   // 同 JS
来源：http://ts.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://ze.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qy.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kj.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://cd.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://jq.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://no.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vk.asd995.cn

JS:   async function f() { await g(); }
来源：http://cp.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aa.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qy.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ya.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iw.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://oj.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://ka.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://ky.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ao.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://xn.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://qh.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ag.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sv.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://xk.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://in.shxzukj.cn

[O06] 使用进程池
来源：http://iz.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ty.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gj.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://pt.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://yh.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dg.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://up.bjjhwx.cn

Ruby: // fork 块
来源：http://pf.huanxung.cn

C#:   Parallel.For
来源：http://wt.muxihuayi.cn

================================================================================
来源：http://we.szxytkj.cn

P. 常用工具函数
来源：http://jg.hnjuh.cn

================================================================================
来源：http://is.huanxung.cn

[P01] 生成 UUID
来源：http://ii.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://er.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ym.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://xp.521024.cn

TS:   crypto.randomUUID()
来源：http://xp.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://ev.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://zi.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://kk.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://ma.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://ef.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mc.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kx.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ro.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rs.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://du.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yh.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zd.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ai.huanxung.cn

[P03] 生成短随机字符串
来源：http://ep.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qn.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://js.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ei.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qk.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pm.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dp.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ba.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jl.huixiangedu.cn

[P04] 求长度
来源：http://mj.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sg.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dp.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mg.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ol.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://zv.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://jx.521024.cn

Ruby: x.length;  x.size
来源：http://yo.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jy.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://gu.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qn.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bh.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rr.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bn.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zo.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mf.nicolike.cn

Ruby: a == b
来源：http://ye.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://va.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ly.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ww.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ou.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hl.muxihuayi.cn

TS:   if (x == null) {}
来源：http://fv.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ds.bjjhwx.cn

Go:   if x == nil {}
来源：http://xw.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://up.shxzukj.cn

C#:   if (x is null) {}
来源：http://lp.nszjky.cn

[P07] 防抖与节流
来源：http://yn.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gt.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://bl.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bp.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kx.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ng.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qw.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qo.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fl.newstarts.cn

[P08] 处理浮点精度问题
来源：http://dm.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mv.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jr.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ec.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ay.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ar.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sd.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sc.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dj.9csxet.cn

================================================================================
来源：http://pj.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ks.521024.cn

================================================================================
来源：http://ub.colortex.cn

[Q01] 创建表
来源：http://nw.panjiajie.cn

CREATE TABLE users (
来源：http://bc.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gn.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://yu.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ig.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gc.jianghongdianzi.cn

);
来源：http://zc.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://pz.wgjwhj.cn

CREATE TABLE orders (
来源：http://mz.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ge.szxytkj.cn

user_id INT NOT NULL,
来源：http://jk.huanxung.cn

amount DECIMAL(10, 2),
来源：http://xt.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rc.lnxyls.cn

);
来源：http://vx.yuexingan06.cn

[Q03] 增加列
来源：http://mr.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vt.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://wn.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uo.lnxyls.cn

[Q05] 重命名列
来源：http://xu.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hj.szxytkj.cn

[Q06] 删除列
来源：http://bs.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rg.panjiajie.cn

[Q07] 删除表
来源：http://rk.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://vp.hnjuh.cn

[Q08] 创建普通索引
来源：http://xs.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qi.shxzukj.cn

[Q09] 创建唯一索引
来源：http://xj.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gg.hnjuh.cn

[Q10] 插入单行
来源：http://uz.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://if.huixiangedu.cn

[Q11] 一次插入多行
来源：http://vf.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://to.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://nu.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ks.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oy.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://vz.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nz.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://np.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wc.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nj.panjiajie.cn

[Q15] 查询全部
来源：http://cw.shxzskj.cn

SELECT * FROM users;
来源：http://up.huanxung.cn

[Q16] 查询指定列
来源：http://yq.nszjky.cn

SELECT id, name FROM users;
来源：http://al.jianghongdianzi.cn

[Q17] 条件查询
来源：http://no.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://do.lnxyls.cn

[Q18] 模糊匹配
来源：http://bd.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wk.jctech888.com.cn

[Q19] 范围查询
来源：http://tf.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tb.wgjwhj.cn

[Q20] IN 列表
来源：http://zb.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qc.haigaiapp.cn

[Q21] 空值判断
来源：http://lb.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pm.521024.cn

[Q22] 排序
来源：http://fa.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ex.asd995.cn

[Q23] 分页
来源：http://rj.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lo.hahajie.cn

[Q24] 去重
来源：http://ki.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://tm.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://oc.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jo.shtwfgs.cn

[Q26] 计数
来源：http://mz.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://wo.huixiangedu.cn

[Q27] 条件计数
来源：http://ne.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fn.521024.cn

[Q28] 求和与平均
来源：http://sc.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sk.lnxyls.cn

[Q29] 最大最小值
来源：http://mg.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://le.nszjky.cn

[Q30] 分组统计
来源：http://qe.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://du.nicolike.cn

[Q31] 分组后过滤
来源：http://yc.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bk.colortex.cn

[Q32] 分组拼接字符串
来源：http://ao.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mc.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gb.jianghongdianzi.cn

[Q33] 多列分组
来源：http://dj.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ii.wgjwhj.cn

[Q34] 每组取第一条
来源：http://jt.colortex.cn

SELECT * FROM (
来源：http://jd.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bu.shtwfgs.cn

) t WHERE rn = 1;
来源：http://hd.bookmarksfly.cn

[Q35] 内连接
来源：http://an.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nh.chemitech.net.cn

[Q36] 左连接
来源：http://hz.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rt.bjjhwx.cn

[Q37] 右连接
来源：http://na.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pj.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vs.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kp.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://jf.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dy.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ew.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eq.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uk.jctech888.com.cn

[Q41] 多表连接
来源：http://fi.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wf.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://jh.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://gu.asd995.cn

[Q42] 连接条件附加过滤
来源：http://yx.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://yy.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jl.nszjky.cn

[Q43] 标量子查询
来源：http://kz.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wu.lnxyls.cn

[Q44] IN 子查询
来源：http://rs.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wi.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://mb.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zt.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hs.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vt.szxytkj.cn

[Q47] 与平均值比较
来源：http://fc.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xv.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://wj.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ie.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://iu.bookmarksfly.cn

[Q49] 更新单行
来源：http://mp.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jb.muxihuayi.cn

[Q50] 批量更新
来源：http://ik.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wk.huanxung.cn

[Q51] 用子查询更新
来源：http://la.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rs.9csxet.cn

[Q52] 删除指定行
来源：http://gm.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://tn.shtwfgs.cn

[Q53] 按条件删除
来源：http://ql.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ej.haigaiapp.cn

[Q54] 清空表
来源：http://js.colortex.cn

TRUNCATE TABLE logs;
来源：http://on.nszjky.cn

[Q55] 排名（并列占位）
来源：http://ki.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sk.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://no.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ik.newstarts.cn

[Q57] 行号
来源：http://gy.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vw.jctech888.com.cn

[Q58] 累计求和
来源：http://rq.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xk.newstarts.cn

[Q59] 分组内累计
来源：http://ma.asd995.cn


<!-- 参考信息 -->
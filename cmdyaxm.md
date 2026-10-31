代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cc.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tg.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://sb.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hw.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ay.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zq.nszjky.cn

[N11] 二叉树中序遍历
来源：http://ie.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ny.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://oi.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ep.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://du.hnjuh.cn

Java: // 手写递归
来源：http://ae.huixinmuqiang.cn

Go:   // 手写递归
来源：http://sq.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ty.nicolike.cn

C#:   // 手写递归
来源：http://bv.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yr.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ix.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ag.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cs.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ic.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xp.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xq.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vf.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lx.nszjky.cn

================================================================================
来源：http://ga.huixiangedu.cn

O. 并发与异步
来源：http://wm.hahajie.cn

================================================================================
来源：http://rs.huixiangedu.cn

[O01] 启动一个线程
来源：http://xo.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qj.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zu.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uf.huixiangedu.cn

TS:   // 同 JS
来源：http://ir.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://uq.chemitech.net.cn

Go:   go f()
来源：http://tl.shxzskj.cn

Ruby: Thread.new { f }
来源：http://bi.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://ff.huixiangedu.cn

[O02] 使用线程池
来源：http://dt.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rk.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sc.huanxung.cn

JS:   // worker_threads 线程池
来源：http://ma.huanxung.cn

TS:   // worker_threads 线程池
来源：http://xz.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hv.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sx.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ai.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pm.nszjky.cn

[O03] 加锁保护共享数据
来源：http://np.huanxung.cn

Py:   with lock: shared += 1
来源：http://gc.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://im.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bs.bookmarksfly.cn

TS:   // 同 JS
来源：http://xm.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://df.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ed.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wk.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://rt.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://qz.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ub.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hm.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://pk.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fn.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tx.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mu.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qs.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://ja.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://ur.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://gp.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://te.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://tk.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://pj.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dy.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sm.nszjky.cn

Ruby: threads.map(&:join)
来源：http://jh.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://do.szxytkj.cn

[O06] 使用进程池
来源：http://vm.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zp.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yb.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://bk.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://zg.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ji.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dw.szxytkj.cn

Ruby: // fork 块
来源：http://wf.yuntaijiaju.cn

C#:   Parallel.For
来源：http://gq.gzmigu.cn

================================================================================
来源：http://gy.nicolike.cn

P. 常用工具函数
来源：http://hj.huanxung.cn

================================================================================
来源：http://rf.haigaiapp.cn

[P01] 生成 UUID
来源：http://hw.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://ld.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ct.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://ce.hahajie.cn

TS:   crypto.randomUUID()
来源：http://ja.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://xw.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://am.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://cl.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://pt.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://xs.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tn.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xb.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yc.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xf.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mj.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bm.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ki.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qy.gzmigu.cn

[P03] 生成短随机字符串
来源：http://sg.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bg.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gx.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ft.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fr.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tt.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cc.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uc.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gd.huixinmuqiang.cn

[P04] 求长度
来源：http://wb.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mx.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vo.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tu.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://de.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://gw.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://kd.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ha.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ag.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://sq.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kl.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pq.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ob.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nu.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ni.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ql.colortex.cn

Ruby: a == b
来源：http://gb.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fq.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pr.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uc.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://yx.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://as.bjjhwx.cn

TS:   if (x == null) {}
来源：http://sg.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jm.haigaiapp.cn

Go:   if x == nil {}
来源：http://li.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tm.9csxet.cn

C#:   if (x is null) {}
来源：http://uo.muxihuayi.cn

[P07] 防抖与节流
来源：http://yd.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cx.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://mm.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xn.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bz.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uf.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uj.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sb.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://xi.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bw.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bj.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://be.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dx.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xt.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bv.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ds.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fz.huixinmuqiang.cn

================================================================================
来源：http://zu.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gg.gzmigu.cn

================================================================================
来源：http://zd.521024.cn

[Q01] 创建表
来源：http://vw.shtwfgs.cn

CREATE TABLE users (
来源：http://ar.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://se.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://tr.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://oq.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ej.yuntaijiaju.cn

);
来源：http://tj.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://lc.huixiangedu.cn

CREATE TABLE orders (
来源：http://rq.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dp.bjjhwx.cn

user_id INT NOT NULL,
来源：http://um.newstarts.cn

amount DECIMAL(10, 2),
来源：http://fo.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gs.nszjky.cn

);
来源：http://ne.colortex.cn

[Q03] 增加列
来源：http://mj.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ee.yuexingan06.cn

[Q04] 修改列类型
来源：http://ht.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vq.szsharing.cn

[Q05] 重命名列
来源：http://dc.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zv.lnxyls.cn

[Q06] 删除列
来源：http://aj.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sg.wgjwhj.cn

[Q07] 删除表
来源：http://md.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://dy.nszjky.cn

[Q08] 创建普通索引
来源：http://yn.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vr.szxytkj.cn

[Q09] 创建唯一索引
来源：http://sk.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pj.szxytkj.cn

[Q10] 插入单行
来源：http://ej.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://in.haigaiapp.cn

[Q11] 一次插入多行
来源：http://ei.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hh.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://xc.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dr.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mo.newstarts.cn

[Q13] 忽略重复插入
来源：http://db.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jp.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://sm.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vy.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dw.haigaiapp.cn

[Q15] 查询全部
来源：http://qg.nicolike.cn

SELECT * FROM users;
来源：http://kc.shtwfgs.cn

[Q16] 查询指定列
来源：http://ky.asd995.cn

SELECT id, name FROM users;
来源：http://uo.bjjhwx.cn

[Q17] 条件查询
来源：http://uc.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rq.yuexingan06.cn

[Q18] 模糊匹配
来源：http://zj.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bj.nszjky.cn

[Q19] 范围查询
来源：http://az.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ou.shxzskj.cn

[Q20] IN 列表
来源：http://dk.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bb.jctech888.com.cn

[Q21] 空值判断
来源：http://eg.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://so.hahajie.cn

[Q22] 排序
来源：http://qn.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tk.hahajie.cn

[Q23] 分页
来源：http://zr.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wj.huanxung.cn

[Q24] 去重
来源：http://to.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://po.szsharing.cn

[Q25] 只取前 N 条
来源：http://mi.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ns.yuntaijiaju.cn

[Q26] 计数
来源：http://gd.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://ys.nszjky.cn

[Q27] 条件计数
来源：http://kx.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vs.wgjwhj.cn

[Q28] 求和与平均
来源：http://oi.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jz.yuexingan06.cn

[Q29] 最大最小值
来源：http://jv.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ov.szsharing.cn

[Q30] 分组统计
来源：http://pj.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ud.521024.cn

[Q31] 分组后过滤
来源：http://gf.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fw.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://wp.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lp.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kr.bookmarksfly.cn

[Q33] 多列分组
来源：http://vw.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yi.wgjwhj.cn

[Q34] 每组取第一条
来源：http://ja.521024.cn

SELECT * FROM (
来源：http://ei.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lx.panjiajie.cn

) t WHERE rn = 1;
来源：http://rt.hnjuh.cn

[Q35] 内连接
来源：http://jp.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xn.bjjhwx.cn

[Q36] 左连接
来源：http://at.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wf.shxzskj.cn

[Q37] 右连接
来源：http://td.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://db.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nc.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vh.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://an.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wp.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fo.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rg.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dw.haigaiapp.cn

[Q41] 多表连接
来源：http://ad.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wl.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://tn.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ya.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://pu.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://wc.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kc.9csxet.cn

[Q43] 标量子查询
来源：http://tp.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bz.nicolike.cn

[Q44] IN 子查询
来源：http://oi.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hl.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://iy.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oa.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rp.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ax.haigaiapp.cn

[Q47] 与平均值比较
来源：http://te.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vo.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://un.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kk.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://qo.yuntaijiaju.cn

[Q49] 更新单行
来源：http://qt.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ck.nszjky.cn

[Q50] 批量更新
来源：http://xq.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ok.haigaiapp.cn

[Q51] 用子查询更新
来源：http://jx.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wn.bjjhwx.cn

[Q52] 删除指定行
来源：http://qq.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://zu.gzmigu.cn

[Q53] 按条件删除
来源：http://zr.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bd.9csxet.cn

[Q54] 清空表
来源：http://oo.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://rn.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://yc.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qg.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://hg.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dw.colortex.cn

[Q57] 行号
来源：http://cu.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://td.yuexingan06.cn

[Q58] 累计求和
来源：http://zq.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jk.yuexingan06.cn

[Q59] 分组内累计
来源：http://yp.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gc.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://wb.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wu.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ic.szxytkj.cn


<!-- 参考信息 -->
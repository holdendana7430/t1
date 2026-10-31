代发 wailian999

PHP:  // 手写递归函数
来源：http://he.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ha.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.hahajie.cn

Java: // 手写递归
来源：http://mh.lnxyls.cn

Go:   // 手写递归
来源：http://np.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xw.jianghongdianzi.cn

C#:   // 手写递归
来源：http://mi.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yg.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://et.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cj.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://as.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kv.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wd.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ao.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xk.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tn.chemitech.net.cn

================================================================================
来源：http://dz.panjiajie.cn

O. 并发与异步
来源：http://ux.gzmigu.cn

================================================================================
来源：http://aa.nicolike.cn

[O01] 启动一个线程
来源：http://bm.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ih.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bg.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iz.bjjhwx.cn

TS:   // 同 JS
来源：http://hi.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://dj.jianghongdianzi.cn

Go:   go f()
来源：http://nc.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://nw.newstarts.cn

C#:   Task.Run(() => F());
来源：http://cp.chemitech.net.cn

[O02] 使用线程池
来源：http://wr.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ep.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dc.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ji.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://fk.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hl.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pb.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ir.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ao.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://vu.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hp.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://hc.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ub.haigaiapp.cn

TS:   // 同 JS
来源：http://nc.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://rv.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rh.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vi.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://qa.hahajie.cn

[O04] 定义异步函数并等待
来源：http://jb.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://th.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uk.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://vq.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zy.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ib.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oz.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jl.asd995.cn

C#:   async Task F() { await G(); }
来源：http://te.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://pp.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://nl.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://he.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://eo.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://br.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sz.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nw.9csxet.cn

Ruby: threads.map(&:join)
来源：http://tw.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zx.lnxyls.cn

[O06] 使用进程池
来源：http://io.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oy.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aw.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://uj.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://cq.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ef.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vm.haigaiapp.cn

Ruby: // fork 块
来源：http://gw.wgjwhj.cn

C#:   Parallel.For
来源：http://fr.szxytkj.cn

================================================================================
来源：http://xf.521024.cn

P. 常用工具函数
来源：http://tx.huixinmuqiang.cn

================================================================================
来源：http://lu.newstarts.cn

[P01] 生成 UUID
来源：http://dr.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://eu.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pv.521024.cn

JS:   crypto.randomUUID()
来源：http://wq.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://vp.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://if.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://ep.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://em.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://sh.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://fm.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kl.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kx.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://on.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gu.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hy.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://po.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jg.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sz.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://ap.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zt.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kd.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kh.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zv.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pt.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iw.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xw.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bj.bookmarksfly.cn

[P04] 求长度
来源：http://ci.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://di.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rq.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uk.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bj.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://ad.szsharing.cn

Go:   len(arr);  len(m)
来源：http://se.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://me.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://az.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://ry.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oa.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tr.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sp.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bb.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yx.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hx.muxihuayi.cn

Ruby: a == b
来源：http://wk.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ti.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lb.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bc.colortex.cn

PHP:  if (empty($x)) {}
来源：http://ri.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gk.yuexingan06.cn

TS:   if (x == null) {}
来源：http://uw.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://op.szxytkj.cn

Go:   if x == nil {}
来源：http://qz.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lp.bjjhwx.cn

C#:   if (x is null) {}
来源：http://sa.shxzukj.cn

[P07] 防抖与节流
来源：http://oy.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jo.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://nb.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://op.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rj.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ux.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pv.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hk.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ii.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://ey.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ti.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ju.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eg.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lj.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gp.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ze.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dj.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ji.bjjhwx.cn

================================================================================
来源：http://cn.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jo.shxzskj.cn

================================================================================
来源：http://sy.huixinmuqiang.cn

[Q01] 创建表
来源：http://yh.muxihuayi.cn

CREATE TABLE users (
来源：http://sc.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vo.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ix.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://lf.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cg.yuntaijiaju.cn

);
来源：http://ku.hahajie.cn

[Q02] 创建带外键的表
来源：http://km.shxzskj.cn

CREATE TABLE orders (
来源：http://ip.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://at.huanxung.cn

user_id INT NOT NULL,
来源：http://nq.szsharing.cn

amount DECIMAL(10, 2),
来源：http://bh.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://py.yuntaijiaju.cn

);
来源：http://hp.huanxung.cn

[Q03] 增加列
来源：http://mt.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dk.bjjhwx.cn

[Q04] 修改列类型
来源：http://jf.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vg.muxihuayi.cn

[Q05] 重命名列
来源：http://gk.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ol.9csxet.cn

[Q06] 删除列
来源：http://it.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qe.huanxung.cn

[Q07] 删除表
来源：http://oe.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://xn.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://be.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yj.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://zq.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uz.huixiangedu.cn

[Q10] 插入单行
来源：http://vp.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qt.wgjwhj.cn

[Q11] 一次插入多行
来源：http://va.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ci.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://uy.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://od.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qh.nicolike.cn

[Q13] 忽略重复插入
来源：http://jf.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ay.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://op.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tf.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ng.shxzskj.cn

[Q15] 查询全部
来源：http://xr.9csxet.cn

SELECT * FROM users;
来源：http://mf.haigaiapp.cn

[Q16] 查询指定列
来源：http://ba.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://nj.9csxet.cn

[Q17] 条件查询
来源：http://ad.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://py.521024.cn

[Q18] 模糊匹配
来源：http://is.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wo.521024.cn

[Q19] 范围查询
来源：http://yl.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qo.jianghongdianzi.cn

[Q20] IN 列表
来源：http://xq.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nk.jianghongdianzi.cn

[Q21] 空值判断
来源：http://ph.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ix.szsharing.cn

[Q22] 排序
来源：http://ud.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pj.huanxung.cn

[Q23] 分页
来源：http://mr.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qe.nszjky.cn

[Q24] 去重
来源：http://rb.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://bm.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://hs.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nf.jianghongdianzi.cn

[Q26] 计数
来源：http://il.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://zz.muxihuayi.cn

[Q27] 条件计数
来源：http://vt.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lq.huanxung.cn

[Q28] 求和与平均
来源：http://tj.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ro.jctech888.com.cn

[Q29] 最大最小值
来源：http://vs.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gg.shtwfgs.cn

[Q30] 分组统计
来源：http://jr.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sl.shtwfgs.cn

[Q31] 分组后过滤
来源：http://ky.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tl.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://de.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cj.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://to.jianghongdianzi.cn

[Q33] 多列分组
来源：http://cw.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hh.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://zl.lnxyls.cn

SELECT * FROM (
来源：http://kx.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qx.panjiajie.cn

) t WHERE rn = 1;
来源：http://es.huixiangedu.cn

[Q35] 内连接
来源：http://zf.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dm.jianghongdianzi.cn

[Q36] 左连接
来源：http://yd.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eg.shxzukj.cn

[Q37] 右连接
来源：http://rz.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lj.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vd.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zr.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://db.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pn.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ho.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sa.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jg.hnjuh.cn

[Q41] 多表连接
来源：http://xm.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qd.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://oi.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://wk.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://uq.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://hs.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ep.521024.cn

[Q43] 标量子查询
来源：http://ta.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cq.haigaiapp.cn

[Q44] IN 子查询
来源：http://le.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://da.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://xc.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kr.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ma.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yt.shtwfgs.cn

[Q47] 与平均值比较
来源：http://wy.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qg.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://ng.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://el.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://wg.shxzukj.cn

[Q49] 更新单行
来源：http://ka.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fw.wgjwhj.cn

[Q50] 批量更新
来源：http://mb.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hb.huixiangedu.cn

[Q51] 用子查询更新
来源：http://wz.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hv.nicolike.cn

[Q52] 删除指定行
来源：http://ay.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://co.hahajie.cn

[Q53] 按条件删除
来源：http://zt.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ex.gzmigu.cn

[Q54] 清空表
来源：http://ug.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://ry.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://mv.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sg.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://gk.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://il.shtwfgs.cn

[Q57] 行号
来源：http://tt.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xu.huixiangedu.cn

[Q58] 累计求和
来源：http://qh.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jd.bookmarksfly.cn

[Q59] 分组内累计
来源：http://px.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yb.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://vm.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fm.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rf.colortex.cn

[Q61] 移动平均
来源：http://uo.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uz.bjjhwx.cn

[Q62] 分组占比
来源：http://ac.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zk.nszjky.cn

[Q63] 开启事务
来源：http://az.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ef.muxihuayi.cn

[Q64] 提交事务
来源：http://kn.hahajie.cn

COMMIT;
来源：http://pr.colortex.cn


<!-- 参考信息 -->
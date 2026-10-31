代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vu.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://az.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pf.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hq.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jk.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://di.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mn.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tx.szxytkj.cn

================================================================================
来源：http://qf.jctech888.com.cn

O. 并发与异步
来源：http://ic.hnjuh.cn

================================================================================
来源：http://il.newstarts.cn

[O01] 启动一个线程
来源：http://hy.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mn.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ys.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cl.yuntaijiaju.cn

TS:   // 同 JS
来源：http://dm.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://ao.jianghongdianzi.cn

Go:   go f()
来源：http://dx.newstarts.cn

Ruby: Thread.new { f }
来源：http://it.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://wo.nicolike.cn

[O02] 使用线程池
来源：http://sm.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iw.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vq.colortex.cn

JS:   // worker_threads 线程池
来源：http://gt.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://eh.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ha.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oz.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zd.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eo.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://oy.shxzukj.cn

Py:   with lock: shared += 1
来源：http://yu.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://bh.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cr.newstarts.cn

TS:   // 同 JS
来源：http://nm.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://de.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kh.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qf.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://fa.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://wx.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://pq.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wc.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://ca.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wp.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yh.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zk.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ph.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://yo.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://ni.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://ke.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tn.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://rh.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://fw.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eu.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hv.newstarts.cn

Ruby: threads.map(&:join)
来源：http://hn.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tz.szsharing.cn

[O06] 使用进程池
来源：http://aj.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mw.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vs.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://nt.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://er.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nv.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ia.huanxung.cn

Ruby: // fork 块
来源：http://kl.gzmigu.cn

C#:   Parallel.For
来源：http://hy.bookmarksfly.cn

================================================================================
来源：http://us.shtwfgs.cn

P. 常用工具函数
来源：http://bh.nicolike.cn

================================================================================
来源：http://ph.szxytkj.cn

[P01] 生成 UUID
来源：http://aj.asd995.cn

Py:   str(uuid.uuid4())
来源：http://an.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qk.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://xa.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://ya.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://ci.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://jv.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://df.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://zd.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://mo.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zw.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qy.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://in.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wj.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://of.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bc.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://er.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rr.9csxet.cn

[P03] 生成短随机字符串
来源：http://rb.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wn.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wn.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vw.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ws.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rh.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qo.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cv.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gx.jianghongdianzi.cn

[P04] 求长度
来源：http://hx.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://py.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iw.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ks.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qw.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://dp.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://yk.colortex.cn

Ruby: x.length;  x.size
来源：http://vr.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vk.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://sf.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xk.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sj.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pc.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dz.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bl.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://or.muxihuayi.cn

Ruby: a == b
来源：http://ep.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ky.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ir.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uu.asd995.cn

PHP:  if (empty($x)) {}
来源：http://kl.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cz.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://gf.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qb.shxzukj.cn

Go:   if x == nil {}
来源：http://vt.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yu.panjiajie.cn

C#:   if (x is null) {}
来源：http://tx.chemitech.net.cn

[P07] 防抖与节流
来源：http://xp.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gn.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://je.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ct.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xz.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ir.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xf.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ey.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ye.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://nb.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ja.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pc.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sl.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dt.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zx.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://go.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fq.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fr.colortex.cn

================================================================================
来源：http://gl.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sf.huixiangedu.cn

================================================================================
来源：http://pt.9csxet.cn

[Q01] 创建表
来源：http://og.chemitech.net.cn

CREATE TABLE users (
来源：http://vi.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gb.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://ml.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://dc.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rf.bjjhwx.cn

);
来源：http://cz.9csxet.cn

[Q02] 创建带外键的表
来源：http://qo.szxytkj.cn

CREATE TABLE orders (
来源：http://vv.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cv.chemitech.net.cn

user_id INT NOT NULL,
来源：http://qa.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://kj.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zu.huixiangedu.cn

);
来源：http://yo.huixinmuqiang.cn

[Q03] 增加列
来源：http://ig.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ku.nszjky.cn

[Q04] 修改列类型
来源：http://hh.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ev.haigaiapp.cn

[Q05] 重命名列
来源：http://xa.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wq.bookmarksfly.cn

[Q06] 删除列
来源：http://gf.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ro.521024.cn

[Q07] 删除表
来源：http://ak.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://jb.bjjhwx.cn

[Q08] 创建普通索引
来源：http://am.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ja.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://vs.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://to.huixinmuqiang.cn

[Q10] 插入单行
来源：http://tm.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ii.chemitech.net.cn

[Q11] 一次插入多行
来源：http://im.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tq.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://qj.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ix.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://op.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://xe.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://in.521024.cn

[Q14] 存在则更新（upsert）
来源：http://fd.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xj.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fx.haigaiapp.cn

[Q15] 查询全部
来源：http://ba.szsharing.cn

SELECT * FROM users;
来源：http://st.szsharing.cn

[Q16] 查询指定列
来源：http://hy.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://xf.panjiajie.cn

[Q17] 条件查询
来源：http://am.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xg.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://xm.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sk.shtwfgs.cn

[Q19] 范围查询
来源：http://wd.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tx.gzmigu.cn

[Q20] IN 列表
来源：http://cv.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qq.gzmigu.cn

[Q21] 空值判断
来源：http://jv.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kz.gzmigu.cn

[Q22] 排序
来源：http://mk.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ik.shxzskj.cn

[Q23] 分页
来源：http://dv.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hq.shtwfgs.cn

[Q24] 去重
来源：http://cf.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://ia.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://mw.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nk.huanxung.cn

[Q26] 计数
来源：http://cx.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://fh.bjjhwx.cn

[Q27] 条件计数
来源：http://qi.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nu.huanxung.cn

[Q28] 求和与平均
来源：http://zu.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ir.szxytkj.cn

[Q29] 最大最小值
来源：http://of.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tk.newstarts.cn

[Q30] 分组统计
来源：http://ey.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ce.yuexingan06.cn

[Q31] 分组后过滤
来源：http://ht.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hq.szsharing.cn

[Q32] 分组拼接字符串
来源：http://yx.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hl.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fg.panjiajie.cn

[Q33] 多列分组
来源：http://qd.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dk.wgjwhj.cn

[Q34] 每组取第一条
来源：http://me.bjjhwx.cn

SELECT * FROM (
来源：http://cy.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gg.newstarts.cn

) t WHERE rn = 1;
来源：http://xa.chemitech.net.cn

[Q35] 内连接
来源：http://op.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qc.yuntaijiaju.cn

[Q36] 左连接
来源：http://rg.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gf.szsharing.cn

[Q37] 右连接
来源：http://xy.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zi.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zx.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cc.asd995.cn

[Q39] 自连接（查上下级）
来源：http://eg.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hu.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hn.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hv.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gu.jctech888.com.cn

[Q41] 多表连接
来源：http://na.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oy.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://cy.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://ye.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://jh.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://xj.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ds.szxytkj.cn

[Q43] 标量子查询
来源：http://by.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cq.colortex.cn

[Q44] IN 子查询
来源：http://bj.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gp.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://zb.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hl.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lm.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ee.jctech888.com.cn

[Q47] 与平均值比较
来源：http://dl.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bx.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://uc.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tn.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://ur.yuntaijiaju.cn

[Q49] 更新单行
来源：http://fj.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sh.shxzukj.cn

[Q50] 批量更新
来源：http://rz.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gp.chemitech.net.cn

[Q51] 用子查询更新
来源：http://rc.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bn.chemitech.net.cn

[Q52] 删除指定行
来源：http://aw.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://ov.hnjuh.cn

[Q53] 按条件删除
来源：http://lm.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wg.haigaiapp.cn

[Q54] 清空表
来源：http://xi.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://wg.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://ps.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tp.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://gi.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sl.bookmarksfly.cn

[Q57] 行号
来源：http://ir.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ci.yuexingan06.cn

[Q58] 累计求和
来源：http://au.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uu.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://pg.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pu.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://nk.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dq.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pm.muxihuayi.cn

[Q61] 移动平均
来源：http://ql.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mw.9csxet.cn

[Q62] 分组占比
来源：http://oj.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://we.colortex.cn

[Q63] 开启事务
来源：http://jx.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ho.521024.cn

[Q64] 提交事务
来源：http://mb.haigaiapp.cn

COMMIT;
来源：http://nq.asd995.cn

[Q65] 回滚事务
来源：http://ff.muxihuayi.cn

ROLLBACK;
来源：http://wc.asd995.cn

[Q66] 行锁查询
来源：http://qg.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qs.lnxyls.cn

[Q67] 设置隔离级别
来源：http://iw.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oc.panjiajie.cn

[Q68] 保存点
来源：http://tk.panjiajie.cn

SAVEPOINT sp1;
来源：http://rg.huixiangedu.cn


<!-- 参考信息 -->
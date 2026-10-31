代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ut.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sn.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dj.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nw.newstarts.cn

================================================================================
来源：http://sx.shtwfgs.cn

O. 并发与异步
来源：http://fq.9csxet.cn

================================================================================
来源：http://bk.huanxung.cn

[O01] 启动一个线程
来源：http://qw.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nr.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ga.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zh.huixinmuqiang.cn

TS:   // 同 JS
来源：http://lf.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://ww.yuntaijiaju.cn

Go:   go f()
来源：http://uy.gzmigu.cn

Ruby: Thread.new { f }
来源：http://kc.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://on.hnjuh.cn

[O02] 使用线程池
来源：http://ti.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xs.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sz.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://sd.nicolike.cn

TS:   // worker_threads 线程池
来源：http://je.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rq.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wz.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cl.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ey.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://vt.nicolike.cn

Py:   with lock: shared += 1
来源：http://ws.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://ip.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ss.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ht.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://of.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ai.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qv.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://gz.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://tt.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://cr.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zl.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://hd.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xk.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hd.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gt.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ks.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://gm.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://lx.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://in.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hx.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://xp.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://qm.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vn.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iu.hahajie.cn

Ruby: threads.map(&:join)
来源：http://ke.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ry.bjjhwx.cn

[O06] 使用进程池
来源：http://nc.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dd.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wg.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://ui.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://de.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fq.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tm.gzmigu.cn

Ruby: // fork 块
来源：http://ki.wgjwhj.cn

C#:   Parallel.For
来源：http://iy.hnjuh.cn

================================================================================
来源：http://mf.bjjhwx.cn

P. 常用工具函数
来源：http://sl.colortex.cn

================================================================================
来源：http://tp.lnxyls.cn

[P01] 生成 UUID
来源：http://tj.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://ki.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hi.hahajie.cn

JS:   crypto.randomUUID()
来源：http://fb.huanxung.cn

TS:   crypto.randomUUID()
来源：http://zc.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://ni.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://dd.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://lt.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://hn.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://fv.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ou.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dv.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gn.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jo.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xo.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zy.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ef.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cb.huanxung.cn

[P03] 生成短随机字符串
来源：http://el.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tr.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kx.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iz.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zu.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kb.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ng.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pg.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nx.gzmigu.cn

[P04] 求长度
来源：http://mj.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dt.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tq.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://db.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ro.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://rq.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://rd.panjiajie.cn

Ruby: x.length;  x.size
来源：http://ui.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://po.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://ku.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mi.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lk.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://om.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vb.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pt.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wl.hnjuh.cn

Ruby: a == b
来源：http://xm.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bt.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yq.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ce.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://xk.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bq.nicolike.cn

TS:   if (x == null) {}
来源：http://ot.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fb.nicolike.cn

Go:   if x == nil {}
来源：http://og.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ro.szsharing.cn

C#:   if (x is null) {}
来源：http://lf.bjjhwx.cn

[P07] 防抖与节流
来源：http://mr.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vc.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://wa.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nf.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bq.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ao.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nl.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dx.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iq.9csxet.cn

[P08] 处理浮点精度问题
来源：http://og.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wl.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kn.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://od.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tu.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wx.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jw.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cl.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pp.gzmigu.cn

================================================================================
来源：http://xr.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bb.szxytkj.cn

================================================================================
来源：http://wg.colortex.cn

[Q01] 创建表
来源：http://hg.huixiangedu.cn

CREATE TABLE users (
来源：http://xn.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jy.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://se.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://lb.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ju.shxzskj.cn

);
来源：http://rq.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://du.521024.cn

CREATE TABLE orders (
来源：http://qv.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ow.wgjwhj.cn

user_id INT NOT NULL,
来源：http://ly.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://oy.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gq.bjjhwx.cn

);
来源：http://gi.hnjuh.cn

[Q03] 增加列
来源：http://ms.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://il.huanxung.cn

[Q04] 修改列类型
来源：http://zk.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://da.wgjwhj.cn

[Q05] 重命名列
来源：http://dy.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bv.jianghongdianzi.cn

[Q06] 删除列
来源：http://kz.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qg.chemitech.net.cn

[Q07] 删除表
来源：http://fu.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://ui.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://id.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jl.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://yp.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vp.szsharing.cn

[Q10] 插入单行
来源：http://dc.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://su.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://dy.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ek.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://qf.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ke.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sw.colortex.cn

[Q13] 忽略重复插入
来源：http://oc.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ye.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://dn.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jl.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sh.lnxyls.cn

[Q15] 查询全部
来源：http://do.muxihuayi.cn

SELECT * FROM users;
来源：http://sg.nszjky.cn

[Q16] 查询指定列
来源：http://kd.chemitech.net.cn

SELECT id, name FROM users;
来源：http://dw.muxihuayi.cn

[Q17] 条件查询
来源：http://tq.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kw.colortex.cn

[Q18] 模糊匹配
来源：http://at.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://me.shtwfgs.cn

[Q19] 范围查询
来源：http://ae.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mx.hnjuh.cn

[Q20] IN 列表
来源：http://an.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gz.newstarts.cn

[Q21] 空值判断
来源：http://jj.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jx.huixinmuqiang.cn

[Q22] 排序
来源：http://bs.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kl.huixinmuqiang.cn

[Q23] 分页
来源：http://cy.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ea.bookmarksfly.cn

[Q24] 去重
来源：http://cn.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://kx.szxytkj.cn

[Q25] 只取前 N 条
来源：http://yo.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ml.nszjky.cn

[Q26] 计数
来源：http://pl.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://yd.9csxet.cn

[Q27] 条件计数
来源：http://gd.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ny.szxytkj.cn

[Q28] 求和与平均
来源：http://lj.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://df.asd995.cn

[Q29] 最大最小值
来源：http://oh.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hx.szxytkj.cn

[Q30] 分组统计
来源：http://zv.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yf.szsharing.cn

[Q31] 分组后过滤
来源：http://fh.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fy.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://cp.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eh.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hi.bookmarksfly.cn

[Q33] 多列分组
来源：http://pl.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qg.asd995.cn

[Q34] 每组取第一条
来源：http://mn.szsharing.cn

SELECT * FROM (
来源：http://lf.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uz.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://ad.huixinmuqiang.cn

[Q35] 内连接
来源：http://ox.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mb.colortex.cn

[Q36] 左连接
来源：http://ak.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gw.newstarts.cn

[Q37] 右连接
来源：http://na.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xf.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qe.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yj.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://tj.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ce.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gm.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://es.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sn.gzmigu.cn

[Q41] 多表连接
来源：http://xf.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qz.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://kt.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ho.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://jy.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://kc.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fs.bjjhwx.cn

[Q43] 标量子查询
来源：http://tz.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ca.lnxyls.cn

[Q44] IN 子查询
来源：http://oe.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lz.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://aq.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ej.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xs.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ii.hnjuh.cn

[Q47] 与平均值比较
来源：http://et.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://md.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://oq.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ol.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ac.asd995.cn

[Q49] 更新单行
来源：http://cz.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fm.shtwfgs.cn

[Q50] 批量更新
来源：http://iq.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gf.nicolike.cn

[Q51] 用子查询更新
来源：http://fq.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ks.szsharing.cn

[Q52] 删除指定行
来源：http://sl.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://zv.gzmigu.cn

[Q53] 按条件删除
来源：http://qg.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wk.chemitech.net.cn

[Q54] 清空表
来源：http://gq.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://xe.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ya.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gq.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://da.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fw.newstarts.cn

[Q57] 行号
来源：http://ah.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ah.shxzskj.cn

[Q58] 累计求和
来源：http://ch.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jp.colortex.cn

[Q59] 分组内累计
来源：http://ge.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bg.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://kn.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://if.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pm.shxzskj.cn

[Q61] 移动平均
来源：http://ho.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cu.huixinmuqiang.cn

[Q62] 分组占比
来源：http://iv.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tv.muxihuayi.cn

[Q63] 开启事务
来源：http://sv.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mo.newstarts.cn

[Q64] 提交事务
来源：http://bw.jianghongdianzi.cn

COMMIT;
来源：http://hb.shtwfgs.cn

[Q65] 回滚事务
来源：http://iy.nszjky.cn

ROLLBACK;
来源：http://zx.asd995.cn

[Q66] 行锁查询
来源：http://aa.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fe.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://dv.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gg.bjjhwx.cn

[Q68] 保存点
来源：http://pq.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://id.hnjuh.cn

ROLLBACK TO sp1;
来源：http://zi.haigaiapp.cn

[Q69] 查看执行计划
来源：http://dj.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ip.muxihuayi.cn

[Q70] 更新统计信息
来源：http://vc.nszjky.cn


<!-- 参考信息 -->
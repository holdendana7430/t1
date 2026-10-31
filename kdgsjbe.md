代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yl.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lf.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jp.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ie.nicolike.cn

================================================================================
来源：http://ar.shtwfgs.cn

O. 并发与异步
来源：http://fm.szxytkj.cn

================================================================================
来源：http://ag.colortex.cn

[O01] 启动一个线程
来源：http://ya.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aq.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mh.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yn.nicolike.cn

TS:   // 同 JS
来源：http://nq.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ts.haigaiapp.cn

Go:   go f()
来源：http://rl.szsharing.cn

Ruby: Thread.new { f }
来源：http://wc.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://uw.chemitech.net.cn

[O02] 使用线程池
来源：http://yz.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vx.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ne.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://xt.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://aw.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fa.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rb.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kb.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://et.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://we.colortex.cn

Py:   with lock: shared += 1
来源：http://ia.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://zy.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uj.521024.cn

TS:   // 同 JS
来源：http://mb.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://va.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mn.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qx.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://tf.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://ot.colortex.cn

Py:   async def f():⏎    await g()
来源：http://ag.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eu.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://ju.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fj.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pe.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tc.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gz.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://dl.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://go.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://ww.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vl.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://ov.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://un.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://au.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hb.hahajie.cn

Ruby: threads.map(&:join)
来源：http://dq.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://et.muxihuayi.cn

[O06] 使用进程池
来源：http://jr.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rn.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dd.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://lz.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://fu.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qj.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fa.jianghongdianzi.cn

Ruby: // fork 块
来源：http://kp.szxytkj.cn

C#:   Parallel.For
来源：http://ek.colortex.cn

================================================================================
来源：http://xg.szxytkj.cn

P. 常用工具函数
来源：http://fj.chemitech.net.cn

================================================================================
来源：http://vk.haigaiapp.cn

[P01] 生成 UUID
来源：http://dh.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://pf.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jp.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://jl.asd995.cn

TS:   crypto.randomUUID()
来源：http://gm.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://xd.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://rr.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://fw.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://ep.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://qt.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iv.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oz.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wh.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sz.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ay.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://id.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ow.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xq.huanxung.cn

[P03] 生成短随机字符串
来源：http://bh.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://id.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://et.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eh.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gw.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kf.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://re.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qf.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aw.nicolike.cn

[P04] 求长度
来源：http://jx.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kl.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mw.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tk.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pr.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://oy.nszjky.cn

Go:   len(arr);  len(m)
来源：http://kz.shxzskj.cn

Ruby: x.length;  x.size
来源：http://ut.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ew.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://wi.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hd.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qc.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yt.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ji.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cr.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ir.9csxet.cn

Ruby: a == b
来源：http://fu.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wa.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dv.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fz.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://nn.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ds.shxzskj.cn

TS:   if (x == null) {}
来源：http://xg.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nv.haigaiapp.cn

Go:   if x == nil {}
来源：http://zs.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://is.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://ms.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ws.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qv.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://df.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sa.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pt.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ad.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ak.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hn.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yg.521024.cn

[P08] 处理浮点精度问题
来源：http://sx.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kt.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ez.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qd.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xr.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sc.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qx.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jz.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vq.shxzukj.cn

================================================================================
来源：http://py.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sk.hnjuh.cn

================================================================================
来源：http://ww.521024.cn

[Q01] 创建表
来源：http://jx.haigaiapp.cn

CREATE TABLE users (
来源：http://ok.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vt.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://kt.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://go.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mu.hahajie.cn

);
来源：http://sc.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://lf.asd995.cn

CREATE TABLE orders (
来源：http://is.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mm.huixiangedu.cn

user_id INT NOT NULL,
来源：http://wd.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://vg.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dj.shtwfgs.cn

);
来源：http://cx.huanxung.cn

[Q03] 增加列
来源：http://pv.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kt.chemitech.net.cn

[Q04] 修改列类型
来源：http://iz.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kr.bjjhwx.cn

[Q05] 重命名列
来源：http://dm.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wv.nszjky.cn

[Q06] 删除列
来源：http://xi.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sr.huanxung.cn

[Q07] 删除表
来源：http://yf.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://av.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://yk.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wj.szsharing.cn

[Q09] 创建唯一索引
来源：http://uu.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ph.nszjky.cn

[Q10] 插入单行
来源：http://zf.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fu.colortex.cn

[Q11] 一次插入多行
来源：http://bt.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ka.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://ff.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jw.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rm.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://wm.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qe.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://nx.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oj.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qy.huixiangedu.cn

[Q15] 查询全部
来源：http://oh.lnxyls.cn

SELECT * FROM users;
来源：http://mf.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://qt.huanxung.cn

SELECT id, name FROM users;
来源：http://of.521024.cn

[Q17] 条件查询
来源：http://rz.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dh.yuexingan06.cn

[Q18] 模糊匹配
来源：http://hd.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://by.jianghongdianzi.cn

[Q19] 范围查询
来源：http://mk.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zi.colortex.cn

[Q20] IN 列表
来源：http://fq.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zw.szxytkj.cn

[Q21] 空值判断
来源：http://mn.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dx.szxytkj.cn

[Q22] 排序
来源：http://tl.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pq.huixiangedu.cn

[Q23] 分页
来源：http://vf.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tq.yuexingan06.cn

[Q24] 去重
来源：http://vk.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://yb.nicolike.cn

[Q25] 只取前 N 条
来源：http://mo.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hn.jianghongdianzi.cn

[Q26] 计数
来源：http://lb.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://im.hnjuh.cn

[Q27] 条件计数
来源：http://sp.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ti.panjiajie.cn

[Q28] 求和与平均
来源：http://ml.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dy.bookmarksfly.cn

[Q29] 最大最小值
来源：http://ap.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yw.colortex.cn

[Q30] 分组统计
来源：http://mf.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rg.asd995.cn

[Q31] 分组后过滤
来源：http://an.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://za.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://fp.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lv.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jo.shtwfgs.cn

[Q33] 多列分组
来源：http://dc.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://se.shtwfgs.cn

[Q34] 每组取第一条
来源：http://uh.hahajie.cn

SELECT * FROM (
来源：http://bn.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ik.asd995.cn

) t WHERE rn = 1;
来源：http://dl.jianghongdianzi.cn

[Q35] 内连接
来源：http://zl.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wg.9csxet.cn

[Q36] 左连接
来源：http://og.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qm.nicolike.cn

[Q37] 右连接
来源：http://hh.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rr.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hi.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ds.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://of.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wf.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ap.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ba.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.lnxyls.cn

[Q41] 多表连接
来源：http://lt.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sp.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://tq.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://ey.asd995.cn

[Q42] 连接条件附加过滤
来源：http://pq.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://pg.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rc.jctech888.com.cn

[Q43] 标量子查询
来源：http://aa.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ch.asd995.cn

[Q44] IN 子查询
来源：http://lb.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hv.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://lp.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vn.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ut.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qm.jctech888.com.cn

[Q47] 与平均值比较
来源：http://bh.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fw.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://ct.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jg.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://yp.huixiangedu.cn

[Q49] 更新单行
来源：http://fi.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eg.huixinmuqiang.cn

[Q50] 批量更新
来源：http://pj.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sm.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://nl.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gw.yuexingan06.cn

[Q52] 删除指定行
来源：http://pr.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://di.wgjwhj.cn

[Q53] 按条件删除
来源：http://vv.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gw.wgjwhj.cn

[Q54] 清空表
来源：http://ca.9csxet.cn

TRUNCATE TABLE logs;
来源：http://cn.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://ue.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gm.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://em.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zo.jianghongdianzi.cn

[Q57] 行号
来源：http://tu.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rx.lnxyls.cn

[Q58] 累计求和
来源：http://ph.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vy.bookmarksfly.cn

[Q59] 分组内累计
来源：http://em.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pm.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://fw.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zg.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bz.wgjwhj.cn

[Q61] 移动平均
来源：http://yv.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ay.szsharing.cn

[Q62] 分组占比
来源：http://dk.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jz.yuntaijiaju.cn

[Q63] 开启事务
来源：http://pg.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lm.haigaiapp.cn

[Q64] 提交事务
来源：http://az.hnjuh.cn

COMMIT;
来源：http://od.szsharing.cn

[Q65] 回滚事务
来源：http://gg.jctech888.com.cn

ROLLBACK;
来源：http://rs.szxytkj.cn

[Q66] 行锁查询
来源：http://jn.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ao.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://my.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ns.nicolike.cn

[Q68] 保存点
来源：http://py.hahajie.cn

SAVEPOINT sp1;
来源：http://ze.asd995.cn

ROLLBACK TO sp1;
来源：http://pu.521024.cn

[Q69] 查看执行计划
来源：http://xi.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lb.szsharing.cn

[Q70] 更新统计信息
来源：http://hl.huixiangedu.cn


<!-- 参考信息 -->
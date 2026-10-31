代发 wailian999

================================================================================
来源：http://fd.jctech888.com.cn

O. 并发与异步
来源：http://ep.wgjwhj.cn

================================================================================
来源：http://zz.huixiangedu.cn

[O01] 启动一个线程
来源：http://hf.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://km.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fv.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ha.muxihuayi.cn

TS:   // 同 JS
来源：http://vl.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://we.muxihuayi.cn

Go:   go f()
来源：http://ps.shxzskj.cn

Ruby: Thread.new { f }
来源：http://eo.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://by.hahajie.cn

[O02] 使用线程池
来源：http://my.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cb.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://le.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://ru.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://nf.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ki.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hx.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dd.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kn.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://hq.asd995.cn

Py:   with lock: shared += 1
来源：http://jp.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://jv.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qa.hahajie.cn

TS:   // 同 JS
来源：http://xp.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://lg.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xo.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rc.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://yn.huanxung.cn

[O04] 定义异步函数并等待
来源：http://jv.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://xh.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dl.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://ie.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kt.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hg.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vp.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cf.colortex.cn

C#:   async Task F() { await G(); }
来源：http://jo.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://xm.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://sw.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ty.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://nu.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://kb.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pt.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rg.9csxet.cn

Ruby: threads.map(&:join)
来源：http://um.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ub.jianghongdianzi.cn

[O06] 使用进程池
来源：http://rz.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ob.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ne.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://nu.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://as.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dl.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ag.muxihuayi.cn

Ruby: // fork 块
来源：http://fi.nicolike.cn

C#:   Parallel.For
来源：http://eg.szsharing.cn

================================================================================
来源：http://ke.asd995.cn

P. 常用工具函数
来源：http://or.shxzukj.cn

================================================================================
来源：http://kv.bjjhwx.cn

[P01] 生成 UUID
来源：http://wy.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://oi.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fp.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://tw.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://fd.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://gh.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://hf.521024.cn

Ruby: SecureRandom.uuid
来源：http://ad.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://uo.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://au.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qq.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bu.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://px.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kn.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ae.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gx.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kk.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pg.huanxung.cn

[P03] 生成短随机字符串
来源：http://sz.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yr.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lr.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bm.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rm.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tl.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sd.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kc.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://on.asd995.cn

[P04] 求长度
来源：http://yr.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ls.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sz.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oz.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nj.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://ku.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://oz.shxzukj.cn

Ruby: x.length;  x.size
来源：http://sg.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zr.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://yn.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jl.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fp.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qx.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zx.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mw.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lu.chemitech.net.cn

Ruby: a == b
来源：http://vl.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lp.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yc.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rs.521024.cn

PHP:  if (empty($x)) {}
来源：http://rp.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ut.nicolike.cn

TS:   if (x == null) {}
来源：http://qf.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://za.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://hi.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oq.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://pj.nicolike.cn

[P07] 防抖与节流
来源：http://yw.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tr.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://eb.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sg.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ac.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xn.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://az.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pw.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sz.asd995.cn

[P08] 处理浮点精度问题
来源：http://ie.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gq.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ow.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qw.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xv.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kv.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://li.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gg.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sv.hnjuh.cn

================================================================================
来源：http://ky.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jb.hnjuh.cn

================================================================================
来源：http://ft.521024.cn

[Q01] 创建表
来源：http://eu.huixiangedu.cn

CREATE TABLE users (
来源：http://bo.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qu.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://ws.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://nu.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://py.lnxyls.cn

);
来源：http://cf.lnxyls.cn

[Q02] 创建带外键的表
来源：http://jd.bookmarksfly.cn

CREATE TABLE orders (
来源：http://rb.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://by.asd995.cn

user_id INT NOT NULL,
来源：http://mq.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://tm.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kw.chemitech.net.cn

);
来源：http://zh.wgjwhj.cn

[Q03] 增加列
来源：http://du.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hl.hnjuh.cn

[Q04] 修改列类型
来源：http://xu.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yk.szxytkj.cn

[Q05] 重命名列
来源：http://qf.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qf.muxihuayi.cn

[Q06] 删除列
来源：http://me.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sk.shxzukj.cn

[Q07] 删除表
来源：http://lp.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://yt.szxytkj.cn

[Q08] 创建普通索引
来源：http://sx.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://do.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://fy.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ob.lnxyls.cn

[Q10] 插入单行
来源：http://xu.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gs.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://sz.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ef.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://tm.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ts.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ck.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://bp.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mw.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://lx.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ba.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dc.huixiangedu.cn

[Q15] 查询全部
来源：http://bi.nszjky.cn

SELECT * FROM users;
来源：http://sd.bookmarksfly.cn

[Q16] 查询指定列
来源：http://sc.szxytkj.cn

SELECT id, name FROM users;
来源：http://vx.asd995.cn

[Q17] 条件查询
来源：http://le.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://by.shtwfgs.cn

[Q18] 模糊匹配
来源：http://ii.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gh.panjiajie.cn

[Q19] 范围查询
来源：http://yr.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hf.bookmarksfly.cn

[Q20] IN 列表
来源：http://wk.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://us.colortex.cn

[Q21] 空值判断
来源：http://zm.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dm.9csxet.cn

[Q22] 排序
来源：http://no.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kp.asd995.cn

[Q23] 分页
来源：http://el.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://du.lnxyls.cn

[Q24] 去重
来源：http://kp.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://wt.nszjky.cn

[Q25] 只取前 N 条
来源：http://mr.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zq.9csxet.cn

[Q26] 计数
来源：http://pw.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://yu.colortex.cn

[Q27] 条件计数
来源：http://jx.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qv.szsharing.cn

[Q28] 求和与平均
来源：http://bo.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tp.521024.cn

[Q29] 最大最小值
来源：http://it.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qa.shxzskj.cn

[Q30] 分组统计
来源：http://ll.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ts.szxytkj.cn

[Q31] 分组后过滤
来源：http://wg.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://km.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://lg.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mu.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xv.haigaiapp.cn

[Q33] 多列分组
来源：http://db.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aq.hahajie.cn

[Q34] 每组取第一条
来源：http://ti.shtwfgs.cn

SELECT * FROM (
来源：http://gc.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tk.bjjhwx.cn

) t WHERE rn = 1;
来源：http://vj.shxzukj.cn

[Q35] 内连接
来源：http://iv.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rn.shxzukj.cn

[Q36] 左连接
来源：http://gp.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sc.yuexingan06.cn

[Q37] 右连接
来源：http://jo.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://he.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lt.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rk.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://tw.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kp.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sa.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cg.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wt.yuexingan06.cn

[Q41] 多表连接
来源：http://gb.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xp.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ns.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://oj.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://og.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://xm.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://se.521024.cn

[Q43] 标量子查询
来源：http://fo.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ov.bookmarksfly.cn

[Q44] IN 子查询
来源：http://sr.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jn.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://wg.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ri.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nl.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lp.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://bd.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uj.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://tk.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wh.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://fx.shxzukj.cn

[Q49] 更新单行
来源：http://eh.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bz.chemitech.net.cn

[Q50] 批量更新
来源：http://bw.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://by.hahajie.cn

[Q51] 用子查询更新
来源：http://zi.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vy.muxihuayi.cn

[Q52] 删除指定行
来源：http://yv.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://hm.gzmigu.cn

[Q53] 按条件删除
来源：http://mp.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yg.shxzskj.cn

[Q54] 清空表
来源：http://iu.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://xx.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://bx.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oz.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://pi.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ls.szsharing.cn

[Q57] 行号
来源：http://dd.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iz.shxzukj.cn

[Q58] 累计求和
来源：http://ml.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://de.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://zs.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sq.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://zk.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pi.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://af.muxihuayi.cn

[Q61] 移动平均
来源：http://sp.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ly.newstarts.cn

[Q62] 分组占比
来源：http://rq.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ie.yuntaijiaju.cn

[Q63] 开启事务
来源：http://hd.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sg.huanxung.cn

[Q64] 提交事务
来源：http://mk.lnxyls.cn

COMMIT;
来源：http://on.shxzskj.cn

[Q65] 回滚事务
来源：http://aq.yuntaijiaju.cn

ROLLBACK;
来源：http://ju.panjiajie.cn

[Q66] 行锁查询
来源：http://ea.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oq.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://bg.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ed.bjjhwx.cn

[Q68] 保存点
来源：http://mv.yuexingan06.cn

SAVEPOINT sp1;
来源：http://nu.9csxet.cn

ROLLBACK TO sp1;
来源：http://xp.newstarts.cn

[Q69] 查看执行计划
来源：http://mk.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yv.szxytkj.cn

[Q70] 更新统计信息
来源：http://ps.muxihuayi.cn

ANALYZE TABLE users;
来源：http://kg.nszjky.cn

[Q71] 查看建表语句
来源：http://bd.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qh.haigaiapp.cn

[Q72] 查看索引
来源：http://gl.521024.cn


<!-- 参考信息 -->
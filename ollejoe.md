代发 wailian999

[O02] 使用线程池
来源：http://si.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nz.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qg.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://xu.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://az.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ht.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ao.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ki.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jn.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://qi.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://pt.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://er.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://og.bookmarksfly.cn

TS:   // 同 JS
来源：http://du.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://ot.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bz.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kv.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://zf.asd995.cn

[O04] 定义异步函数并等待
来源：http://mz.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://gx.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hw.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://gn.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cp.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sq.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://em.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ll.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://mt.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://xd.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://eg.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bq.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://fi.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://vc.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://em.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ww.newstarts.cn

Ruby: threads.map(&:join)
来源：http://ja.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tr.asd995.cn

[O06] 使用进程池
来源：http://cy.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yt.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yj.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://jg.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://an.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wp.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gx.bookmarksfly.cn

Ruby: // fork 块
来源：http://vl.huixiangedu.cn

C#:   Parallel.For
来源：http://fc.huixiangedu.cn

================================================================================
来源：http://ov.yuexingan06.cn

P. 常用工具函数
来源：http://mz.yuexingan06.cn

================================================================================
来源：http://vw.panjiajie.cn

[P01] 生成 UUID
来源：http://dq.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://lq.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yn.huanxung.cn

JS:   crypto.randomUUID()
来源：http://je.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://qw.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://fn.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://wa.asd995.cn

Ruby: SecureRandom.uuid
来源：http://po.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://be.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://xv.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xs.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://np.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xl.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gi.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wz.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fg.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dj.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lp.9csxet.cn

[P03] 生成短随机字符串
来源：http://oy.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kd.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ym.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://au.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xd.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mn.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bj.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pd.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qt.huixiangedu.cn

[P04] 求长度
来源：http://jj.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aq.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dj.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xd.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://te.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://sp.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://pa.lnxyls.cn

Ruby: x.length;  x.size
来源：http://ju.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gj.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ra.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://he.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qy.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vm.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xu.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oh.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ls.asd995.cn

Ruby: a == b
来源：http://wu.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hq.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pa.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lw.colortex.cn

PHP:  if (empty($x)) {}
来源：http://xy.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ud.hahajie.cn

TS:   if (x == null) {}
来源：http://pj.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tl.hahajie.cn

Go:   if x == nil {}
来源：http://zd.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hw.wgjwhj.cn

C#:   if (x is null) {}
来源：http://zp.chemitech.net.cn

[P07] 防抖与节流
来源：http://oo.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ec.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://xe.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://st.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ir.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jv.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pl.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zp.9csxet.cn

[P08] 处理浮点精度问题
来源：http://yt.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nh.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pd.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nq.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ve.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bo.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yt.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fd.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uh.yuexingan06.cn

================================================================================
来源：http://hu.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rl.shtwfgs.cn

================================================================================
来源：http://su.521024.cn

[Q01] 创建表
来源：http://pd.chemitech.net.cn

CREATE TABLE users (
来源：http://fk.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ws.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ql.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://uz.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kt.yuexingan06.cn

);
来源：http://xr.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://lw.huanxung.cn

CREATE TABLE orders (
来源：http://mo.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yi.bjjhwx.cn

user_id INT NOT NULL,
来源：http://tc.colortex.cn

amount DECIMAL(10, 2),
来源：http://co.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fa.9csxet.cn

);
来源：http://pb.hnjuh.cn

[Q03] 增加列
来源：http://tk.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vd.muxihuayi.cn

[Q04] 修改列类型
来源：http://pa.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://km.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ev.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ag.shtwfgs.cn

[Q06] 删除列
来源：http://pf.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pa.yuexingan06.cn

[Q07] 删除表
来源：http://qo.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://mk.lnxyls.cn

[Q08] 创建普通索引
来源：http://wl.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ff.panjiajie.cn

[Q09] 创建唯一索引
来源：http://ej.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://el.muxihuayi.cn

[Q10] 插入单行
来源：http://mu.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ck.hahajie.cn

[Q11] 一次插入多行
来源：http://vc.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hr.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://yz.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ce.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sd.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://nc.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uw.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://gg.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rv.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ic.panjiajie.cn

[Q15] 查询全部
来源：http://bn.shxzskj.cn

SELECT * FROM users;
来源：http://op.lnxyls.cn

[Q16] 查询指定列
来源：http://ob.nszjky.cn

SELECT id, name FROM users;
来源：http://dd.szxytkj.cn

[Q17] 条件查询
来源：http://mt.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wy.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://eb.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cp.huixiangedu.cn

[Q19] 范围查询
来源：http://ok.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wy.hnjuh.cn

[Q20] IN 列表
来源：http://gk.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lq.521024.cn

[Q21] 空值判断
来源：http://bl.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ys.lnxyls.cn

[Q22] 排序
来源：http://vz.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tz.9csxet.cn

[Q23] 分页
来源：http://zr.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sy.szsharing.cn

[Q24] 去重
来源：http://kl.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://ya.asd995.cn

[Q25] 只取前 N 条
来源：http://zj.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://an.newstarts.cn

[Q26] 计数
来源：http://qz.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://fr.huixiangedu.cn

[Q27] 条件计数
来源：http://zq.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yb.panjiajie.cn

[Q28] 求和与平均
来源：http://ms.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vh.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://ds.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lr.shxzukj.cn

[Q30] 分组统计
来源：http://au.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ar.shtwfgs.cn

[Q31] 分组后过滤
来源：http://sq.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xg.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://rs.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nw.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ul.wgjwhj.cn

[Q33] 多列分组
来源：http://xf.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fr.newstarts.cn

[Q34] 每组取第一条
来源：http://cw.shxzskj.cn

SELECT * FROM (
来源：http://gz.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mc.huixiangedu.cn

) t WHERE rn = 1;
来源：http://fw.jctech888.com.cn

[Q35] 内连接
来源：http://dr.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qr.jctech888.com.cn

[Q36] 左连接
来源：http://oa.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://az.hahajie.cn

[Q37] 右连接
来源：http://hk.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ea.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://at.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qc.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://qf.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://og.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ju.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sk.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rb.nszjky.cn

[Q41] 多表连接
来源：http://kc.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uq.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://wn.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://kk.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://nc.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://ek.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://io.shxzskj.cn

[Q43] 标量子查询
来源：http://zp.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zh.haigaiapp.cn

[Q44] IN 子查询
来源：http://pq.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tg.asd995.cn

[Q45] EXISTS 判断存在
来源：http://nm.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kb.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kb.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gh.jctech888.com.cn

[Q47] 与平均值比较
来源：http://iw.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://us.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://vw.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kv.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://dj.bookmarksfly.cn

[Q49] 更新单行
来源：http://dl.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ii.newstarts.cn

[Q50] 批量更新
来源：http://mo.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://il.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://do.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://un.bjjhwx.cn

[Q52] 删除指定行
来源：http://qp.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://qz.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://sm.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ci.nicolike.cn

[Q54] 清空表
来源：http://db.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://vr.521024.cn

[Q55] 排名（并列占位）
来源：http://mq.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ba.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://nf.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://on.asd995.cn

[Q57] 行号
来源：http://ze.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mz.panjiajie.cn

[Q58] 累计求和
来源：http://uo.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zt.szsharing.cn

[Q59] 分组内累计
来源：http://so.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ih.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://bt.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ad.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jl.jianghongdianzi.cn

[Q61] 移动平均
来源：http://nf.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xe.shxzukj.cn

[Q62] 分组占比
来源：http://rc.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ho.panjiajie.cn

[Q63] 开启事务
来源：http://rb.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vy.wgjwhj.cn

[Q64] 提交事务
来源：http://uu.shxzukj.cn

COMMIT;
来源：http://dc.chemitech.net.cn

[Q65] 回滚事务
来源：http://ii.huixinmuqiang.cn

ROLLBACK;
来源：http://xm.jctech888.com.cn

[Q66] 行锁查询
来源：http://ni.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lm.szsharing.cn

[Q67] 设置隔离级别
来源：http://ca.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jb.hnjuh.cn

[Q68] 保存点
来源：http://dz.newstarts.cn

SAVEPOINT sp1;
来源：http://qa.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://hf.lnxyls.cn

[Q69] 查看执行计划
来源：http://bz.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://on.bjjhwx.cn

[Q70] 更新统计信息
来源：http://jb.muxihuayi.cn

ANALYZE TABLE users;
来源：http://km.nszjky.cn

[Q71] 查看建表语句
来源：http://ee.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mo.colortex.cn

[Q72] 查看索引
来源：http://ok.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://fo.lnxyls.cn

[Q73] 查看表状态
来源：http://mu.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ti.521024.cn

[Q74] 强制使用索引
来源：http://zc.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jx.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://ie.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mv.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hl.nszjky.cn

[Q76] 按天统计
来源：http://wq.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xu.huanxung.cn

[Q77] 时间加减
来源：http://yk.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lx.newstarts.cn


<!-- 参考信息 -->
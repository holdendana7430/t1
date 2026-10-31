代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://zx.wgjwhj.cn

Go:   go f()
来源：http://sh.gzmigu.cn

Ruby: Thread.new { f }
来源：http://cn.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://he.hahajie.cn

[O02] 使用线程池
来源：http://sv.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cp.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nq.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://km.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://qa.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ic.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kf.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://du.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hq.521024.cn

[O03] 加锁保护共享数据
来源：http://hi.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://ve.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://re.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zt.szsharing.cn

TS:   // 同 JS
来源：http://ap.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://bk.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ol.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tv.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://mz.asd995.cn

[O04] 定义异步函数并等待
来源：http://dd.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://to.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bq.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://fs.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fl.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qc.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gx.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://up.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://ff.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://me.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://bk.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ww.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://mf.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://cg.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fv.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://st.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://cs.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xn.huixiangedu.cn

[O06] 使用进程池
来源：http://xf.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://er.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tv.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://so.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://fk.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jr.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hx.shtwfgs.cn

Ruby: // fork 块
来源：http://cg.huixiangedu.cn

C#:   Parallel.For
来源：http://mq.521024.cn

================================================================================
来源：http://rh.nicolike.cn

P. 常用工具函数
来源：http://mm.chemitech.net.cn

================================================================================
来源：http://ih.9csxet.cn

[P01] 生成 UUID
来源：http://ym.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://wp.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pr.hahajie.cn

JS:   crypto.randomUUID()
来源：http://fr.hahajie.cn

TS:   crypto.randomUUID()
来源：http://dv.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://db.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://ag.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://rl.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://fw.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://tp.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://at.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gr.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://en.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://py.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cr.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fk.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oo.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://da.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://dm.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ub.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jx.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gs.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iy.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://di.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tm.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xk.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qs.asd995.cn

[P04] 求长度
来源：http://zm.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dd.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lh.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cs.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://un.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://yg.nszjky.cn

Go:   len(arr);  len(m)
来源：http://rr.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://qe.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ep.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://wk.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xm.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ej.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zm.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lm.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qp.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fr.hnjuh.cn

Ruby: a == b
来源：http://lx.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ch.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://if.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wt.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://cr.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ff.nszjky.cn

TS:   if (x == null) {}
来源：http://fx.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rg.muxihuayi.cn

Go:   if x == nil {}
来源：http://le.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cp.muxihuayi.cn

C#:   if (x is null) {}
来源：http://up.huixiangedu.cn

[P07] 防抖与节流
来源：http://nc.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lg.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://oj.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jq.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tc.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ao.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qe.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qa.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dr.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://qs.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ic.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xb.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wp.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uw.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gt.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mq.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ae.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fg.9csxet.cn

================================================================================
来源：http://er.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rt.nszjky.cn

================================================================================
来源：http://wb.panjiajie.cn

[Q01] 创建表
来源：http://bc.hahajie.cn

CREATE TABLE users (
来源：http://lk.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cz.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://zy.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://ez.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gu.haigaiapp.cn

);
来源：http://ag.szxytkj.cn

[Q02] 创建带外键的表
来源：http://iu.lnxyls.cn

CREATE TABLE orders (
来源：http://vo.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dc.muxihuayi.cn

user_id INT NOT NULL,
来源：http://zd.newstarts.cn

amount DECIMAL(10, 2),
来源：http://bl.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zw.shxzskj.cn

);
来源：http://gv.asd995.cn

[Q03] 增加列
来源：http://ci.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oo.huanxung.cn

[Q04] 修改列类型
来源：http://cc.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cs.shtwfgs.cn

[Q05] 重命名列
来源：http://nd.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://px.gzmigu.cn

[Q06] 删除列
来源：http://re.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qy.bjjhwx.cn

[Q07] 删除表
来源：http://si.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://wz.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://gl.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ah.asd995.cn

[Q09] 创建唯一索引
来源：http://na.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eu.huanxung.cn

[Q10] 插入单行
来源：http://tc.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://as.shtwfgs.cn

[Q11] 一次插入多行
来源：http://xr.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rk.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://tm.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://px.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pk.szsharing.cn

[Q13] 忽略重复插入
来源：http://jc.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hx.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://wp.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ca.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mx.huixinmuqiang.cn

[Q15] 查询全部
来源：http://om.nszjky.cn

SELECT * FROM users;
来源：http://lc.521024.cn

[Q16] 查询指定列
来源：http://ve.huixiangedu.cn

SELECT id, name FROM users;
来源：http://qy.nszjky.cn

[Q17] 条件查询
来源：http://oj.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zd.szsharing.cn

[Q18] 模糊匹配
来源：http://ap.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bt.shtwfgs.cn

[Q19] 范围查询
来源：http://oy.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lc.muxihuayi.cn

[Q20] IN 列表
来源：http://ga.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lq.shxzskj.cn

[Q21] 空值判断
来源：http://wt.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vd.colortex.cn

[Q22] 排序
来源：http://cg.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xo.nicolike.cn

[Q23] 分页
来源：http://bn.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://st.newstarts.cn

[Q24] 去重
来源：http://fg.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://bf.huanxung.cn

[Q25] 只取前 N 条
来源：http://dq.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hw.hahajie.cn

[Q26] 计数
来源：http://nk.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://qk.521024.cn

[Q27] 条件计数
来源：http://ud.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fs.chemitech.net.cn

[Q28] 求和与平均
来源：http://zm.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ea.nicolike.cn

[Q29] 最大最小值
来源：http://in.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uh.newstarts.cn

[Q30] 分组统计
来源：http://ip.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vs.huanxung.cn

[Q31] 分组后过滤
来源：http://gy.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nm.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://qi.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ql.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tb.yuexingan06.cn

[Q33] 多列分组
来源：http://oi.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cc.hahajie.cn

[Q34] 每组取第一条
来源：http://fw.nicolike.cn

SELECT * FROM (
来源：http://aw.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kt.9csxet.cn

) t WHERE rn = 1;
来源：http://cf.bookmarksfly.cn

[Q35] 内连接
来源：http://ks.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eg.shxzukj.cn

[Q36] 左连接
来源：http://da.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ev.jianghongdianzi.cn

[Q37] 右连接
来源：http://us.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vy.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zc.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xw.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://gb.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dk.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eu.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qc.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aw.colortex.cn

[Q41] 多表连接
来源：http://cc.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tt.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://yo.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://cz.521024.cn

[Q42] 连接条件附加过滤
来源：http://do.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://sb.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://io.haigaiapp.cn

[Q43] 标量子查询
来源：http://ao.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fq.chemitech.net.cn

[Q44] IN 子查询
来源：http://xi.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jl.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://rr.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hi.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fd.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dn.muxihuayi.cn

[Q47] 与平均值比较
来源：http://yz.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ss.colortex.cn

[Q48] CTE 公用表表达式
来源：http://hx.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dj.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://bq.521024.cn

[Q49] 更新单行
来源：http://yv.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ps.haigaiapp.cn

[Q50] 批量更新
来源：http://ju.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lg.bjjhwx.cn

[Q51] 用子查询更新
来源：http://om.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zh.shxzskj.cn

[Q52] 删除指定行
来源：http://mf.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://cp.shtwfgs.cn

[Q53] 按条件删除
来源：http://dm.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fs.shtwfgs.cn

[Q54] 清空表
来源：http://ts.colortex.cn

TRUNCATE TABLE logs;
来源：http://pf.newstarts.cn

[Q55] 排名（并列占位）
来源：http://zh.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tc.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://gb.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gc.gzmigu.cn

[Q57] 行号
来源：http://sl.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dy.nicolike.cn

[Q58] 累计求和
来源：http://kq.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qc.panjiajie.cn

[Q59] 分组内累计
来源：http://zj.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ix.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://zu.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tr.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ud.muxihuayi.cn

[Q61] 移动平均
来源：http://lr.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iv.haigaiapp.cn

[Q62] 分组占比
来源：http://wx.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ih.huanxung.cn

[Q63] 开启事务
来源：http://wo.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gd.hnjuh.cn

[Q64] 提交事务
来源：http://lo.hnjuh.cn

COMMIT;
来源：http://wo.asd995.cn

[Q65] 回滚事务
来源：http://pr.shxzukj.cn

ROLLBACK;
来源：http://ye.haigaiapp.cn

[Q66] 行锁查询
来源：http://bj.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dj.szsharing.cn

[Q67] 设置隔离级别
来源：http://jl.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://da.521024.cn

[Q68] 保存点
来源：http://om.panjiajie.cn

SAVEPOINT sp1;
来源：http://qd.szsharing.cn

ROLLBACK TO sp1;
来源：http://ke.newstarts.cn

[Q69] 查看执行计划
来源：http://fd.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gw.shxzskj.cn

[Q70] 更新统计信息
来源：http://pk.huanxung.cn

ANALYZE TABLE users;
来源：http://dx.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://uv.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cz.gzmigu.cn

[Q72] 查看索引
来源：http://ab.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://vm.lnxyls.cn

[Q73] 查看表状态
来源：http://kc.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rv.shxzskj.cn

[Q74] 强制使用索引
来源：http://is.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dc.jctech888.com.cn

[Q75] 日期格式化
来源：http://te.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://le.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://se.nszjky.cn


<!-- 参考信息 -->
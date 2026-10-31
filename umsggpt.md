代发 wailian999

[O02] 使用线程池
来源：http://ck.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zy.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://il.hahajie.cn

JS:   // worker_threads 线程池
来源：http://pw.huanxung.cn

TS:   // worker_threads 线程池
来源：http://ee.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rt.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cr.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sl.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ef.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://qh.shxzskj.cn

Py:   with lock: shared += 1
来源：http://hw.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://xg.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lj.asd995.cn

TS:   // 同 JS
来源：http://xf.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://ud.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ia.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ec.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://ic.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://qk.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://au.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hd.nicolike.cn

JS:   async function f() { await g(); }
来源：http://jv.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rx.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bn.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ta.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xt.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://ic.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://pi.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://on.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lq.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://co.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://fo.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jp.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zd.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://zp.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dw.shxzskj.cn

[O06] 使用进程池
来源：http://qq.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ai.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://om.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://px.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://kw.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://du.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://op.shxzukj.cn

Ruby: // fork 块
来源：http://ub.newstarts.cn

C#:   Parallel.For
来源：http://db.shxzskj.cn

================================================================================
来源：http://kz.gzmigu.cn

P. 常用工具函数
来源：http://vd.jctech888.com.cn

================================================================================
来源：http://no.panjiajie.cn

[P01] 生成 UUID
来源：http://kt.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://vc.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bp.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ze.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://fa.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://ng.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://lf.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://at.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://gs.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://dc.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ln.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nz.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ic.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ac.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://et.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wn.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hy.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uc.huanxung.cn

[P03] 生成短随机字符串
来源：http://sl.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ns.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ne.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aj.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sd.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://he.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dv.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wk.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tu.hahajie.cn

[P04] 求长度
来源：http://tg.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gj.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sj.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sk.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bi.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://kj.hahajie.cn

Go:   len(arr);  len(m)
来源：http://qg.521024.cn

Ruby: x.length;  x.size
来源：http://zn.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lc.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://uu.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wg.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sj.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mm.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://na.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ma.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ds.muxihuayi.cn

Ruby: a == b
来源：http://dw.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hp.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gd.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mu.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://by.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nv.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://fr.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aj.szxytkj.cn

Go:   if x == nil {}
来源：http://mm.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://za.shxzskj.cn

C#:   if (x is null) {}
来源：http://hi.bookmarksfly.cn

[P07] 防抖与节流
来源：http://jh.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jk.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://pi.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hc.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lh.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fa.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hf.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wi.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mi.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://kv.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wk.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xt.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xz.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vp.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tg.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vc.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://me.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gk.bookmarksfly.cn

================================================================================
来源：http://jr.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pf.bjjhwx.cn

================================================================================
来源：http://te.nicolike.cn

[Q01] 创建表
来源：http://cl.bjjhwx.cn

CREATE TABLE users (
来源：http://ew.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qu.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ji.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://ff.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rc.lnxyls.cn

);
来源：http://lp.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://ej.nszjky.cn

CREATE TABLE orders (
来源：http://ty.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lu.szsharing.cn

user_id INT NOT NULL,
来源：http://en.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://om.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dm.9csxet.cn

);
来源：http://yh.huixiangedu.cn

[Q03] 增加列
来源：http://mf.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lm.hahajie.cn

[Q04] 修改列类型
来源：http://vp.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iz.521024.cn

[Q05] 重命名列
来源：http://le.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hg.bjjhwx.cn

[Q06] 删除列
来源：http://ab.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jv.muxihuayi.cn

[Q07] 删除表
来源：http://nk.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://xc.gzmigu.cn

[Q08] 创建普通索引
来源：http://xd.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ba.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://qw.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iy.shxzskj.cn

[Q10] 插入单行
来源：http://pq.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fl.huixiangedu.cn

[Q11] 一次插入多行
来源：http://zd.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zs.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://sm.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ss.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uj.hahajie.cn

[Q13] 忽略重复插入
来源：http://vl.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pw.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://rm.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://da.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oz.bjjhwx.cn

[Q15] 查询全部
来源：http://pd.newstarts.cn

SELECT * FROM users;
来源：http://dk.muxihuayi.cn

[Q16] 查询指定列
来源：http://jj.muxihuayi.cn

SELECT id, name FROM users;
来源：http://zw.haigaiapp.cn

[Q17] 条件查询
来源：http://xt.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sn.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://rh.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mn.bookmarksfly.cn

[Q19] 范围查询
来源：http://xh.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xw.lnxyls.cn

[Q20] IN 列表
来源：http://fn.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dj.hnjuh.cn

[Q21] 空值判断
来源：http://tj.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vt.hnjuh.cn

[Q22] 排序
来源：http://fu.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rc.huanxung.cn

[Q23] 分页
来源：http://lf.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ut.wgjwhj.cn

[Q24] 去重
来源：http://yx.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://zw.hnjuh.cn

[Q25] 只取前 N 条
来源：http://nc.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sl.chemitech.net.cn

[Q26] 计数
来源：http://fe.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://nr.haigaiapp.cn

[Q27] 条件计数
来源：http://dl.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zz.szsharing.cn

[Q28] 求和与平均
来源：http://fk.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kc.shxzskj.cn

[Q29] 最大最小值
来源：http://id.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hr.hahajie.cn

[Q30] 分组统计
来源：http://dz.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gs.shxzskj.cn

[Q31] 分组后过滤
来源：http://nj.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qe.hahajie.cn

[Q32] 分组拼接字符串
来源：http://ca.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dx.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jg.gzmigu.cn

[Q33] 多列分组
来源：http://re.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://il.521024.cn

[Q34] 每组取第一条
来源：http://bp.asd995.cn

SELECT * FROM (
来源：http://er.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bl.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://ez.szxytkj.cn

[Q35] 内连接
来源：http://kb.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uj.panjiajie.cn

[Q36] 左连接
来源：http://fv.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vy.newstarts.cn

[Q37] 右连接
来源：http://yd.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://px.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://af.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cp.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://su.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hj.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ih.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sr.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qt.521024.cn

[Q41] 多表连接
来源：http://pm.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gg.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://ea.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://il.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://ig.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://bn.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://km.nicolike.cn

[Q43] 标量子查询
来源：http://ag.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vz.wgjwhj.cn

[Q44] IN 子查询
来源：http://wc.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nu.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://gs.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ot.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xw.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ba.haigaiapp.cn

[Q47] 与平均值比较
来源：http://zp.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://si.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://xw.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ud.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://pz.huixiangedu.cn

[Q49] 更新单行
来源：http://tm.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qn.gzmigu.cn

[Q50] 批量更新
来源：http://wl.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cx.521024.cn

[Q51] 用子查询更新
来源：http://lx.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rh.chemitech.net.cn

[Q52] 删除指定行
来源：http://uo.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://bj.9csxet.cn

[Q53] 按条件删除
来源：http://xr.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yl.nszjky.cn

[Q54] 清空表
来源：http://ez.newstarts.cn

TRUNCATE TABLE logs;
来源：http://ki.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://zt.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eu.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://pp.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://de.muxihuayi.cn

[Q57] 行号
来源：http://ae.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yx.colortex.cn

[Q58] 累计求和
来源：http://zh.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mt.gzmigu.cn

[Q59] 分组内累计
来源：http://eg.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ut.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://mo.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kd.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qw.huixinmuqiang.cn

[Q61] 移动平均
来源：http://ej.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gi.szsharing.cn

[Q62] 分组占比
来源：http://fu.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ds.bjjhwx.cn

[Q63] 开启事务
来源：http://zu.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wu.haigaiapp.cn

[Q64] 提交事务
来源：http://nb.haigaiapp.cn

COMMIT;
来源：http://yy.yuexingan06.cn

[Q65] 回滚事务
来源：http://qb.muxihuayi.cn

ROLLBACK;
来源：http://qo.shxzukj.cn

[Q66] 行锁查询
来源：http://ho.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bz.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://ty.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://go.521024.cn

[Q68] 保存点
来源：http://ro.wgjwhj.cn

SAVEPOINT sp1;
来源：http://hq.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://xz.yuexingan06.cn

[Q69] 查看执行计划
来源：http://yp.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rz.wgjwhj.cn

[Q70] 更新统计信息
来源：http://th.shxzukj.cn

ANALYZE TABLE users;
来源：http://bv.nicolike.cn

[Q71] 查看建表语句
来源：http://df.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sw.bjjhwx.cn

[Q72] 查看索引
来源：http://bh.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://hw.9csxet.cn

[Q73] 查看表状态
来源：http://xf.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lh.gzmigu.cn

[Q74] 强制使用索引
来源：http://rn.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://te.haigaiapp.cn

[Q75] 日期格式化
来源：http://wb.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qr.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ud.muxihuayi.cn

[Q76] 按天统计
来源：http://rn.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ho.9csxet.cn

[Q77] 时间加减
来源：http://np.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dr.colortex.cn


<!-- 参考信息 -->
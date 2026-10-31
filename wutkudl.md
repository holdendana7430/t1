代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ut.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://zw.szxytkj.cn

Py:   with lock: shared += 1
来源：http://mj.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://eo.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nl.chemitech.net.cn

TS:   // 同 JS
来源：http://ya.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://ze.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yn.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cx.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://kd.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://cf.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://hg.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ec.huanxung.cn

JS:   async function f() { await g(); }
来源：http://az.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://th.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ps.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ts.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cz.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://bv.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://oa.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://qi.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://in.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://ec.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://gq.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ya.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ix.nszjky.cn

Ruby: threads.map(&:join)
来源：http://pg.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ff.gzmigu.cn

[O06] 使用进程池
来源：http://hu.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ie.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qe.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://fd.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://ir.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tv.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cm.nicolike.cn

Ruby: // fork 块
来源：http://ku.shxzskj.cn

C#:   Parallel.For
来源：http://to.newstarts.cn

================================================================================
来源：http://qp.huixinmuqiang.cn

P. 常用工具函数
来源：http://md.newstarts.cn

================================================================================
来源：http://st.shxzskj.cn

[P01] 生成 UUID
来源：http://ol.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://ep.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pw.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://yg.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ws.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://db.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://rl.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://mo.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://km.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://tx.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zf.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fz.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ir.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gh.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ek.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xm.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fl.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hs.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://on.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ba.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mo.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rf.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mw.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xn.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ua.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ce.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ts.nszjky.cn

[P04] 求长度
来源：http://fe.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fw.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://un.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gf.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rq.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://do.huanxung.cn

Go:   len(arr);  len(m)
来源：http://uy.521024.cn

Ruby: x.length;  x.size
来源：http://cp.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pi.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ut.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dy.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ac.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://to.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gq.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jn.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zp.colortex.cn

Ruby: a == b
来源：http://dt.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qh.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vv.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://di.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://vw.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ox.yuexingan06.cn

TS:   if (x == null) {}
来源：http://jx.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mf.szxytkj.cn

Go:   if x == nil {}
来源：http://aq.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zo.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://bo.521024.cn

[P07] 防抖与节流
来源：http://uw.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lg.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://qi.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://em.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cn.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yj.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iv.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fl.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nx.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://qx.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oc.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jg.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kr.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hx.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iz.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tf.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wh.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://un.haigaiapp.cn

================================================================================
来源：http://uf.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wu.szsharing.cn

================================================================================
来源：http://xe.szxytkj.cn

[Q01] 创建表
来源：http://gs.jctech888.com.cn

CREATE TABLE users (
来源：http://km.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sz.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://zh.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://ge.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mv.bjjhwx.cn

);
来源：http://hi.hnjuh.cn

[Q02] 创建带外键的表
来源：http://db.panjiajie.cn

CREATE TABLE orders (
来源：http://nz.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qo.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://th.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://vi.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hf.panjiajie.cn

);
来源：http://yx.gzmigu.cn

[Q03] 增加列
来源：http://it.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xg.chemitech.net.cn

[Q04] 修改列类型
来源：http://tv.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jw.colortex.cn

[Q05] 重命名列
来源：http://cv.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://df.jianghongdianzi.cn

[Q06] 删除列
来源：http://ek.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uf.jctech888.com.cn

[Q07] 删除表
来源：http://lk.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://ap.colortex.cn

[Q08] 创建普通索引
来源：http://zk.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qv.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://qg.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pl.huixinmuqiang.cn

[Q10] 插入单行
来源：http://ov.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aw.lnxyls.cn

[Q11] 一次插入多行
来源：http://kx.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xe.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://rp.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kn.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sf.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://dl.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hu.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://tc.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bj.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pa.chemitech.net.cn

[Q15] 查询全部
来源：http://rr.9csxet.cn

SELECT * FROM users;
来源：http://rk.lnxyls.cn

[Q16] 查询指定列
来源：http://kb.panjiajie.cn

SELECT id, name FROM users;
来源：http://vq.huanxung.cn

[Q17] 条件查询
来源：http://vg.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dx.asd995.cn

[Q18] 模糊匹配
来源：http://pj.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zu.szxytkj.cn

[Q19] 范围查询
来源：http://hv.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ll.9csxet.cn

[Q20] IN 列表
来源：http://rm.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bw.colortex.cn

[Q21] 空值判断
来源：http://yk.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hh.hnjuh.cn

[Q22] 排序
来源：http://tp.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pl.bookmarksfly.cn

[Q23] 分页
来源：http://eu.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bz.newstarts.cn

[Q24] 去重
来源：http://qk.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://us.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://sl.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vk.newstarts.cn

[Q26] 计数
来源：http://st.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://vn.panjiajie.cn

[Q27] 条件计数
来源：http://dk.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fm.jctech888.com.cn

[Q28] 求和与平均
来源：http://ob.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vz.521024.cn

[Q29] 最大最小值
来源：http://ex.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mc.yuntaijiaju.cn

[Q30] 分组统计
来源：http://om.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mr.shxzukj.cn

[Q31] 分组后过滤
来源：http://ds.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mg.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://fb.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kw.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xl.shtwfgs.cn

[Q33] 多列分组
来源：http://pc.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zl.521024.cn

[Q34] 每组取第一条
来源：http://ut.szsharing.cn

SELECT * FROM (
来源：http://pn.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pa.newstarts.cn

) t WHERE rn = 1;
来源：http://kq.nicolike.cn

[Q35] 内连接
来源：http://zl.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zp.colortex.cn

[Q36] 左连接
来源：http://wx.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bb.jianghongdianzi.cn

[Q37] 右连接
来源：http://xr.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://re.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oj.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mc.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://yp.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ob.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eo.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ez.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gm.huixiangedu.cn

[Q41] 多表连接
来源：http://zy.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nb.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://sy.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://mg.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://dq.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://zh.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qv.newstarts.cn

[Q43] 标量子查询
来源：http://br.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fy.nicolike.cn

[Q44] IN 子查询
来源：http://ec.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zo.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://xt.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sd.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vx.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pl.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://vc.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pj.asd995.cn

[Q48] CTE 公用表表达式
来源：http://lx.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nm.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://nc.shxzukj.cn

[Q49] 更新单行
来源：http://fx.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gj.panjiajie.cn

[Q50] 批量更新
来源：http://yq.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uk.colortex.cn

[Q51] 用子查询更新
来源：http://im.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pr.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://qf.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://kk.szxytkj.cn

[Q53] 按条件删除
来源：http://cj.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ez.lnxyls.cn

[Q54] 清空表
来源：http://yk.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://cb.newstarts.cn

[Q55] 排名（并列占位）
来源：http://os.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wa.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://dx.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mr.hahajie.cn

[Q57] 行号
来源：http://wp.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vy.hahajie.cn

[Q58] 累计求和
来源：http://yu.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qb.hnjuh.cn

[Q59] 分组内累计
来源：http://dj.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://op.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://jq.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pq.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qc.nicolike.cn

[Q61] 移动平均
来源：http://le.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sf.muxihuayi.cn

[Q62] 分组占比
来源：http://tm.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tc.haigaiapp.cn

[Q63] 开启事务
来源：http://jk.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lc.bjjhwx.cn

[Q64] 提交事务
来源：http://gm.huanxung.cn

COMMIT;
来源：http://ao.panjiajie.cn

[Q65] 回滚事务
来源：http://dq.haigaiapp.cn

ROLLBACK;
来源：http://eg.nicolike.cn

[Q66] 行锁查询
来源：http://ua.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pl.gzmigu.cn

[Q67] 设置隔离级别
来源：http://xx.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lh.wgjwhj.cn

[Q68] 保存点
来源：http://wf.jctech888.com.cn

SAVEPOINT sp1;
来源：http://oi.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://eq.gzmigu.cn

[Q69] 查看执行计划
来源：http://ef.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://st.huanxung.cn

[Q70] 更新统计信息
来源：http://hm.newstarts.cn

ANALYZE TABLE users;
来源：http://jt.wgjwhj.cn

[Q71] 查看建表语句
来源：http://sm.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xd.huanxung.cn

[Q72] 查看索引
来源：http://yj.nszjky.cn

SHOW INDEX FROM users;
来源：http://gk.wgjwhj.cn

[Q73] 查看表状态
来源：http://pm.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xt.yuexingan06.cn

[Q74] 强制使用索引
来源：http://jo.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ee.521024.cn

[Q75] 日期格式化
来源：http://ji.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jp.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://np.newstarts.cn

[Q76] 按天统计
来源：http://if.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vd.nicolike.cn

[Q77] 时间加减
来源：http://mh.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bj.haigaiapp.cn

[Q78] 当前时间
来源：http://ir.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://el.hnjuh.cn

[Q79] 字符串拼接
来源：http://bs.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lb.hnjuh.cn

[Q80] 字符串截取
来源：http://er.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lo.shxzskj.cn

[Q81] 字符串替换
来源：http://ag.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ix.hnjuh.cn


<!-- 参考信息 -->
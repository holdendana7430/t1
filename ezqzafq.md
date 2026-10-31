代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qe.jctech888.com.cn

TS:   // 同 JS
来源：http://ut.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://sz.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://se.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uo.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://xe.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://ym.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://jo.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ht.hahajie.cn

JS:   async function f() { await g(); }
来源：http://br.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vf.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tm.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jo.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ys.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://hb.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://xg.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://rb.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uk.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://or.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://yd.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gq.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nr.hahajie.cn

Ruby: threads.map(&:join)
来源：http://mg.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rg.szsharing.cn

[O06] 使用进程池
来源：http://jc.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qh.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hp.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://he.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ub.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qk.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hk.hnjuh.cn

Ruby: // fork 块
来源：http://sn.panjiajie.cn

C#:   Parallel.For
来源：http://wa.shxzskj.cn

================================================================================
来源：http://jl.haigaiapp.cn

P. 常用工具函数
来源：http://nr.colortex.cn

================================================================================
来源：http://qs.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://wa.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://ea.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wj.9csxet.cn

JS:   crypto.randomUUID()
来源：http://eq.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://xo.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://jw.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://oc.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://tn.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://qj.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://ky.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ng.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bk.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hl.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ku.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://br.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tc.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bg.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nj.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://tu.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yb.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rh.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zo.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cw.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://np.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pm.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zv.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mh.nicolike.cn

[P04] 求长度
来源：http://hd.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tz.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rf.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sk.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wj.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://id.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://fh.szsharing.cn

Ruby: x.length;  x.size
来源：http://tz.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://de.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://yw.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://id.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qp.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://us.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ht.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fa.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ko.newstarts.cn

Ruby: a == b
来源：http://bv.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ge.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pu.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zz.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://xb.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pd.asd995.cn

TS:   if (x == null) {}
来源：http://mu.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ec.gzmigu.cn

Go:   if x == nil {}
来源：http://is.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xe.jctech888.com.cn

C#:   if (x is null) {}
来源：http://tm.asd995.cn

[P07] 防抖与节流
来源：http://pl.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xc.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://zc.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dt.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xf.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ol.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://li.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zh.huanxung.cn

[P08] 处理浮点精度问题
来源：http://qb.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ty.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wx.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rm.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ru.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pq.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://le.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://za.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://au.wgjwhj.cn

================================================================================
来源：http://xl.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mf.huixiangedu.cn

================================================================================
来源：http://qe.newstarts.cn

[Q01] 创建表
来源：http://eo.yuntaijiaju.cn

CREATE TABLE users (
来源：http://oo.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bv.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ay.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://su.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sw.bookmarksfly.cn

);
来源：http://xm.lnxyls.cn

[Q02] 创建带外键的表
来源：http://jk.shxzskj.cn

CREATE TABLE orders (
来源：http://jl.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ja.521024.cn

user_id INT NOT NULL,
来源：http://hy.hahajie.cn

amount DECIMAL(10, 2),
来源：http://la.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wt.nicolike.cn

);
来源：http://xm.hahajie.cn

[Q03] 增加列
来源：http://lk.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pd.muxihuayi.cn

[Q04] 修改列类型
来源：http://sx.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eh.haigaiapp.cn

[Q05] 重命名列
来源：http://oz.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://en.huixiangedu.cn

[Q06] 删除列
来源：http://yc.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aj.jctech888.com.cn

[Q07] 删除表
来源：http://vz.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://xy.shtwfgs.cn

[Q08] 创建普通索引
来源：http://eu.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gx.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://yh.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dm.nszjky.cn

[Q10] 插入单行
来源：http://ev.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mx.nszjky.cn

[Q11] 一次插入多行
来源：http://eq.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wf.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://nq.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ij.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ho.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://lf.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tc.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://jf.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hu.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tr.szxytkj.cn

[Q15] 查询全部
来源：http://xu.haigaiapp.cn

SELECT * FROM users;
来源：http://fz.huanxung.cn

[Q16] 查询指定列
来源：http://hz.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://sr.muxihuayi.cn

[Q17] 条件查询
来源：http://rv.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ex.nszjky.cn

[Q18] 模糊匹配
来源：http://cs.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bx.yuntaijiaju.cn

[Q19] 范围查询
来源：http://sl.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iq.szxytkj.cn

[Q20] IN 列表
来源：http://iv.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bw.yuntaijiaju.cn

[Q21] 空值判断
来源：http://xr.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pp.yuntaijiaju.cn

[Q22] 排序
来源：http://pb.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fy.szsharing.cn

[Q23] 分页
来源：http://il.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lp.wgjwhj.cn

[Q24] 去重
来源：http://ry.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://ky.hnjuh.cn

[Q25] 只取前 N 条
来源：http://ri.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://it.yuntaijiaju.cn

[Q26] 计数
来源：http://oq.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://qn.nicolike.cn

[Q27] 条件计数
来源：http://jr.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://js.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://wh.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xm.nicolike.cn

[Q29] 最大最小值
来源：http://dd.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nv.hnjuh.cn

[Q30] 分组统计
来源：http://bf.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dc.hnjuh.cn

[Q31] 分组后过滤
来源：http://jq.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ud.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://xr.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mt.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ig.yuexingan06.cn

[Q33] 多列分组
来源：http://vq.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rn.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://qs.shxzukj.cn

SELECT * FROM (
来源：http://fl.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mk.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://jp.yuntaijiaju.cn

[Q35] 内连接
来源：http://vf.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wo.yuexingan06.cn

[Q36] 左连接
来源：http://th.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://in.huixinmuqiang.cn

[Q37] 右连接
来源：http://bv.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xq.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yo.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cq.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://ag.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cz.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kp.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rr.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://he.hahajie.cn

[Q41] 多表连接
来源：http://vs.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fs.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://kb.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://yv.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://pa.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://xu.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vq.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://pp.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ph.9csxet.cn

[Q44] IN 子查询
来源：http://fi.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fd.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://cl.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nd.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://em.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sz.shtwfgs.cn

[Q47] 与平均值比较
来源：http://yy.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pj.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://ys.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vt.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://jq.asd995.cn

[Q49] 更新单行
来源：http://cp.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ui.yuntaijiaju.cn

[Q50] 批量更新
来源：http://me.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dn.hnjuh.cn

[Q51] 用子查询更新
来源：http://bv.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bh.wgjwhj.cn

[Q52] 删除指定行
来源：http://cc.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://xk.muxihuayi.cn

[Q53] 按条件删除
来源：http://tq.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://in.huixiangedu.cn

[Q54] 清空表
来源：http://dt.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://uw.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://sx.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sr.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://jo.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://df.colortex.cn

[Q57] 行号
来源：http://fw.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tt.jianghongdianzi.cn

[Q58] 累计求和
来源：http://jw.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jo.shtwfgs.cn

[Q59] 分组内累计
来源：http://mf.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fj.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://pw.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hi.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fh.newstarts.cn

[Q61] 移动平均
来源：http://rs.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ds.szsharing.cn

[Q62] 分组占比
来源：http://nw.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ms.muxihuayi.cn

[Q63] 开启事务
来源：http://va.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xx.haigaiapp.cn

[Q64] 提交事务
来源：http://ze.asd995.cn

COMMIT;
来源：http://ky.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://os.hahajie.cn

ROLLBACK;
来源：http://bs.shxzukj.cn

[Q66] 行锁查询
来源：http://xm.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ic.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://hc.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.nicolike.cn

[Q68] 保存点
来源：http://fi.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://wr.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://wv.521024.cn

[Q69] 查看执行计划
来源：http://tt.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://al.huixiangedu.cn

[Q70] 更新统计信息
来源：http://my.newstarts.cn

ANALYZE TABLE users;
来源：http://lv.bjjhwx.cn

[Q71] 查看建表语句
来源：http://fa.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mk.shtwfgs.cn

[Q72] 查看索引
来源：http://dd.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://pn.shxzskj.cn

[Q73] 查看表状态
来源：http://fd.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lr.gzmigu.cn

[Q74] 强制使用索引
来源：http://fx.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://px.521024.cn

[Q75] 日期格式化
来源：http://wk.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gy.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zt.jianghongdianzi.cn

[Q76] 按天统计
来源：http://tz.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ka.wgjwhj.cn

[Q77] 时间加减
来源：http://eu.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fl.jianghongdianzi.cn

[Q78] 当前时间
来源：http://fc.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zj.shxzukj.cn

[Q79] 字符串拼接
来源：http://vh.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://el.gzmigu.cn

[Q80] 字符串截取
来源：http://bn.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hb.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://ex.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cw.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://rn.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jt.gzmigu.cn

[Q83] 大小写转换
来源：http://wj.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pk.9csxet.cn


<!-- 参考信息 -->
代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ud.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://is.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://ao.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://tt.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://wd.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uj.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://po.asd995.cn

TS:   await Promise.all(tasks)
来源：http://zp.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gh.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rh.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://md.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kn.huixinmuqiang.cn

[O06] 使用进程池
来源：http://gk.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://du.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ik.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://ts.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://ak.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zg.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oh.nicolike.cn

Ruby: // fork 块
来源：http://um.shxzskj.cn

C#:   Parallel.For
来源：http://ll.szsharing.cn

================================================================================
来源：http://fj.jianghongdianzi.cn

P. 常用工具函数
来源：http://kj.bjjhwx.cn

================================================================================
来源：http://qa.szsharing.cn

[P01] 生成 UUID
来源：http://ub.521024.cn

Py:   str(uuid.uuid4())
来源：http://tu.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://th.newstarts.cn

JS:   crypto.randomUUID()
来源：http://zm.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://ei.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://op.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://qu.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://qd.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ox.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://dy.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zg.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ib.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sw.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yd.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ax.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ln.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yv.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fi.newstarts.cn

[P03] 生成短随机字符串
来源：http://da.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bh.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://up.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://au.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qy.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hx.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pl.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zu.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ds.szsharing.cn

[P04] 求长度
来源：http://af.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ut.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ne.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ze.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nr.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://rq.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://mv.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://bv.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lj.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ed.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zd.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iy.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://da.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kr.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zv.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ug.huixiangedu.cn

Ruby: a == b
来源：http://is.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gu.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ia.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aq.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://il.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mp.nicolike.cn

TS:   if (x == null) {}
来源：http://uq.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ir.asd995.cn

Go:   if x == nil {}
来源：http://ld.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xa.521024.cn

C#:   if (x is null) {}
来源：http://ph.shxzskj.cn

[P07] 防抖与节流
来源：http://pp.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mt.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://dd.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ns.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yo.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mx.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ia.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qy.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fl.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://ob.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qg.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xh.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xk.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ow.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://he.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gz.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xk.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wu.gzmigu.cn

================================================================================
来源：http://na.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fl.colortex.cn

================================================================================
来源：http://ia.shxzukj.cn

[Q01] 创建表
来源：http://da.shtwfgs.cn

CREATE TABLE users (
来源：http://mj.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xi.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://bq.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://qp.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bm.jianghongdianzi.cn

);
来源：http://qm.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://bj.lnxyls.cn

CREATE TABLE orders (
来源：http://me.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qp.lnxyls.cn

user_id INT NOT NULL,
来源：http://oo.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://oj.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zv.hnjuh.cn

);
来源：http://pn.szsharing.cn

[Q03] 增加列
来源：http://wo.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hd.lnxyls.cn

[Q04] 修改列类型
来源：http://gw.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qo.nicolike.cn

[Q05] 重命名列
来源：http://rq.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yo.hnjuh.cn

[Q06] 删除列
来源：http://am.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nz.szxytkj.cn

[Q07] 删除表
来源：http://mr.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://oc.muxihuayi.cn

[Q08] 创建普通索引
来源：http://ip.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pl.lnxyls.cn

[Q09] 创建唯一索引
来源：http://dh.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xo.9csxet.cn

[Q10] 插入单行
来源：http://fp.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ru.yuexingan06.cn

[Q11] 一次插入多行
来源：http://kl.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cl.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://wk.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zb.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ws.newstarts.cn

[Q13] 忽略重复插入
来源：http://fe.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pf.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://aq.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rh.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qh.hahajie.cn

[Q15] 查询全部
来源：http://vf.nicolike.cn

SELECT * FROM users;
来源：http://mj.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://jq.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://vi.hnjuh.cn

[Q17] 条件查询
来源：http://pi.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zj.panjiajie.cn

[Q18] 模糊匹配
来源：http://da.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dc.bookmarksfly.cn

[Q19] 范围查询
来源：http://nr.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yt.bjjhwx.cn

[Q20] IN 列表
来源：http://mv.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xz.muxihuayi.cn

[Q21] 空值判断
来源：http://kc.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xj.colortex.cn

[Q22] 排序
来源：http://jk.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://la.shxzukj.cn

[Q23] 分页
来源：http://vh.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vg.lnxyls.cn

[Q24] 去重
来源：http://kq.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://mz.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://fx.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zk.wgjwhj.cn

[Q26] 计数
来源：http://to.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://ml.huixiangedu.cn

[Q27] 条件计数
来源：http://jc.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fb.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://ay.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zn.bookmarksfly.cn

[Q29] 最大最小值
来源：http://gl.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sv.bjjhwx.cn

[Q30] 分组统计
来源：http://sp.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ls.colortex.cn

[Q31] 分组后过滤
来源：http://ae.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hq.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://cw.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hn.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pr.chemitech.net.cn

[Q33] 多列分组
来源：http://ue.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tt.gzmigu.cn

[Q34] 每组取第一条
来源：http://mw.wgjwhj.cn

SELECT * FROM (
来源：http://gh.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wl.newstarts.cn

) t WHERE rn = 1;
来源：http://gq.shxzskj.cn

[Q35] 内连接
来源：http://dx.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wz.nszjky.cn

[Q36] 左连接
来源：http://ms.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gs.yuntaijiaju.cn

[Q37] 右连接
来源：http://rz.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qd.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dq.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tn.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://zu.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xq.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jz.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ca.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ca.huanxung.cn

[Q41] 多表连接
来源：http://zg.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wf.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://dh.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://yq.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://qa.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://dx.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nl.shtwfgs.cn

[Q43] 标量子查询
来源：http://ba.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://my.newstarts.cn

[Q44] IN 子查询
来源：http://fi.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hk.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://oq.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cb.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ru.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dt.muxihuayi.cn

[Q47] 与平均值比较
来源：http://sx.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kg.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ds.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wr.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://rp.yuexingan06.cn

[Q49] 更新单行
来源：http://vt.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vt.9csxet.cn

[Q50] 批量更新
来源：http://qv.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pk.shtwfgs.cn

[Q51] 用子查询更新
来源：http://za.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fl.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://ep.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://zd.hnjuh.cn

[Q53] 按条件删除
来源：http://ol.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://me.9csxet.cn

[Q54] 清空表
来源：http://ij.colortex.cn

TRUNCATE TABLE logs;
来源：http://ql.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://jz.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sq.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://sv.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pr.szsharing.cn

[Q57] 行号
来源：http://id.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kp.chemitech.net.cn

[Q58] 累计求和
来源：http://sb.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vz.jctech888.com.cn

[Q59] 分组内累计
来源：http://my.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zr.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://nh.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xy.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qq.wgjwhj.cn

[Q61] 移动平均
来源：http://fj.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hj.jianghongdianzi.cn

[Q62] 分组占比
来源：http://jx.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dp.szxytkj.cn

[Q63] 开启事务
来源：http://md.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qz.chemitech.net.cn

[Q64] 提交事务
来源：http://ot.yuexingan06.cn

COMMIT;
来源：http://vx.huanxung.cn

[Q65] 回滚事务
来源：http://jq.huixinmuqiang.cn

ROLLBACK;
来源：http://bk.nicolike.cn

[Q66] 行锁查询
来源：http://vr.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jk.huanxung.cn

[Q67] 设置隔离级别
来源：http://mc.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ic.colortex.cn

[Q68] 保存点
来源：http://wu.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://ew.9csxet.cn

ROLLBACK TO sp1;
来源：http://xv.newstarts.cn

[Q69] 查看执行计划
来源：http://gi.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gp.huixiangedu.cn

[Q70] 更新统计信息
来源：http://ls.szxytkj.cn

ANALYZE TABLE users;
来源：http://cf.9csxet.cn

[Q71] 查看建表语句
来源：http://xt.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lb.gzmigu.cn

[Q72] 查看索引
来源：http://mh.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://rd.wgjwhj.cn

[Q73] 查看表状态
来源：http://wm.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uq.shxzukj.cn

[Q74] 强制使用索引
来源：http://sg.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ql.bookmarksfly.cn

[Q75] 日期格式化
来源：http://tc.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dc.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qr.nszjky.cn

[Q76] 按天统计
来源：http://fw.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jk.colortex.cn

[Q77] 时间加减
来源：http://bd.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cf.nszjky.cn

[Q78] 当前时间
来源：http://wn.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jl.haigaiapp.cn

[Q79] 字符串拼接
来源：http://hr.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mv.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://fy.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rt.nicolike.cn

[Q81] 字符串替换
来源：http://gg.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ux.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://vd.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rl.bookmarksfly.cn

[Q83] 大小写转换
来源：http://mh.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://au.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://om.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://sn.szxytkj.cn

[Q85] 数值取整
来源：http://id.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bt.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://xy.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ht.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://fb.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cn.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://ku.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mp.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zw.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://dn.colortex.cn


<!-- 参考信息 -->
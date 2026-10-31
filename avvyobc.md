代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://qc.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xq.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://sz.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://nz.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sc.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fw.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://yk.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xs.nicolike.cn

[O06] 使用进程池
来源：http://tv.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ef.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ue.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://of.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://da.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ei.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kt.shxzukj.cn

Ruby: // fork 块
来源：http://pn.shxzukj.cn

C#:   Parallel.For
来源：http://zg.9csxet.cn

================================================================================
来源：http://fy.jctech888.com.cn

P. 常用工具函数
来源：http://ly.hnjuh.cn

================================================================================
来源：http://nm.shxzukj.cn

[P01] 生成 UUID
来源：http://zk.asd995.cn

Py:   str(uuid.uuid4())
来源：http://gq.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ns.huanxung.cn

JS:   crypto.randomUUID()
来源：http://bj.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://rd.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://mh.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://kv.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://cl.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://bx.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://ot.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zs.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fn.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ee.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jo.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qo.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ru.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bn.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gt.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://yk.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gs.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ps.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lr.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mw.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jm.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kz.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iy.shxzukj.cn

[P04] 求长度
来源：http://rp.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fb.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ve.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bv.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sl.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://ie.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://wg.nszjky.cn

Ruby: x.length;  x.size
来源：http://jp.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gk.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://nq.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cy.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gj.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ch.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rf.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zb.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://od.9csxet.cn

Ruby: a == b
来源：http://kt.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yc.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hi.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://im.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://mw.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xo.nicolike.cn

TS:   if (x == null) {}
来源：http://wv.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gb.chemitech.net.cn

Go:   if x == nil {}
来源：http://il.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hm.bjjhwx.cn

C#:   if (x is null) {}
来源：http://fp.hnjuh.cn

[P07] 防抖与节流
来源：http://hi.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cq.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://fb.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fu.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oz.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nx.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://im.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ud.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://ba.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xp.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mh.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pe.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ee.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qe.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ct.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zf.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hg.yuntaijiaju.cn

================================================================================
来源：http://eg.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gg.colortex.cn

================================================================================
来源：http://qe.bookmarksfly.cn

[Q01] 创建表
来源：http://eb.jctech888.com.cn

CREATE TABLE users (
来源：http://kf.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bg.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://el.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://qt.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yv.panjiajie.cn

);
来源：http://hh.szsharing.cn

[Q02] 创建带外键的表
来源：http://fd.nszjky.cn

CREATE TABLE orders (
来源：http://ek.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xf.huixiangedu.cn

user_id INT NOT NULL,
来源：http://pv.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://dx.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pr.asd995.cn

);
来源：http://lv.lnxyls.cn

[Q03] 增加列
来源：http://nd.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ke.hnjuh.cn

[Q04] 修改列类型
来源：http://ng.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uz.jctech888.com.cn

[Q05] 重命名列
来源：http://qd.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oj.shxzukj.cn

[Q06] 删除列
来源：http://zt.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ab.nicolike.cn

[Q07] 删除表
来源：http://ut.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://su.szxytkj.cn

[Q08] 创建普通索引
来源：http://hs.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ku.9csxet.cn

[Q09] 创建唯一索引
来源：http://mq.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qn.hahajie.cn

[Q10] 插入单行
来源：http://ge.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fg.shtwfgs.cn

[Q11] 一次插入多行
来源：http://bd.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lt.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://uz.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tx.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nd.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://nr.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ux.521024.cn

[Q14] 存在则更新（upsert）
来源：http://wj.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://be.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pp.szsharing.cn

[Q15] 查询全部
来源：http://oe.bookmarksfly.cn

SELECT * FROM users;
来源：http://qp.nicolike.cn

[Q16] 查询指定列
来源：http://ru.asd995.cn

SELECT id, name FROM users;
来源：http://gt.hahajie.cn

[Q17] 条件查询
来源：http://uo.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ga.szxytkj.cn

[Q18] 模糊匹配
来源：http://vr.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pm.newstarts.cn

[Q19] 范围查询
来源：http://te.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mb.nicolike.cn

[Q20] IN 列表
来源：http://ty.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hl.hnjuh.cn

[Q21] 空值判断
来源：http://uq.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pg.panjiajie.cn

[Q22] 排序
来源：http://pz.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sm.nicolike.cn

[Q23] 分页
来源：http://dy.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://am.hnjuh.cn

[Q24] 去重
来源：http://xa.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://pz.lnxyls.cn

[Q25] 只取前 N 条
来源：http://bq.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vj.nszjky.cn

[Q26] 计数
来源：http://lu.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://cb.shtwfgs.cn

[Q27] 条件计数
来源：http://ba.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ij.wgjwhj.cn

[Q28] 求和与平均
来源：http://cq.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zl.521024.cn

[Q29] 最大最小值
来源：http://rt.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fa.newstarts.cn

[Q30] 分组统计
来源：http://ke.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zp.bjjhwx.cn

[Q31] 分组后过滤
来源：http://by.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dr.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://fh.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://in.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ae.yuntaijiaju.cn

[Q33] 多列分组
来源：http://sv.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fp.colortex.cn

[Q34] 每组取第一条
来源：http://ry.shtwfgs.cn

SELECT * FROM (
来源：http://ft.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://um.newstarts.cn

) t WHERE rn = 1;
来源：http://yy.521024.cn

[Q35] 内连接
来源：http://xu.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://va.haigaiapp.cn

[Q36] 左连接
来源：http://yg.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://um.jianghongdianzi.cn

[Q37] 右连接
来源：http://qu.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wj.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cp.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ds.521024.cn

[Q39] 自连接（查上下级）
来源：http://pd.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qj.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hc.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zi.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zi.lnxyls.cn

[Q41] 多表连接
来源：http://xy.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://db.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://hv.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://bt.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://wx.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://gu.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jr.hnjuh.cn

[Q43] 标量子查询
来源：http://tr.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uq.shxzskj.cn

[Q44] IN 子查询
来源：http://qz.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zc.521024.cn

[Q45] EXISTS 判断存在
来源：http://kk.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gs.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fo.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kv.hahajie.cn

[Q47] 与平均值比较
来源：http://gc.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ox.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://wc.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gf.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://yx.huixinmuqiang.cn

[Q49] 更新单行
来源：http://ir.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ts.szxytkj.cn

[Q50] 批量更新
来源：http://zg.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kl.wgjwhj.cn

[Q51] 用子查询更新
来源：http://on.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xr.gzmigu.cn

[Q52] 删除指定行
来源：http://cs.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://kp.newstarts.cn

[Q53] 按条件删除
来源：http://ad.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yl.huanxung.cn

[Q54] 清空表
来源：http://nm.9csxet.cn

TRUNCATE TABLE logs;
来源：http://ej.colortex.cn

[Q55] 排名（并列占位）
来源：http://yd.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hm.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://tk.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bd.shxzskj.cn

[Q57] 行号
来源：http://hi.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ll.hnjuh.cn

[Q58] 累计求和
来源：http://bh.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fh.nicolike.cn

[Q59] 分组内累计
来源：http://lb.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lq.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://xz.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hf.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cz.szsharing.cn

[Q61] 移动平均
来源：http://cj.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qf.jctech888.com.cn

[Q62] 分组占比
来源：http://yz.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tz.huixinmuqiang.cn

[Q63] 开启事务
来源：http://ce.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qn.yuexingan06.cn

[Q64] 提交事务
来源：http://gx.wgjwhj.cn

COMMIT;
来源：http://tt.jctech888.com.cn

[Q65] 回滚事务
来源：http://uy.shtwfgs.cn

ROLLBACK;
来源：http://ay.muxihuayi.cn

[Q66] 行锁查询
来源：http://cw.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vc.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://nq.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vl.wgjwhj.cn

[Q68] 保存点
来源：http://ww.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://he.panjiajie.cn

ROLLBACK TO sp1;
来源：http://xh.bjjhwx.cn

[Q69] 查看执行计划
来源：http://ya.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ms.nicolike.cn

[Q70] 更新统计信息
来源：http://py.yuexingan06.cn

ANALYZE TABLE users;
来源：http://mt.szxytkj.cn

[Q71] 查看建表语句
来源：http://dj.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bz.asd995.cn

[Q72] 查看索引
来源：http://tv.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://lq.9csxet.cn

[Q73] 查看表状态
来源：http://kv.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oi.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ok.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wl.jctech888.com.cn

[Q75] 日期格式化
来源：http://gj.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sx.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wj.wgjwhj.cn

[Q76] 按天统计
来源：http://zy.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://up.hahajie.cn

[Q77] 时间加减
来源：http://cs.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ey.jianghongdianzi.cn

[Q78] 当前时间
来源：http://qm.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ep.panjiajie.cn

[Q79] 字符串拼接
来源：http://bx.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xc.lnxyls.cn

[Q80] 字符串截取
来源：http://dl.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zc.haigaiapp.cn

[Q81] 字符串替换
来源：http://fo.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wc.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://vl.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zw.hnjuh.cn

[Q83] 大小写转换
来源：http://xn.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wl.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://jp.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://tz.shtwfgs.cn

[Q85] 数值取整
来源：http://ei.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://di.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://wc.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eb.newstarts.cn

[Q87] JSON 字段做条件
来源：http://al.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gj.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://nc.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aw.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yz.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://bh.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gx.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://im.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rb.hnjuh.cn

================================================================================
来源：http://hg.wgjwhj.cn


<!-- 参考信息 -->
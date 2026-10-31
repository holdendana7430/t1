代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gu.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hj.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://yd.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ss.hnjuh.cn

[O06] 使用进程池
来源：http://tb.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sh.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mk.521024.cn

JS:   // child_process / cluster 模块
来源：http://id.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://bo.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fj.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hj.lnxyls.cn

Ruby: // fork 块
来源：http://qa.lnxyls.cn

C#:   Parallel.For
来源：http://wl.yuexingan06.cn

================================================================================
来源：http://oi.shtwfgs.cn

P. 常用工具函数
来源：http://to.asd995.cn

================================================================================
来源：http://sz.szsharing.cn

[P01] 生成 UUID
来源：http://vg.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://yn.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oc.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://et.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://ti.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://qw.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ha.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://nn.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://aj.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://ow.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tb.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kd.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zw.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mk.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sz.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nn.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xb.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yf.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://zz.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bl.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rv.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yh.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://av.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mq.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bb.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://si.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pd.shxzukj.cn

[P04] 求长度
来源：http://dx.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mk.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lg.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ep.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bz.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://vn.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://rh.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://to.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ch.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://bs.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zd.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fl.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sp.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://er.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ak.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://my.muxihuayi.cn

Ruby: a == b
来源：http://um.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xm.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qa.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zo.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://bi.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wl.shxzskj.cn

TS:   if (x == null) {}
来源：http://iv.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ck.colortex.cn

Go:   if x == nil {}
来源：http://uh.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uo.szxytkj.cn

C#:   if (x is null) {}
来源：http://if.shtwfgs.cn

[P07] 防抖与节流
来源：http://oo.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hi.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://hj.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kn.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oo.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ib.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rb.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ub.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://wb.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hi.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ka.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sk.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xb.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tq.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://og.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qy.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tr.521024.cn

================================================================================
来源：http://tv.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fh.newstarts.cn

================================================================================
来源：http://tl.muxihuayi.cn

[Q01] 创建表
来源：http://gx.bookmarksfly.cn

CREATE TABLE users (
来源：http://gm.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vt.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://mm.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://nk.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oz.muxihuayi.cn

);
来源：http://ra.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://nf.muxihuayi.cn

CREATE TABLE orders (
来源：http://pd.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://th.nicolike.cn

user_id INT NOT NULL,
来源：http://hf.colortex.cn

amount DECIMAL(10, 2),
来源：http://db.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://av.muxihuayi.cn

);
来源：http://oc.bookmarksfly.cn

[Q03] 增加列
来源：http://ro.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cf.9csxet.cn

[Q04] 修改列类型
来源：http://pl.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ce.yuntaijiaju.cn

[Q05] 重命名列
来源：http://jm.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cw.jctech888.com.cn

[Q06] 删除列
来源：http://cs.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://se.bookmarksfly.cn

[Q07] 删除表
来源：http://uo.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://fw.wgjwhj.cn

[Q08] 创建普通索引
来源：http://kc.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cn.panjiajie.cn

[Q09] 创建唯一索引
来源：http://xg.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gx.haigaiapp.cn

[Q10] 插入单行
来源：http://kk.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nk.lnxyls.cn

[Q11] 一次插入多行
来源：http://pn.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yv.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://rq.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rw.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ot.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://tu.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lv.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://xw.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bc.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://af.hahajie.cn

[Q15] 查询全部
来源：http://qx.haigaiapp.cn

SELECT * FROM users;
来源：http://vb.asd995.cn

[Q16] 查询指定列
来源：http://fg.shtwfgs.cn

SELECT id, name FROM users;
来源：http://bk.colortex.cn

[Q17] 条件查询
来源：http://qi.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vr.hahajie.cn

[Q18] 模糊匹配
来源：http://jv.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wb.szxytkj.cn

[Q19] 范围查询
来源：http://wg.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ii.hnjuh.cn

[Q20] IN 列表
来源：http://jq.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mx.gzmigu.cn

[Q21] 空值判断
来源：http://zb.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pg.yuexingan06.cn

[Q22] 排序
来源：http://ej.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ne.wgjwhj.cn

[Q23] 分页
来源：http://sr.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jk.yuexingan06.cn

[Q24] 去重
来源：http://nv.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://ys.hnjuh.cn

[Q25] 只取前 N 条
来源：http://us.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://im.shtwfgs.cn

[Q26] 计数
来源：http://kl.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://ms.lnxyls.cn

[Q27] 条件计数
来源：http://fp.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bw.yuexingan06.cn

[Q28] 求和与平均
来源：http://iy.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://im.haigaiapp.cn

[Q29] 最大最小值
来源：http://xp.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://st.jctech888.com.cn

[Q30] 分组统计
来源：http://gl.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nd.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://wu.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nx.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://zg.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mw.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bo.bookmarksfly.cn

[Q33] 多列分组
来源：http://ri.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kx.nszjky.cn

[Q34] 每组取第一条
来源：http://tg.shxzskj.cn

SELECT * FROM (
来源：http://ru.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bu.shtwfgs.cn

) t WHERE rn = 1;
来源：http://oi.nicolike.cn

[Q35] 内连接
来源：http://nn.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://or.jianghongdianzi.cn

[Q36] 左连接
来源：http://hg.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cp.szxytkj.cn

[Q37] 右连接
来源：http://ou.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ty.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ua.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jo.colortex.cn

[Q39] 自连接（查上下级）
来源：http://lh.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ag.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iw.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zu.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uk.szxytkj.cn

[Q41] 多表连接
来源：http://vr.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xk.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ke.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://xe.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://gu.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://wz.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wx.hnjuh.cn

[Q43] 标量子查询
来源：http://bh.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qe.szxytkj.cn

[Q44] IN 子查询
来源：http://dw.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tu.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://en.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kz.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://go.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ok.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://xj.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://to.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ps.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rx.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://kk.bookmarksfly.cn

[Q49] 更新单行
来源：http://ou.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mu.szxytkj.cn

[Q50] 批量更新
来源：http://ys.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aw.nicolike.cn

[Q51] 用子查询更新
来源：http://wl.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cr.huanxung.cn

[Q52] 删除指定行
来源：http://qa.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://oz.haigaiapp.cn

[Q53] 按条件删除
来源：http://lm.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ji.521024.cn

[Q54] 清空表
来源：http://pa.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://wt.nicolike.cn

[Q55] 排名（并列占位）
来源：http://ry.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qa.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://ut.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vg.521024.cn

[Q57] 行号
来源：http://rg.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mc.shtwfgs.cn

[Q58] 累计求和
来源：http://gq.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qa.nicolike.cn

[Q59] 分组内累计
来源：http://ty.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jc.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://wm.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ac.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zx.hahajie.cn

[Q61] 移动平均
来源：http://rn.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://is.muxihuayi.cn

[Q62] 分组占比
来源：http://zm.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://db.lnxyls.cn

[Q63] 开启事务
来源：http://si.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ix.panjiajie.cn

[Q64] 提交事务
来源：http://ek.wgjwhj.cn

COMMIT;
来源：http://tu.colortex.cn

[Q65] 回滚事务
来源：http://ir.yuexingan06.cn

ROLLBACK;
来源：http://gk.szxytkj.cn

[Q66] 行锁查询
来源：http://sr.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kn.gzmigu.cn

[Q67] 设置隔离级别
来源：http://oz.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fy.wgjwhj.cn

[Q68] 保存点
来源：http://ht.hahajie.cn

SAVEPOINT sp1;
来源：http://dh.shxzukj.cn

ROLLBACK TO sp1;
来源：http://ao.shtwfgs.cn

[Q69] 查看执行计划
来源：http://jd.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ws.shxzukj.cn

[Q70] 更新统计信息
来源：http://ii.colortex.cn

ANALYZE TABLE users;
来源：http://me.gzmigu.cn

[Q71] 查看建表语句
来源：http://gv.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mf.yuexingan06.cn

[Q72] 查看索引
来源：http://dv.9csxet.cn

SHOW INDEX FROM users;
来源：http://tl.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://yp.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ud.shtwfgs.cn

[Q74] 强制使用索引
来源：http://dp.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oq.huanxung.cn

[Q75] 日期格式化
来源：http://yh.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wp.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gs.shxzskj.cn

[Q76] 按天统计
来源：http://dt.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vf.szxytkj.cn

[Q77] 时间加减
来源：http://gb.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mz.bjjhwx.cn

[Q78] 当前时间
来源：http://bo.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yt.wgjwhj.cn

[Q79] 字符串拼接
来源：http://ll.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oj.newstarts.cn

[Q80] 字符串截取
来源：http://iw.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ih.hnjuh.cn

[Q81] 字符串替换
来源：http://ig.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tj.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://mn.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ul.bjjhwx.cn

[Q83] 大小写转换
来源：http://ph.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lm.shxzskj.cn

[Q84] 去除首尾空格
来源：http://da.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://wk.yuntaijiaju.cn

[Q85] 数值取整
来源：http://nd.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ml.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://qr.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fq.huanxung.cn

[Q87] JSON 字段做条件
来源：http://oy.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qm.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://km.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lb.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nj.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://zq.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oy.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://dc.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://of.huixiangedu.cn

================================================================================
来源：http://jc.haigaiapp.cn

R. Bash 专题
来源：http://at.szxytkj.cn

================================================================================
来源：http://iw.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://xo.huanxung.cn

#!/usr/bin/env bash
来源：http://vc.jianghongdianzi.cn


<!-- 参考信息 -->
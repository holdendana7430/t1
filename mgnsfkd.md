代发 wailian999

[O06] 使用进程池
来源：http://qu.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kw.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qe.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://wt.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://ne.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://um.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ah.9csxet.cn

Ruby: // fork 块
来源：http://wj.nszjky.cn

C#:   Parallel.For
来源：http://od.shxzukj.cn

================================================================================
来源：http://pq.chemitech.net.cn

P. 常用工具函数
来源：http://jf.newstarts.cn

================================================================================
来源：http://vw.colortex.cn

[P01] 生成 UUID
来源：http://nh.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://tc.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oy.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://sl.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://oh.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://cz.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://je.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://lr.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://pg.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://lq.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ei.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://us.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cc.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ll.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qm.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nb.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://id.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zm.shxzskj.cn

[P03] 生成短随机字符串
来源：http://pb.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cb.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zh.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://do.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://js.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sx.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://um.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ld.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nz.hahajie.cn

[P04] 求长度
来源：http://io.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jb.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nj.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ze.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ns.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://gg.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://zn.521024.cn

Ruby: x.length;  x.size
来源：http://xp.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iz.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://ac.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wx.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bj.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lr.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jr.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://do.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fu.newstarts.cn

Ruby: a == b
来源：http://kx.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jk.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://le.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lb.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://cc.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://md.nicolike.cn

TS:   if (x == null) {}
来源：http://wq.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dx.yuexingan06.cn

Go:   if x == nil {}
来源：http://iz.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ai.yuexingan06.cn

C#:   if (x is null) {}
来源：http://qr.hahajie.cn

[P07] 防抖与节流
来源：http://mt.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vu.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://ks.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ud.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rb.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tk.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ri.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sk.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://he.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://te.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cx.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ma.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wh.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nd.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hb.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ap.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sd.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://si.jctech888.com.cn

================================================================================
来源：http://ae.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qs.huixiangedu.cn

================================================================================
来源：http://df.wgjwhj.cn

[Q01] 创建表
来源：http://us.hnjuh.cn

CREATE TABLE users (
来源：http://gb.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ro.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://es.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://hs.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fe.shtwfgs.cn

);
来源：http://rk.gzmigu.cn

[Q02] 创建带外键的表
来源：http://fd.hnjuh.cn

CREATE TABLE orders (
来源：http://yj.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rn.colortex.cn

user_id INT NOT NULL,
来源：http://sq.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://kb.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ic.jctech888.com.cn

);
来源：http://uv.newstarts.cn

[Q03] 增加列
来源：http://qi.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://as.asd995.cn

[Q04] 修改列类型
来源：http://fz.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tb.muxihuayi.cn

[Q05] 重命名列
来源：http://ns.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ao.jianghongdianzi.cn

[Q06] 删除列
来源：http://wh.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qe.huixinmuqiang.cn

[Q07] 删除表
来源：http://hq.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://es.colortex.cn

[Q08] 创建普通索引
来源：http://km.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sv.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://wb.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yn.asd995.cn

[Q10] 插入单行
来源：http://gg.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sw.huanxung.cn

[Q11] 一次插入多行
来源：http://yz.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hk.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://eg.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://be.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mz.hnjuh.cn

[Q13] 忽略重复插入
来源：http://gm.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://du.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://wa.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ku.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nv.yuexingan06.cn

[Q15] 查询全部
来源：http://jt.shtwfgs.cn

SELECT * FROM users;
来源：http://wu.bookmarksfly.cn

[Q16] 查询指定列
来源：http://fm.newstarts.cn

SELECT id, name FROM users;
来源：http://ky.yuexingan06.cn

[Q17] 条件查询
来源：http://xs.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yt.huixiangedu.cn

[Q18] 模糊匹配
来源：http://ev.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rf.shxzskj.cn

[Q19] 范围查询
来源：http://pn.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yo.shxzukj.cn

[Q20] IN 列表
来源：http://je.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ka.wgjwhj.cn

[Q21] 空值判断
来源：http://bm.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wq.gzmigu.cn

[Q22] 排序
来源：http://mh.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eh.asd995.cn

[Q23] 分页
来源：http://px.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cn.muxihuayi.cn

[Q24] 去重
来源：http://be.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://ec.gzmigu.cn

[Q25] 只取前 N 条
来源：http://cv.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sm.shxzskj.cn

[Q26] 计数
来源：http://mf.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://km.szsharing.cn

[Q27] 条件计数
来源：http://lf.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uj.shxzskj.cn

[Q28] 求和与平均
来源：http://hs.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yt.shxzskj.cn

[Q29] 最大最小值
来源：http://ay.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lr.shtwfgs.cn

[Q30] 分组统计
来源：http://xi.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sd.nicolike.cn

[Q31] 分组后过滤
来源：http://bk.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xp.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://es.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gx.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ym.huanxung.cn

[Q33] 多列分组
来源：http://do.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mk.521024.cn

[Q34] 每组取第一条
来源：http://fz.bjjhwx.cn

SELECT * FROM (
来源：http://zw.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vg.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://uc.jianghongdianzi.cn

[Q35] 内连接
来源：http://ji.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ve.wgjwhj.cn

[Q36] 左连接
来源：http://io.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qi.huixinmuqiang.cn

[Q37] 右连接
来源：http://ks.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hu.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ky.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://px.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://fp.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vz.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://of.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yy.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hy.bjjhwx.cn

[Q41] 多表连接
来源：http://sf.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hq.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://te.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://fk.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://pm.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://xf.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://he.521024.cn

[Q43] 标量子查询
来源：http://ta.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vo.newstarts.cn

[Q44] IN 子查询
来源：http://on.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kk.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://ue.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nu.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ep.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://js.huixiangedu.cn

[Q47] 与平均值比较
来源：http://zd.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lf.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://fv.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hp.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://gt.hahajie.cn

[Q49] 更新单行
来源：http://bw.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yb.szsharing.cn

[Q50] 批量更新
来源：http://cs.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zu.colortex.cn

[Q51] 用子查询更新
来源：http://ny.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ia.szsharing.cn

[Q52] 删除指定行
来源：http://rv.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://ct.bookmarksfly.cn

[Q53] 按条件删除
来源：http://al.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kr.shxzukj.cn

[Q54] 清空表
来源：http://np.hahajie.cn

TRUNCATE TABLE logs;
来源：http://mq.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://rz.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tv.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://rd.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jp.jianghongdianzi.cn

[Q57] 行号
来源：http://ok.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gp.haigaiapp.cn

[Q58] 累计求和
来源：http://ch.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ma.shxzskj.cn

[Q59] 分组内累计
来源：http://hv.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mx.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://oy.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yq.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ur.hnjuh.cn

[Q61] 移动平均
来源：http://ts.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qg.muxihuayi.cn

[Q62] 分组占比
来源：http://tw.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://no.jianghongdianzi.cn

[Q63] 开启事务
来源：http://ee.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dn.huixiangedu.cn

[Q64] 提交事务
来源：http://tz.wgjwhj.cn

COMMIT;
来源：http://sm.bookmarksfly.cn

[Q65] 回滚事务
来源：http://dk.asd995.cn

ROLLBACK;
来源：http://xe.shxzskj.cn

[Q66] 行锁查询
来源：http://ej.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vv.shxzskj.cn

[Q67] 设置隔离级别
来源：http://ws.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://or.gzmigu.cn

[Q68] 保存点
来源：http://xm.muxihuayi.cn

SAVEPOINT sp1;
来源：http://vl.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://ae.panjiajie.cn

[Q69] 查看执行计划
来源：http://wn.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hr.szxytkj.cn

[Q70] 更新统计信息
来源：http://yd.szsharing.cn

ANALYZE TABLE users;
来源：http://sz.chemitech.net.cn

[Q71] 查看建表语句
来源：http://wh.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kf.shxzskj.cn

[Q72] 查看索引
来源：http://jg.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://jm.muxihuayi.cn

[Q73] 查看表状态
来源：http://mt.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://md.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://dc.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rn.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://lt.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dc.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sk.muxihuayi.cn

[Q76] 按天统计
来源：http://ld.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kz.colortex.cn

[Q77] 时间加减
来源：http://gq.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gd.521024.cn

[Q78] 当前时间
来源：http://zr.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jx.shxzskj.cn

[Q79] 字符串拼接
来源：http://bf.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hv.szxytkj.cn

[Q80] 字符串截取
来源：http://xw.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hm.chemitech.net.cn

[Q81] 字符串替换
来源：http://wz.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cq.colortex.cn

[Q82] 字符长度与字节长度
来源：http://gx.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sc.shxzskj.cn

[Q83] 大小写转换
来源：http://ny.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cm.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://dn.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://om.nszjky.cn

[Q85] 数值取整
来源：http://ca.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ep.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://wy.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://af.nszjky.cn

[Q87] JSON 字段做条件
来源：http://rj.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cm.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://ng.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://au.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nc.szxytkj.cn

[Q89] 判断表是否存在
来源：http://uw.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://or.asd995.cn

[Q90] 生成序号列
来源：http://ar.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vm.huanxung.cn

================================================================================
来源：http://jn.hahajie.cn

R. Bash 专题
来源：http://dy.newstarts.cn

================================================================================
来源：http://qz.huanxung.cn

[R01] shebang 与严格模式
来源：http://hr.hahajie.cn

#!/usr/bin/env bash
来源：http://ck.newstarts.cn

set -euo pipefail
来源：http://rc.asd995.cn

[R02] 变量赋值与使用
来源：http://sb.szxytkj.cn

name="Tom"; echo "$name"
来源：http://ov.muxihuayi.cn

[R03] 只读变量
来源：http://py.huanxung.cn


<!-- 参考信息 -->
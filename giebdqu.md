代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ar.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vp.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qh.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vt.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mi.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cx.521024.cn

[P03] 生成短随机字符串
来源：http://kg.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wo.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sm.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://up.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zg.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cb.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mg.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qf.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ex.jianghongdianzi.cn

[P04] 求长度
来源：http://ub.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://te.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qi.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rp.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dn.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://fr.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://tz.panjiajie.cn

Ruby: x.length;  x.size
来源：http://ri.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vp.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://ge.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yj.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pq.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mo.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bz.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dh.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://av.szsharing.cn

Ruby: a == b
来源：http://no.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ni.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vi.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hk.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://jv.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sw.jctech888.com.cn

TS:   if (x == null) {}
来源：http://vt.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jo.shxzskj.cn

Go:   if x == nil {}
来源：http://ct.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ud.huanxung.cn

C#:   if (x is null) {}
来源：http://hh.hahajie.cn

[P07] 防抖与节流
来源：http://yi.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xb.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ck.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fi.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hq.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iq.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yt.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gh.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lc.szsharing.cn

[P08] 处理浮点精度问题
来源：http://ho.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xb.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xu.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nh.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fy.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fv.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tk.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tj.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://my.shxzukj.cn

================================================================================
来源：http://kl.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://va.haigaiapp.cn

================================================================================
来源：http://ll.newstarts.cn

[Q01] 创建表
来源：http://or.wgjwhj.cn

CREATE TABLE users (
来源：http://vb.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xg.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://mh.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://bh.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vj.huixinmuqiang.cn

);
来源：http://zz.lnxyls.cn

[Q02] 创建带外键的表
来源：http://mn.colortex.cn

CREATE TABLE orders (
来源：http://bt.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qv.lnxyls.cn

user_id INT NOT NULL,
来源：http://oy.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://vn.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oz.shtwfgs.cn

);
来源：http://ni.hnjuh.cn

[Q03] 增加列
来源：http://fr.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tc.huixiangedu.cn

[Q04] 修改列类型
来源：http://nw.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uf.jctech888.com.cn

[Q05] 重命名列
来源：http://se.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ef.szsharing.cn

[Q06] 删除列
来源：http://au.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yn.nicolike.cn

[Q07] 删除表
来源：http://ci.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://hl.9csxet.cn

[Q08] 创建普通索引
来源：http://lz.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ju.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://lh.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kx.colortex.cn

[Q10] 插入单行
来源：http://xh.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qm.shxzskj.cn

[Q11] 一次插入多行
来源：http://lw.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bh.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://fe.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qj.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ut.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://ty.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://co.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://ea.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mz.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rz.muxihuayi.cn

[Q15] 查询全部
来源：http://tk.gzmigu.cn

SELECT * FROM users;
来源：http://dy.nicolike.cn

[Q16] 查询指定列
来源：http://xt.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://fg.jianghongdianzi.cn

[Q17] 条件查询
来源：http://js.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hf.521024.cn

[Q18] 模糊匹配
来源：http://ou.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fi.shxzukj.cn

[Q19] 范围查询
来源：http://qv.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://af.huixinmuqiang.cn

[Q20] IN 列表
来源：http://vo.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pk.bookmarksfly.cn

[Q21] 空值判断
来源：http://jm.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://on.wgjwhj.cn

[Q22] 排序
来源：http://qi.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xj.huixinmuqiang.cn

[Q23] 分页
来源：http://ph.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rp.yuexingan06.cn

[Q24] 去重
来源：http://gi.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://tc.colortex.cn

[Q25] 只取前 N 条
来源：http://du.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fl.panjiajie.cn

[Q26] 计数
来源：http://cg.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://ab.hahajie.cn

[Q27] 条件计数
来源：http://fx.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ut.gzmigu.cn

[Q28] 求和与平均
来源：http://pw.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ye.szsharing.cn

[Q29] 最大最小值
来源：http://sf.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qu.newstarts.cn

[Q30] 分组统计
来源：http://de.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bu.colortex.cn

[Q31] 分组后过滤
来源：http://hc.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ye.szsharing.cn

[Q32] 分组拼接字符串
来源：http://qr.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fj.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ef.panjiajie.cn

[Q33] 多列分组
来源：http://sr.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wu.yuexingan06.cn

[Q34] 每组取第一条
来源：http://yp.shxzukj.cn

SELECT * FROM (
来源：http://mz.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mp.521024.cn

) t WHERE rn = 1;
来源：http://zd.huixinmuqiang.cn

[Q35] 内连接
来源：http://yw.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xi.nszjky.cn

[Q36] 左连接
来源：http://mb.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://js.yuntaijiaju.cn

[Q37] 右连接
来源：http://tv.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ag.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sf.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jk.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://kq.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fr.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dx.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://we.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ol.panjiajie.cn

[Q41] 多表连接
来源：http://tn.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yy.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://he.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://an.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://kf.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://fo.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zv.bookmarksfly.cn

[Q43] 标量子查询
来源：http://es.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://he.hnjuh.cn

[Q44] IN 子查询
来源：http://iy.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hp.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://cq.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sa.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ce.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.nszjky.cn

[Q47] 与平均值比较
来源：http://rx.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rz.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://um.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vc.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://rb.huanxung.cn

[Q49] 更新单行
来源：http://gd.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rf.panjiajie.cn

[Q50] 批量更新
来源：http://kn.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tq.521024.cn

[Q51] 用子查询更新
来源：http://up.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wz.wgjwhj.cn

[Q52] 删除指定行
来源：http://lz.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://no.shxzukj.cn

[Q53] 按条件删除
来源：http://kr.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kw.gzmigu.cn

[Q54] 清空表
来源：http://uf.9csxet.cn

TRUNCATE TABLE logs;
来源：http://bi.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://zs.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iy.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://or.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tz.huanxung.cn

[Q57] 行号
来源：http://xb.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://em.muxihuayi.cn

[Q58] 累计求和
来源：http://mj.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ql.colortex.cn

[Q59] 分组内累计
来源：http://la.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ox.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://fg.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wd.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pu.shxzukj.cn

[Q61] 移动平均
来源：http://qy.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wh.newstarts.cn

[Q62] 分组占比
来源：http://cr.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cg.colortex.cn

[Q63] 开启事务
来源：http://zo.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ng.haigaiapp.cn

[Q64] 提交事务
来源：http://qw.haigaiapp.cn

COMMIT;
来源：http://mc.wgjwhj.cn

[Q65] 回滚事务
来源：http://ie.nszjky.cn

ROLLBACK;
来源：http://xg.wgjwhj.cn

[Q66] 行锁查询
来源：http://ts.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pa.9csxet.cn

[Q67] 设置隔离级别
来源：http://us.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cm.haigaiapp.cn

[Q68] 保存点
来源：http://pw.huanxung.cn

SAVEPOINT sp1;
来源：http://mx.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://kl.shtwfgs.cn

[Q69] 查看执行计划
来源：http://ch.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://py.szsharing.cn

[Q70] 更新统计信息
来源：http://so.nszjky.cn

ANALYZE TABLE users;
来源：http://mz.szxytkj.cn

[Q71] 查看建表语句
来源：http://fz.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://an.huixiangedu.cn

[Q72] 查看索引
来源：http://my.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://sd.haigaiapp.cn

[Q73] 查看表状态
来源：http://lx.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ss.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://mx.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ij.newstarts.cn

[Q75] 日期格式化
来源：http://lm.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vk.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qy.panjiajie.cn

[Q76] 按天统计
来源：http://rq.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fv.szxytkj.cn

[Q77] 时间加减
来源：http://ot.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mc.chemitech.net.cn

[Q78] 当前时间
来源：http://jj.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wh.jctech888.com.cn

[Q79] 字符串拼接
来源：http://cw.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mt.gzmigu.cn

[Q80] 字符串截取
来源：http://mz.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ga.huixiangedu.cn

[Q81] 字符串替换
来源：http://mt.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fe.colortex.cn

[Q82] 字符长度与字节长度
来源：http://wa.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ia.colortex.cn

[Q83] 大小写转换
来源：http://ik.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fg.shxzskj.cn

[Q84] 去除首尾空格
来源：http://rk.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://cz.newstarts.cn

[Q85] 数值取整
来源：http://lv.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zr.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://ez.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jo.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://mp.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kd.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://av.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bt.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://av.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://oj.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kh.lnxyls.cn

[Q90] 生成序号列
来源：http://oq.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://el.hnjuh.cn

================================================================================
来源：http://fw.yuntaijiaju.cn

R. Bash 专题
来源：http://wy.muxihuayi.cn

================================================================================
来源：http://hz.hnjuh.cn

[R01] shebang 与严格模式
来源：http://ev.shxzukj.cn

#!/usr/bin/env bash
来源：http://mc.9csxet.cn

set -euo pipefail
来源：http://yu.asd995.cn

[R02] 变量赋值与使用
来源：http://ox.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://je.lnxyls.cn

[R03] 只读变量
来源：http://sw.chemitech.net.cn

readonly PI=3.14
来源：http://ko.colortex.cn

[R04] 位置参数
来源：http://yk.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://go.shtwfgs.cn

[R05] 参数默认值
来源：http://dy.szxytkj.cn

name="${1:-default}"
来源：http://wu.shxzukj.cn

[R06] 判断命令是否存在
来源：http://ax.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wi.nicolike.cn

[R07] if 判断文件
来源：http://sw.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jw.chemitech.net.cn

[R08] 数值比较
来源：http://cx.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://de.yuntaijiaju.cn

[R09] 字符串比较
来源：http://ly.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cm.yuexingan06.cn

[R10] 正则匹配
来源：http://go.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bn.shxzskj.cn

[R11] case 多分支
来源：http://zr.shxzskj.cn

case "$1" in
来源：http://wh.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://hd.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://du.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://ds.521024.cn

esac
来源：http://kv.jctech888.com.cn

[R12] for 遍历文件
来源：http://ep.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://rh.jianghongdianzi.cn

[R13] for 计数循环
来源：http://wk.chemitech.net.cn


<!-- 参考信息 -->
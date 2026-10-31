代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zv.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jd.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wu.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bv.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ov.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oy.newstarts.cn

[P03] 生成短随机字符串
来源：http://lf.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ew.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ty.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tv.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kq.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xn.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dk.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://de.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uc.nszjky.cn

[P04] 求长度
来源：http://xu.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ud.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://om.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eo.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cg.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://dn.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://sk.nszjky.cn

Ruby: x.length;  x.size
来源：http://bv.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cf.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://rg.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mf.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ka.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aq.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qe.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qh.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yl.huixiangedu.cn

Ruby: a == b
来源：http://no.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hd.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zi.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oh.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://hm.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lh.szxytkj.cn

TS:   if (x == null) {}
来源：http://fi.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zc.chemitech.net.cn

Go:   if x == nil {}
来源：http://mf.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gq.huanxung.cn

C#:   if (x is null) {}
来源：http://by.nicolike.cn

[P07] 防抖与节流
来源：http://vr.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eg.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://wm.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fr.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://al.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tn.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ig.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ou.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yp.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://hh.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jq.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kq.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://at.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nw.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hg.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qp.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fs.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zc.yuexingan06.cn

================================================================================
来源：http://lg.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xd.bookmarksfly.cn

================================================================================
来源：http://fl.shxzskj.cn

[Q01] 创建表
来源：http://zt.chemitech.net.cn

CREATE TABLE users (
来源：http://ay.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zs.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://ke.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://jq.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ms.jctech888.com.cn

);
来源：http://bo.asd995.cn

[Q02] 创建带外键的表
来源：http://ad.panjiajie.cn

CREATE TABLE orders (
来源：http://ry.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bb.muxihuayi.cn

user_id INT NOT NULL,
来源：http://fh.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://ky.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lf.szsharing.cn

);
来源：http://ao.bookmarksfly.cn

[Q03] 增加列
来源：http://ms.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vc.szxytkj.cn

[Q04] 修改列类型
来源：http://fq.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://px.huixiangedu.cn

[Q05] 重命名列
来源：http://sz.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ml.jianghongdianzi.cn

[Q06] 删除列
来源：http://kv.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xb.9csxet.cn

[Q07] 删除表
来源：http://ul.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://il.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://dw.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cw.huanxung.cn

[Q09] 创建唯一索引
来源：http://wn.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://al.jianghongdianzi.cn

[Q10] 插入单行
来源：http://jg.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qd.lnxyls.cn

[Q11] 一次插入多行
来源：http://uw.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uj.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://hk.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gc.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qp.asd995.cn

[Q13] 忽略重复插入
来源：http://hk.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fw.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://jd.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eu.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xn.huanxung.cn

[Q15] 查询全部
来源：http://iy.huanxung.cn

SELECT * FROM users;
来源：http://ou.nszjky.cn

[Q16] 查询指定列
来源：http://fh.wgjwhj.cn

SELECT id, name FROM users;
来源：http://ju.nicolike.cn

[Q17] 条件查询
来源：http://ef.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://on.yuexingan06.cn

[Q18] 模糊匹配
来源：http://jw.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qg.yuntaijiaju.cn

[Q19] 范围查询
来源：http://on.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sr.jctech888.com.cn

[Q20] IN 列表
来源：http://nm.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gg.jctech888.com.cn

[Q21] 空值判断
来源：http://hi.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dj.gzmigu.cn

[Q22] 排序
来源：http://eg.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gh.shxzskj.cn

[Q23] 分页
来源：http://ne.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zx.lnxyls.cn

[Q24] 去重
来源：http://bk.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://bl.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://qt.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iw.gzmigu.cn

[Q26] 计数
来源：http://ym.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://qc.szsharing.cn

[Q27] 条件计数
来源：http://tb.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tm.colortex.cn

[Q28] 求和与平均
来源：http://zi.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rx.szxytkj.cn

[Q29] 最大最小值
来源：http://ac.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jg.yuntaijiaju.cn

[Q30] 分组统计
来源：http://rw.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oh.huanxung.cn

[Q31] 分组后过滤
来源：http://yc.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hn.huanxung.cn

[Q32] 分组拼接字符串
来源：http://uq.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dr.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eg.muxihuayi.cn

[Q33] 多列分组
来源：http://kp.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://er.nicolike.cn

[Q34] 每组取第一条
来源：http://ty.shxzskj.cn

SELECT * FROM (
来源：http://bg.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rz.huixiangedu.cn

) t WHERE rn = 1;
来源：http://wc.lnxyls.cn

[Q35] 内连接
来源：http://mc.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jp.hnjuh.cn

[Q36] 左连接
来源：http://bo.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mt.chemitech.net.cn

[Q37] 右连接
来源：http://hr.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cr.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ql.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://do.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://lk.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yj.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://im.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gn.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iw.jianghongdianzi.cn

[Q41] 多表连接
来源：http://ij.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dl.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://xr.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://tg.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://hu.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://nl.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ks.nszjky.cn

[Q43] 标量子查询
来源：http://be.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ds.yuexingan06.cn

[Q44] IN 子查询
来源：http://ls.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://px.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://hw.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ao.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fi.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://je.wgjwhj.cn

[Q47] 与平均值比较
来源：http://rn.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vg.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://mn.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ss.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://lm.panjiajie.cn

[Q49] 更新单行
来源：http://iu.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jz.hahajie.cn

[Q50] 批量更新
来源：http://zd.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://am.muxihuayi.cn

[Q51] 用子查询更新
来源：http://wm.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bm.hnjuh.cn

[Q52] 删除指定行
来源：http://dv.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://jl.muxihuayi.cn

[Q53] 按条件删除
来源：http://fe.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ef.wgjwhj.cn

[Q54] 清空表
来源：http://il.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://fd.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://wc.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qi.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://gh.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xs.nszjky.cn

[Q57] 行号
来源：http://dk.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ky.wgjwhj.cn

[Q58] 累计求和
来源：http://hx.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tj.haigaiapp.cn

[Q59] 分组内累计
来源：http://dv.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ry.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://pq.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ip.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cd.muxihuayi.cn

[Q61] 移动平均
来源：http://sd.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jz.shxzskj.cn

[Q62] 分组占比
来源：http://es.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jn.lnxyls.cn

[Q63] 开启事务
来源：http://zu.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nk.huixiangedu.cn

[Q64] 提交事务
来源：http://gm.hahajie.cn

COMMIT;
来源：http://nv.newstarts.cn

[Q65] 回滚事务
来源：http://kx.shtwfgs.cn

ROLLBACK;
来源：http://cr.bookmarksfly.cn

[Q66] 行锁查询
来源：http://ro.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sl.lnxyls.cn

[Q67] 设置隔离级别
来源：http://ed.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fn.bookmarksfly.cn

[Q68] 保存点
来源：http://xe.hahajie.cn

SAVEPOINT sp1;
来源：http://vp.szsharing.cn

ROLLBACK TO sp1;
来源：http://ud.jctech888.com.cn

[Q69] 查看执行计划
来源：http://ge.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://om.shxzskj.cn

[Q70] 更新统计信息
来源：http://cu.colortex.cn

ANALYZE TABLE users;
来源：http://qw.521024.cn

[Q71] 查看建表语句
来源：http://ob.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oj.hahajie.cn

[Q72] 查看索引
来源：http://hu.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://yw.shxzukj.cn

[Q73] 查看表状态
来源：http://vx.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mg.lnxyls.cn

[Q74] 强制使用索引
来源：http://hp.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yk.huixiangedu.cn

[Q75] 日期格式化
来源：http://tm.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pw.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pb.yuexingan06.cn

[Q76] 按天统计
来源：http://yo.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aj.yuntaijiaju.cn

[Q77] 时间加减
来源：http://zq.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uu.muxihuayi.cn

[Q78] 当前时间
来源：http://zq.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qe.nszjky.cn

[Q79] 字符串拼接
来源：http://tg.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cl.bjjhwx.cn

[Q80] 字符串截取
来源：http://zm.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.haigaiapp.cn

[Q81] 字符串替换
来源：http://kj.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rt.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://qa.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sm.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://to.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lg.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://ic.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://sb.bookmarksfly.cn

[Q85] 数值取整
来源：http://ke.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ce.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://df.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dh.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://dj.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zj.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://my.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://br.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zc.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://qk.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xh.muxihuayi.cn

[Q90] 生成序号列
来源：http://gc.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hd.jianghongdianzi.cn

================================================================================
来源：http://wl.muxihuayi.cn

R. Bash 专题
来源：http://wo.jianghongdianzi.cn

================================================================================
来源：http://vy.nszjky.cn

[R01] shebang 与严格模式
来源：http://ak.yuexingan06.cn

#!/usr/bin/env bash
来源：http://nl.gzmigu.cn

set -euo pipefail
来源：http://nm.colortex.cn

[R02] 变量赋值与使用
来源：http://rf.nszjky.cn

name="Tom"; echo "$name"
来源：http://ek.muxihuayi.cn

[R03] 只读变量
来源：http://nj.hahajie.cn

readonly PI=3.14
来源：http://yx.chemitech.net.cn

[R04] 位置参数
来源：http://sh.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://he.bjjhwx.cn

[R05] 参数默认值
来源：http://ju.asd995.cn

name="${1:-default}"
来源：http://bm.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://nm.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gl.haigaiapp.cn

[R07] if 判断文件
来源：http://ha.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cp.shxzskj.cn

[R08] 数值比较
来源：http://mu.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pw.521024.cn

[R09] 字符串比较
来源：http://it.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cw.huanxung.cn

[R10] 正则匹配
来源：http://xg.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ez.nszjky.cn

[R11] case 多分支
来源：http://ac.9csxet.cn

case "$1" in
来源：http://hw.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://jq.lnxyls.cn

stop)  echo "停止" ;;
来源：http://na.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://qs.hnjuh.cn

esac
来源：http://yo.521024.cn

[R12] for 遍历文件
来源：http://ld.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://lf.hahajie.cn

[R13] for 计数循环
来源：http://dd.colortex.cn


<!-- 参考信息 -->
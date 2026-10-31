代发 wailian999

C#:   Parallel.For
来源：http://tm.newstarts.cn

================================================================================
来源：http://wb.bjjhwx.cn

P. 常用工具函数
来源：http://gt.521024.cn

================================================================================
来源：http://og.bjjhwx.cn

[P01] 生成 UUID
来源：http://fz.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://mm.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pz.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://dt.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://ze.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://pg.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://ar.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://lb.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://ua.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://sj.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vg.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ew.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uj.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wd.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mn.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iy.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jb.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pg.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://cl.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xa.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ge.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ik.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://em.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vj.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hr.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ca.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bo.wgjwhj.cn

[P04] 求长度
来源：http://fl.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rn.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://se.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bt.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ci.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://ot.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://en.521024.cn

Ruby: x.length;  x.size
来源：http://ej.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hx.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://nu.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://di.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dv.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bz.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ff.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uj.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mn.nicolike.cn

Ruby: a == b
来源：http://hp.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xn.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zg.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rj.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://fn.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xt.muxihuayi.cn

TS:   if (x == null) {}
来源：http://as.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hb.huixiangedu.cn

Go:   if x == nil {}
来源：http://wt.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://um.szsharing.cn

C#:   if (x is null) {}
来源：http://aw.bookmarksfly.cn

[P07] 防抖与节流
来源：http://ig.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uw.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://lc.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://np.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xj.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vh.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sa.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eo.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vi.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://xd.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sg.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xb.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://si.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nd.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yn.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ws.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yb.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://er.nszjky.cn

================================================================================
来源：http://yz.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bf.chemitech.net.cn

================================================================================
来源：http://gt.yuexingan06.cn

[Q01] 创建表
来源：http://xq.yuntaijiaju.cn

CREATE TABLE users (
来源：http://kk.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hs.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://py.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://zr.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nm.jianghongdianzi.cn

);
来源：http://jz.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://da.yuexingan06.cn

CREATE TABLE orders (
来源：http://nf.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qm.shtwfgs.cn

user_id INT NOT NULL,
来源：http://ea.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://dv.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dn.szsharing.cn

);
来源：http://vv.nszjky.cn

[Q03] 增加列
来源：http://ah.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ke.yuexingan06.cn

[Q04] 修改列类型
来源：http://iu.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lw.lnxyls.cn

[Q05] 重命名列
来源：http://yn.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uw.yuexingan06.cn

[Q06] 删除列
来源：http://vm.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vs.jctech888.com.cn

[Q07] 删除表
来源：http://uv.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://tq.huanxung.cn

[Q08] 创建普通索引
来源：http://le.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cf.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://op.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rs.bjjhwx.cn

[Q10] 插入单行
来源：http://on.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://or.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://zn.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://js.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://ge.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qo.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ul.nszjky.cn

[Q13] 忽略重复插入
来源：http://fk.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ev.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://lz.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fu.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jd.nicolike.cn

[Q15] 查询全部
来源：http://ha.521024.cn

SELECT * FROM users;
来源：http://xm.9csxet.cn

[Q16] 查询指定列
来源：http://of.wgjwhj.cn

SELECT id, name FROM users;
来源：http://ou.9csxet.cn

[Q17] 条件查询
来源：http://vr.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fe.yuexingan06.cn

[Q18] 模糊匹配
来源：http://uk.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://om.hahajie.cn

[Q19] 范围查询
来源：http://kc.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qe.colortex.cn

[Q20] IN 列表
来源：http://za.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uk.shxzskj.cn

[Q21] 空值判断
来源：http://rf.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ov.hnjuh.cn

[Q22] 排序
来源：http://lt.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zz.hahajie.cn

[Q23] 分页
来源：http://ip.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oy.huixinmuqiang.cn

[Q24] 去重
来源：http://et.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://dr.shxzukj.cn

[Q25] 只取前 N 条
来源：http://lk.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lh.nszjky.cn

[Q26] 计数
来源：http://qs.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://dh.shtwfgs.cn

[Q27] 条件计数
来源：http://rg.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jx.wgjwhj.cn

[Q28] 求和与平均
来源：http://ry.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oi.9csxet.cn

[Q29] 最大最小值
来源：http://lu.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hn.bjjhwx.cn

[Q30] 分组统计
来源：http://js.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sc.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://bl.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wk.asd995.cn

[Q32] 分组拼接字符串
来源：http://us.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qm.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://is.jianghongdianzi.cn

[Q33] 多列分组
来源：http://qx.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ae.yuexingan06.cn

[Q34] 每组取第一条
来源：http://jt.asd995.cn

SELECT * FROM (
来源：http://dn.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gx.nicolike.cn

) t WHERE rn = 1;
来源：http://tx.wgjwhj.cn

[Q35] 内连接
来源：http://pp.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zl.szxytkj.cn

[Q36] 左连接
来源：http://tz.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kw.yuntaijiaju.cn

[Q37] 右连接
来源：http://ji.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vy.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pd.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ry.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ja.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wp.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gg.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pe.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fl.hahajie.cn

[Q41] 多表连接
来源：http://my.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://le.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://kl.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://kx.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://zz.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://oq.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jj.hnjuh.cn

[Q43] 标量子查询
来源：http://rs.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://up.asd995.cn

[Q44] IN 子查询
来源：http://za.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pd.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://ep.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wm.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jj.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://al.9csxet.cn

[Q47] 与平均值比较
来源：http://eq.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ur.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://ov.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ni.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://qb.nszjky.cn

[Q49] 更新单行
来源：http://bh.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oi.haigaiapp.cn

[Q50] 批量更新
来源：http://hs.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bj.chemitech.net.cn

[Q51] 用子查询更新
来源：http://ic.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ca.hahajie.cn

[Q52] 删除指定行
来源：http://ie.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://wd.bjjhwx.cn

[Q53] 按条件删除
来源：http://bm.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lu.yuexingan06.cn

[Q54] 清空表
来源：http://jp.hahajie.cn

TRUNCATE TABLE logs;
来源：http://kx.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://td.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oy.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://ry.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://il.bjjhwx.cn

[Q57] 行号
来源：http://nd.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://si.hnjuh.cn

[Q58] 累计求和
来源：http://zy.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fa.szsharing.cn

[Q59] 分组内累计
来源：http://xw.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zc.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://ly.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sh.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qa.muxihuayi.cn

[Q61] 移动平均
来源：http://ff.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pl.huanxung.cn

[Q62] 分组占比
来源：http://pn.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sx.szxytkj.cn

[Q63] 开启事务
来源：http://el.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vu.bookmarksfly.cn

[Q64] 提交事务
来源：http://xf.yuntaijiaju.cn

COMMIT;
来源：http://tx.panjiajie.cn

[Q65] 回滚事务
来源：http://sg.bjjhwx.cn

ROLLBACK;
来源：http://jf.shtwfgs.cn

[Q66] 行锁查询
来源：http://ab.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rr.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://lz.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://el.yuntaijiaju.cn

[Q68] 保存点
来源：http://vu.wgjwhj.cn

SAVEPOINT sp1;
来源：http://rt.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://cy.newstarts.cn

[Q69] 查看执行计划
来源：http://ip.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zw.szsharing.cn

[Q70] 更新统计信息
来源：http://nu.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://ap.asd995.cn

[Q71] 查看建表语句
来源：http://vg.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jv.huixinmuqiang.cn

[Q72] 查看索引
来源：http://fp.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://xb.gzmigu.cn

[Q73] 查看表状态
来源：http://wq.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zx.9csxet.cn

[Q74] 强制使用索引
来源：http://kb.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sd.chemitech.net.cn

[Q75] 日期格式化
来源：http://nl.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wj.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eq.chemitech.net.cn

[Q76] 按天统计
来源：http://py.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oz.huixiangedu.cn

[Q77] 时间加减
来源：http://yy.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bx.huixiangedu.cn

[Q78] 当前时间
来源：http://ga.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xo.chemitech.net.cn

[Q79] 字符串拼接
来源：http://jr.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fh.huanxung.cn

[Q80] 字符串截取
来源：http://co.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zc.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://iz.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bz.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://uu.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mt.shxzukj.cn

[Q83] 大小写转换
来源：http://yr.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ub.hahajie.cn

[Q84] 去除首尾空格
来源：http://zj.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://lw.newstarts.cn

[Q85] 数值取整
来源：http://ng.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ok.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://dy.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rb.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://qw.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mg.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://en.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qp.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hx.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://ej.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fn.shxzskj.cn

[Q90] 生成序号列
来源：http://nb.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mw.haigaiapp.cn

================================================================================
来源：http://bd.newstarts.cn

R. Bash 专题
来源：http://ae.hahajie.cn

================================================================================
来源：http://vg.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://cl.521024.cn

#!/usr/bin/env bash
来源：http://pl.muxihuayi.cn

set -euo pipefail
来源：http://xj.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ov.szsharing.cn

name="Tom"; echo "$name"
来源：http://mx.huanxung.cn

[R03] 只读变量
来源：http://hk.haigaiapp.cn

readonly PI=3.14
来源：http://ic.gzmigu.cn

[R04] 位置参数
来源：http://gi.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mq.shxzukj.cn

[R05] 参数默认值
来源：http://um.huanxung.cn

name="${1:-default}"
来源：http://ln.lnxyls.cn

[R06] 判断命令是否存在
来源：http://vr.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://en.wgjwhj.cn

[R07] if 判断文件
来源：http://pd.gzmigu.cn


<!-- 参考信息 -->
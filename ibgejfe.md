代发 wailian999

C#:   Parallel.For
来源：http://yh.nszjky.cn

================================================================================
来源：http://ob.panjiajie.cn

P. 常用工具函数
来源：http://su.haigaiapp.cn

================================================================================
来源：http://qc.lnxyls.cn

[P01] 生成 UUID
来源：http://rv.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://zl.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pl.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://rg.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://yh.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://ry.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://ds.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://fs.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://yc.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://yj.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gz.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lr.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zp.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mm.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://au.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ei.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tu.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qt.colortex.cn

[P03] 生成短随机字符串
来源：http://yd.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nd.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vf.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jd.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qe.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jt.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tt.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ts.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://op.nszjky.cn

[P04] 求长度
来源：http://iv.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xm.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jn.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xm.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ge.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://jd.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://zc.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://hh.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kp.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://lf.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qz.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ie.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sx.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eo.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tz.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ix.bookmarksfly.cn

Ruby: a == b
来源：http://iv.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dk.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://le.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ke.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://er.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pf.yuexingan06.cn

TS:   if (x == null) {}
来源：http://fu.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lu.yuexingan06.cn

Go:   if x == nil {}
来源：http://rb.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ow.newstarts.cn

C#:   if (x is null) {}
来源：http://yk.hnjuh.cn

[P07] 防抖与节流
来源：http://mf.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bh.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://nq.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dv.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ez.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ps.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tu.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ay.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ni.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://xy.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gc.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qe.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rj.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nf.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zm.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lq.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zk.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cd.bjjhwx.cn

================================================================================
来源：http://yy.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mx.yuntaijiaju.cn

================================================================================
来源：http://xt.shxzskj.cn

[Q01] 创建表
来源：http://ey.bjjhwx.cn

CREATE TABLE users (
来源：http://jy.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qx.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://zz.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://li.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ae.shxzukj.cn

);
来源：http://cx.shxzukj.cn

[Q02] 创建带外键的表
来源：http://hg.bookmarksfly.cn

CREATE TABLE orders (
来源：http://yl.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mm.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://gv.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://jy.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://th.huixiangedu.cn

);
来源：http://df.gzmigu.cn

[Q03] 增加列
来源：http://tb.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qo.bookmarksfly.cn

[Q04] 修改列类型
来源：http://xe.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zn.521024.cn

[Q05] 重命名列
来源：http://xi.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yg.shxzskj.cn

[Q06] 删除列
来源：http://ej.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hq.shtwfgs.cn

[Q07] 删除表
来源：http://do.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://kn.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://hu.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rx.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://cv.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wm.szxytkj.cn

[Q10] 插入单行
来源：http://cf.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lw.szxytkj.cn

[Q11] 一次插入多行
来源：http://ri.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sx.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ih.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hf.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xp.gzmigu.cn

[Q13] 忽略重复插入
来源：http://aq.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aj.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://jy.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cy.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rv.shxzukj.cn

[Q15] 查询全部
来源：http://kl.haigaiapp.cn

SELECT * FROM users;
来源：http://kl.huixiangedu.cn

[Q16] 查询指定列
来源：http://ry.huixiangedu.cn

SELECT id, name FROM users;
来源：http://dk.nicolike.cn

[Q17] 条件查询
来源：http://rg.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bn.szxytkj.cn

[Q18] 模糊匹配
来源：http://iu.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zm.wgjwhj.cn

[Q19] 范围查询
来源：http://zr.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uk.szsharing.cn

[Q20] IN 列表
来源：http://vp.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ca.shxzskj.cn

[Q21] 空值判断
来源：http://lg.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://th.gzmigu.cn

[Q22] 排序
来源：http://xz.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yi.szsharing.cn

[Q23] 分页
来源：http://tu.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ys.yuntaijiaju.cn

[Q24] 去重
来源：http://do.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://bl.nszjky.cn

[Q25] 只取前 N 条
来源：http://xt.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qk.yuntaijiaju.cn

[Q26] 计数
来源：http://qu.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://pq.shxzukj.cn

[Q27] 条件计数
来源：http://mu.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ti.bookmarksfly.cn

[Q28] 求和与平均
来源：http://pp.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tr.colortex.cn

[Q29] 最大最小值
来源：http://la.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hr.yuntaijiaju.cn

[Q30] 分组统计
来源：http://dq.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ui.asd995.cn

[Q31] 分组后过滤
来源：http://tp.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pt.9csxet.cn

[Q32] 分组拼接字符串
来源：http://au.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oe.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vo.gzmigu.cn

[Q33] 多列分组
来源：http://ae.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://td.shtwfgs.cn

[Q34] 每组取第一条
来源：http://jv.yuexingan06.cn

SELECT * FROM (
来源：http://mb.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xq.newstarts.cn

) t WHERE rn = 1;
来源：http://cx.yuexingan06.cn

[Q35] 内连接
来源：http://yt.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bn.yuexingan06.cn

[Q36] 左连接
来源：http://li.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ej.yuexingan06.cn

[Q37] 右连接
来源：http://pk.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qn.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ms.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nd.colortex.cn

[Q39] 自连接（查上下级）
来源：http://gk.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hq.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hw.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kz.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nf.bjjhwx.cn

[Q41] 多表连接
来源：http://am.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dp.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://xf.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://lw.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://la.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://sc.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wz.gzmigu.cn

[Q43] 标量子查询
来源：http://jk.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sf.chemitech.net.cn

[Q44] IN 子查询
来源：http://mf.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qd.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ds.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://am.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rc.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ap.newstarts.cn

[Q47] 与平均值比较
来源：http://hn.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hg.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://qy.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pe.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://fm.shxzukj.cn

[Q49] 更新单行
来源：http://ok.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rj.szxytkj.cn

[Q50] 批量更新
来源：http://sv.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://le.muxihuayi.cn

[Q51] 用子查询更新
来源：http://ek.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mh.haigaiapp.cn

[Q52] 删除指定行
来源：http://my.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://mg.521024.cn

[Q53] 按条件删除
来源：http://ni.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://je.yuexingan06.cn

[Q54] 清空表
来源：http://cs.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://eq.nicolike.cn

[Q55] 排名（并列占位）
来源：http://qc.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ie.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://nf.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vb.jianghongdianzi.cn

[Q57] 行号
来源：http://mk.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lm.jianghongdianzi.cn

[Q58] 累计求和
来源：http://sz.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bc.szxytkj.cn

[Q59] 分组内累计
来源：http://dh.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qj.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://it.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zf.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ho.bjjhwx.cn

[Q61] 移动平均
来源：http://iv.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rp.szxytkj.cn

[Q62] 分组占比
来源：http://co.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ke.haigaiapp.cn

[Q63] 开启事务
来源：http://uz.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rg.chemitech.net.cn

[Q64] 提交事务
来源：http://eq.yuntaijiaju.cn

COMMIT;
来源：http://lt.9csxet.cn

[Q65] 回滚事务
来源：http://cj.panjiajie.cn

ROLLBACK;
来源：http://mz.muxihuayi.cn

[Q66] 行锁查询
来源：http://wz.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wn.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://ec.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://go.9csxet.cn

[Q68] 保存点
来源：http://jd.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://it.nszjky.cn

ROLLBACK TO sp1;
来源：http://io.szsharing.cn

[Q69] 查看执行计划
来源：http://ab.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qj.chemitech.net.cn

[Q70] 更新统计信息
来源：http://om.lnxyls.cn

ANALYZE TABLE users;
来源：http://ga.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://vd.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rm.wgjwhj.cn

[Q72] 查看索引
来源：http://sg.szsharing.cn

SHOW INDEX FROM users;
来源：http://pa.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://da.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dn.nicolike.cn

[Q74] 强制使用索引
来源：http://ou.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://me.haigaiapp.cn

[Q75] 日期格式化
来源：http://nf.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bo.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uh.lnxyls.cn

[Q76] 按天统计
来源：http://oi.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fq.shtwfgs.cn

[Q77] 时间加减
来源：http://fc.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ls.jctech888.com.cn

[Q78] 当前时间
来源：http://zx.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mt.hnjuh.cn

[Q79] 字符串拼接
来源：http://un.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vo.nicolike.cn

[Q80] 字符串截取
来源：http://lm.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ot.hnjuh.cn

[Q81] 字符串替换
来源：http://uc.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lf.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://xo.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rb.newstarts.cn

[Q83] 大小写转换
来源：http://hs.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lx.panjiajie.cn

[Q84] 去除首尾空格
来源：http://hi.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://ux.colortex.cn

[Q85] 数值取整
来源：http://va.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jb.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://ze.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xr.newstarts.cn

[Q87] JSON 字段做条件
来源：http://qn.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ax.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://ku.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hi.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ti.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://xx.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://en.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://jb.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gw.huanxung.cn

================================================================================
来源：http://vg.huixiangedu.cn

R. Bash 专题
来源：http://dr.szsharing.cn

================================================================================
来源：http://ui.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://sb.newstarts.cn

#!/usr/bin/env bash
来源：http://wi.9csxet.cn

set -euo pipefail
来源：http://uq.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://ku.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://iz.9csxet.cn

[R03] 只读变量
来源：http://sf.bjjhwx.cn

readonly PI=3.14
来源：http://ir.chemitech.net.cn

[R04] 位置参数
来源：http://xd.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kd.521024.cn

[R05] 参数默认值
来源：http://lk.colortex.cn

name="${1:-default}"
来源：http://af.szsharing.cn

[R06] 判断命令是否存在
来源：http://lq.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ym.shxzskj.cn

[R07] if 判断文件
来源：http://yw.haigaiapp.cn


<!-- 参考信息 -->
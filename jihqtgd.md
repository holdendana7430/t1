代发 wailian999

C#:   Parallel.For
来源：http://kh.hnjuh.cn

================================================================================
来源：http://yo.muxihuayi.cn

P. 常用工具函数
来源：http://ei.gzmigu.cn

================================================================================
来源：http://dj.bjjhwx.cn

[P01] 生成 UUID
来源：http://xh.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://aa.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hc.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ed.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ry.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://iy.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://si.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://tl.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://va.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://fa.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rg.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bf.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xb.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vu.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nc.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gn.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ie.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ie.szsharing.cn

[P03] 生成短随机字符串
来源：http://vs.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sh.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tb.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kx.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hw.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lp.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pa.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gl.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ei.hahajie.cn

[P04] 求长度
来源：http://wa.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tp.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sq.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qu.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tk.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://me.asd995.cn

Go:   len(arr);  len(m)
来源：http://vu.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://kp.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dq.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://zx.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jk.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ut.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gd.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://it.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vi.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yb.hnjuh.cn

Ruby: a == b
来源：http://fh.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nq.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fc.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hp.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://bw.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xj.newstarts.cn

TS:   if (x == null) {}
来源：http://zf.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dg.lnxyls.cn

Go:   if x == nil {}
来源：http://mm.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cw.521024.cn

C#:   if (x is null) {}
来源：http://oz.newstarts.cn

[P07] 防抖与节流
来源：http://ei.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qi.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://ni.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yg.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kd.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wj.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sg.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zg.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://xe.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sv.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cu.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bp.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://la.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nf.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pr.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nf.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xg.colortex.cn

================================================================================
来源：http://lc.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pq.jctech888.com.cn

================================================================================
来源：http://am.asd995.cn

[Q01] 创建表
来源：http://iz.huixinmuqiang.cn

CREATE TABLE users (
来源：http://mk.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qy.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://bq.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://ab.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ic.szsharing.cn

);
来源：http://fx.9csxet.cn

[Q02] 创建带外键的表
来源：http://nc.bookmarksfly.cn

CREATE TABLE orders (
来源：http://jo.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ub.huixiangedu.cn

user_id INT NOT NULL,
来源：http://fe.szsharing.cn

amount DECIMAL(10, 2),
来源：http://gk.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jx.hnjuh.cn

);
来源：http://ak.huixinmuqiang.cn

[Q03] 增加列
来源：http://zc.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ti.szxytkj.cn

[Q04] 修改列类型
来源：http://aw.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oi.bjjhwx.cn

[Q05] 重命名列
来源：http://qv.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zp.chemitech.net.cn

[Q06] 删除列
来源：http://zo.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zi.hnjuh.cn

[Q07] 删除表
来源：http://fi.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://hn.huanxung.cn

[Q08] 创建普通索引
来源：http://hm.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ty.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://ij.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ub.nszjky.cn

[Q10] 插入单行
来源：http://af.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dk.colortex.cn

[Q11] 一次插入多行
来源：http://dh.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ws.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://xu.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jr.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://np.colortex.cn

[Q13] 忽略重复插入
来源：http://lh.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sa.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://lq.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ko.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://te.hahajie.cn

[Q15] 查询全部
来源：http://bo.hnjuh.cn

SELECT * FROM users;
来源：http://is.gzmigu.cn

[Q16] 查询指定列
来源：http://sf.521024.cn

SELECT id, name FROM users;
来源：http://dx.lnxyls.cn

[Q17] 条件查询
来源：http://eg.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bo.nszjky.cn

[Q18] 模糊匹配
来源：http://ma.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kr.panjiajie.cn

[Q19] 范围查询
来源：http://ch.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wl.nicolike.cn

[Q20] IN 列表
来源：http://cp.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nw.bookmarksfly.cn

[Q21] 空值判断
来源：http://ag.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vc.huanxung.cn

[Q22] 排序
来源：http://rr.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lq.hnjuh.cn

[Q23] 分页
来源：http://et.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dp.huanxung.cn

[Q24] 去重
来源：http://vu.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://en.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://rg.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zy.521024.cn

[Q26] 计数
来源：http://oj.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://gy.muxihuayi.cn

[Q27] 条件计数
来源：http://yl.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oq.szsharing.cn

[Q28] 求和与平均
来源：http://wk.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pi.gzmigu.cn

[Q29] 最大最小值
来源：http://bo.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kl.lnxyls.cn

[Q30] 分组统计
来源：http://sx.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vz.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://xb.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rw.nicolike.cn

[Q32] 分组拼接字符串
来源：http://nw.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bs.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://id.yuntaijiaju.cn

[Q33] 多列分组
来源：http://bc.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nk.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://qv.bjjhwx.cn

SELECT * FROM (
来源：http://ah.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cz.shtwfgs.cn

) t WHERE rn = 1;
来源：http://ro.yuexingan06.cn

[Q35] 内连接
来源：http://jg.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ck.colortex.cn

[Q36] 左连接
来源：http://fo.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xv.chemitech.net.cn

[Q37] 右连接
来源：http://ai.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bm.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ob.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gh.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://jy.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eb.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mn.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gx.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ig.wgjwhj.cn

[Q41] 多表连接
来源：http://md.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vl.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://ch.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://uk.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://js.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://pr.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bu.yuexingan06.cn

[Q43] 标量子查询
来源：http://gj.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xm.nszjky.cn

[Q44] IN 子查询
来源：http://jj.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gj.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://li.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qj.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xb.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://as.huixiangedu.cn

[Q47] 与平均值比较
来源：http://wm.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mt.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://lz.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dl.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://ca.yuntaijiaju.cn

[Q49] 更新单行
来源：http://kt.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ds.huanxung.cn

[Q50] 批量更新
来源：http://ew.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tu.gzmigu.cn

[Q51] 用子查询更新
来源：http://by.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lu.muxihuayi.cn

[Q52] 删除指定行
来源：http://ea.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://fi.9csxet.cn

[Q53] 按条件删除
来源：http://ay.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qi.bjjhwx.cn

[Q54] 清空表
来源：http://ev.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://am.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://lm.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aa.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://pr.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fb.shxzukj.cn

[Q57] 行号
来源：http://ib.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fd.shxzskj.cn

[Q58] 累计求和
来源：http://sb.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wl.haigaiapp.cn

[Q59] 分组内累计
来源：http://ho.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://su.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://vm.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iq.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fa.nicolike.cn

[Q61] 移动平均
来源：http://qd.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cd.shxzukj.cn

[Q62] 分组占比
来源：http://in.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wm.shxzukj.cn

[Q63] 开启事务
来源：http://nx.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xf.gzmigu.cn

[Q64] 提交事务
来源：http://kb.yuntaijiaju.cn

COMMIT;
来源：http://pw.521024.cn

[Q65] 回滚事务
来源：http://vh.haigaiapp.cn

ROLLBACK;
来源：http://ip.521024.cn

[Q66] 行锁查询
来源：http://tu.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jl.szsharing.cn

[Q67] 设置隔离级别
来源：http://kx.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ce.wgjwhj.cn

[Q68] 保存点
来源：http://aq.nicolike.cn

SAVEPOINT sp1;
来源：http://ei.nicolike.cn

ROLLBACK TO sp1;
来源：http://xg.muxihuayi.cn

[Q69] 查看执行计划
来源：http://km.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ko.colortex.cn

[Q70] 更新统计信息
来源：http://bw.yuexingan06.cn

ANALYZE TABLE users;
来源：http://gs.asd995.cn

[Q71] 查看建表语句
来源：http://xg.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ts.shxzukj.cn

[Q72] 查看索引
来源：http://vm.newstarts.cn

SHOW INDEX FROM users;
来源：http://wk.nicolike.cn

[Q73] 查看表状态
来源：http://va.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://of.shxzukj.cn

[Q74] 强制使用索引
来源：http://pz.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zi.newstarts.cn

[Q75] 日期格式化
来源：http://it.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cs.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kf.521024.cn

[Q76] 按天统计
来源：http://eh.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uc.panjiajie.cn

[Q77] 时间加减
来源：http://ew.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ve.bjjhwx.cn

[Q78] 当前时间
来源：http://kf.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jm.asd995.cn

[Q79] 字符串拼接
来源：http://qt.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ki.szxytkj.cn

[Q80] 字符串截取
来源：http://wb.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xi.muxihuayi.cn

[Q81] 字符串替换
来源：http://lt.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dr.asd995.cn

[Q82] 字符长度与字节长度
来源：http://gg.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vh.huixiangedu.cn

[Q83] 大小写转换
来源：http://nu.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://io.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://uv.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://mk.colortex.cn

[Q85] 数值取整
来源：http://dj.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wl.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://za.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cq.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ym.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yn.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://mq.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://su.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oo.shxzukj.cn

[Q89] 判断表是否存在
来源：http://fg.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tb.shxzskj.cn

[Q90] 生成序号列
来源：http://lw.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ud.bookmarksfly.cn

================================================================================
来源：http://cu.panjiajie.cn

R. Bash 专题
来源：http://fo.yuntaijiaju.cn

================================================================================
来源：http://kx.gzmigu.cn

[R01] shebang 与严格模式
来源：http://uk.shtwfgs.cn

#!/usr/bin/env bash
来源：http://jx.wgjwhj.cn

set -euo pipefail
来源：http://jz.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://fb.colortex.cn

name="Tom"; echo "$name"
来源：http://qm.shxzukj.cn

[R03] 只读变量
来源：http://rl.huixinmuqiang.cn

readonly PI=3.14
来源：http://sm.colortex.cn

[R04] 位置参数
来源：http://lz.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vu.521024.cn

[R05] 参数默认值
来源：http://fu.muxihuayi.cn

name="${1:-default}"
来源：http://mx.hnjuh.cn

[R06] 判断命令是否存在
来源：http://ts.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hh.colortex.cn

[R07] if 判断文件
来源：http://da.huixiangedu.cn


<!-- 参考信息 -->
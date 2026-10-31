代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ry.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://su.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://no.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uj.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jn.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zx.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://mm.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pi.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aw.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qi.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tt.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bx.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mv.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gu.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://is.wgjwhj.cn

[P04] 求长度
来源：http://xo.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sb.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cg.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nj.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fb.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://mc.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://cs.szsharing.cn

Ruby: x.length;  x.size
来源：http://ck.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vj.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://ee.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oz.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://up.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hd.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qr.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cx.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rq.bjjhwx.cn

Ruby: a == b
来源：http://wj.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ai.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wd.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yg.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://yo.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mi.521024.cn

TS:   if (x == null) {}
来源：http://te.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xw.wgjwhj.cn

Go:   if x == nil {}
来源：http://tn.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lf.yuexingan06.cn

C#:   if (x is null) {}
来源：http://ib.asd995.cn

[P07] 防抖与节流
来源：http://kl.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yb.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://eb.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pq.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ld.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://df.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fm.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jb.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ze.asd995.cn

[P08] 处理浮点精度问题
来源：http://tr.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://in.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pl.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ai.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ai.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hx.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mc.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://la.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zr.colortex.cn

================================================================================
来源：http://hf.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ho.haigaiapp.cn

================================================================================
来源：http://rk.chemitech.net.cn

[Q01] 创建表
来源：http://pu.muxihuayi.cn

CREATE TABLE users (
来源：http://ta.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qy.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://dh.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://yc.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bw.szxytkj.cn

);
来源：http://ma.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://lr.shxzskj.cn

CREATE TABLE orders (
来源：http://ba.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://af.nszjky.cn

user_id INT NOT NULL,
来源：http://ws.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://zf.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yf.bjjhwx.cn

);
来源：http://ls.nszjky.cn

[Q03] 增加列
来源：http://zd.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yu.colortex.cn

[Q04] 修改列类型
来源：http://sg.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jt.shxzskj.cn

[Q05] 重命名列
来源：http://uo.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vy.haigaiapp.cn

[Q06] 删除列
来源：http://ft.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ab.shtwfgs.cn

[Q07] 删除表
来源：http://zm.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://go.nicolike.cn

[Q08] 创建普通索引
来源：http://ax.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bs.shxzukj.cn

[Q09] 创建唯一索引
来源：http://wd.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zq.lnxyls.cn

[Q10] 插入单行
来源：http://ov.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ox.nicolike.cn

[Q11] 一次插入多行
来源：http://sr.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://js.colortex.cn

[Q12] 插入后取自增 ID
来源：http://wz.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lt.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rd.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://fn.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pc.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://bu.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yz.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ue.colortex.cn

[Q15] 查询全部
来源：http://at.huanxung.cn

SELECT * FROM users;
来源：http://co.huanxung.cn

[Q16] 查询指定列
来源：http://lx.chemitech.net.cn

SELECT id, name FROM users;
来源：http://lq.huanxung.cn

[Q17] 条件查询
来源：http://up.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://av.huanxung.cn

[Q18] 模糊匹配
来源：http://ii.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zl.hnjuh.cn

[Q19] 范围查询
来源：http://ff.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pu.huixinmuqiang.cn

[Q20] IN 列表
来源：http://ap.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://he.newstarts.cn

[Q21] 空值判断
来源：http://dn.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iz.gzmigu.cn

[Q22] 排序
来源：http://ny.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fi.yuntaijiaju.cn

[Q23] 分页
来源：http://ja.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tc.huanxung.cn

[Q24] 去重
来源：http://is.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://rh.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://ra.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zc.wgjwhj.cn

[Q26] 计数
来源：http://md.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://xm.shtwfgs.cn

[Q27] 条件计数
来源：http://ei.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ot.asd995.cn

[Q28] 求和与平均
来源：http://gt.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sz.hahajie.cn

[Q29] 最大最小值
来源：http://wy.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zi.colortex.cn

[Q30] 分组统计
来源：http://pk.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rm.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ov.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xw.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://nu.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vx.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://om.9csxet.cn

[Q33] 多列分组
来源：http://bl.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qe.colortex.cn

[Q34] 每组取第一条
来源：http://qm.bjjhwx.cn

SELECT * FROM (
来源：http://hu.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ud.hahajie.cn

) t WHERE rn = 1;
来源：http://nt.huanxung.cn

[Q35] 内连接
来源：http://cu.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://or.hnjuh.cn

[Q36] 左连接
来源：http://je.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wq.haigaiapp.cn

[Q37] 右连接
来源：http://cp.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jf.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vf.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ef.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://xf.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sf.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ot.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ix.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gj.jctech888.com.cn

[Q41] 多表连接
来源：http://bj.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rv.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://nh.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://ou.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://sv.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://tu.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vb.szxytkj.cn

[Q43] 标量子查询
来源：http://og.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hq.9csxet.cn

[Q44] IN 子查询
来源：http://or.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dj.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://vn.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zd.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fx.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hk.shxzukj.cn

[Q47] 与平均值比较
来源：http://bf.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://de.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://mj.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ou.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://lx.jianghongdianzi.cn

[Q49] 更新单行
来源：http://vj.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nd.bjjhwx.cn

[Q50] 批量更新
来源：http://aw.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dq.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://cl.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bn.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://hp.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://ay.asd995.cn

[Q53] 按条件删除
来源：http://aq.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ke.gzmigu.cn

[Q54] 清空表
来源：http://hc.nszjky.cn

TRUNCATE TABLE logs;
来源：http://ig.newstarts.cn

[Q55] 排名（并列占位）
来源：http://qf.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gc.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://mu.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xm.asd995.cn

[Q57] 行号
来源：http://rc.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pb.521024.cn

[Q58] 累计求和
来源：http://ub.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ml.hnjuh.cn

[Q59] 分组内累计
来源：http://sh.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nm.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://vw.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ez.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vt.hnjuh.cn

[Q61] 移动平均
来源：http://xx.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sn.huanxung.cn

[Q62] 分组占比
来源：http://ul.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://up.newstarts.cn

[Q63] 开启事务
来源：http://pt.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sf.yuntaijiaju.cn

[Q64] 提交事务
来源：http://gc.yuexingan06.cn

COMMIT;
来源：http://no.hnjuh.cn

[Q65] 回滚事务
来源：http://yd.hnjuh.cn

ROLLBACK;
来源：http://ex.9csxet.cn

[Q66] 行锁查询
来源：http://ag.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xf.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://hc.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.haigaiapp.cn

[Q68] 保存点
来源：http://at.wgjwhj.cn

SAVEPOINT sp1;
来源：http://fg.asd995.cn

ROLLBACK TO sp1;
来源：http://iy.hahajie.cn

[Q69] 查看执行计划
来源：http://te.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ml.colortex.cn

[Q70] 更新统计信息
来源：http://zx.gzmigu.cn

ANALYZE TABLE users;
来源：http://bv.chemitech.net.cn

[Q71] 查看建表语句
来源：http://ih.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fa.hnjuh.cn

[Q72] 查看索引
来源：http://br.hahajie.cn

SHOW INDEX FROM users;
来源：http://ia.muxihuayi.cn

[Q73] 查看表状态
来源：http://zi.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ic.shxzukj.cn

[Q74] 强制使用索引
来源：http://wx.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nf.jctech888.com.cn

[Q75] 日期格式化
来源：http://sw.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tu.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nn.nicolike.cn

[Q76] 按天统计
来源：http://zq.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nm.shxzskj.cn

[Q77] 时间加减
来源：http://kp.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hl.muxihuayi.cn

[Q78] 当前时间
来源：http://ot.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fg.colortex.cn

[Q79] 字符串拼接
来源：http://tk.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ok.bjjhwx.cn

[Q80] 字符串截取
来源：http://sa.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ww.szsharing.cn

[Q81] 字符串替换
来源：http://tk.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dv.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://vt.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yj.asd995.cn

[Q83] 大小写转换
来源：http://ye.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zd.szxytkj.cn

[Q84] 去除首尾空格
来源：http://cl.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://lk.asd995.cn

[Q85] 数值取整
来源：http://oy.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ma.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://xs.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pc.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://be.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fy.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://zt.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ip.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jr.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://nj.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://md.huixiangedu.cn

[Q90] 生成序号列
来源：http://dn.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ye.wgjwhj.cn

================================================================================
来源：http://by.jianghongdianzi.cn

R. Bash 专题
来源：http://ml.gzmigu.cn

================================================================================
来源：http://au.nszjky.cn

[R01] shebang 与严格模式
来源：http://hy.panjiajie.cn

#!/usr/bin/env bash
来源：http://uc.huixinmuqiang.cn

set -euo pipefail
来源：http://fx.szsharing.cn

[R02] 变量赋值与使用
来源：http://fl.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://uo.jianghongdianzi.cn

[R03] 只读变量
来源：http://lf.asd995.cn

readonly PI=3.14
来源：http://zf.yuntaijiaju.cn

[R04] 位置参数
来源：http://hw.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bn.nicolike.cn

[R05] 参数默认值
来源：http://ft.newstarts.cn

name="${1:-default}"
来源：http://xv.hahajie.cn

[R06] 判断命令是否存在
来源：http://mp.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ch.shxzukj.cn

[R07] if 判断文件
来源：http://ce.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dx.huixiangedu.cn

[R08] 数值比较
来源：http://sx.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ko.shtwfgs.cn

[R09] 字符串比较
来源：http://zf.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ts.521024.cn

[R10] 正则匹配
来源：http://tg.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xu.nicolike.cn

[R11] case 多分支
来源：http://qz.huanxung.cn

case "$1" in
来源：http://sg.szxytkj.cn

start) echo "启动" ;;
来源：http://nc.nicolike.cn

stop)  echo "停止" ;;
来源：http://pa.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://kn.wgjwhj.cn

esac
来源：http://hi.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://jk.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://nl.shtwfgs.cn

[R13] for 计数循环
来源：http://oe.chemitech.net.cn


<!-- 参考信息 -->
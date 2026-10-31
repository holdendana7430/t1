代发 wailian999

[P01] 生成 UUID
来源：http://wy.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://te.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ex.nicolike.cn

JS:   crypto.randomUUID()
来源：http://xc.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://lo.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://co.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://qf.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://oy.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://xz.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://ca.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mz.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bp.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://et.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ev.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kl.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://et.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wc.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qr.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://gs.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://an.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zt.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kq.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oh.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uo.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mf.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xc.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ys.9csxet.cn

[P04] 求长度
来源：http://eo.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://au.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hb.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iz.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ck.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://of.521024.cn

Go:   len(arr);  len(m)
来源：http://pp.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://kc.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fj.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://sy.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sd.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://np.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yl.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ms.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ko.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pu.chemitech.net.cn

Ruby: a == b
来源：http://zv.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mu.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ps.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eo.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://dw.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sb.hnjuh.cn

TS:   if (x == null) {}
来源：http://bv.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ou.muxihuayi.cn

Go:   if x == nil {}
来源：http://pl.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zp.521024.cn

C#:   if (x is null) {}
来源：http://ii.shxzskj.cn

[P07] 防抖与节流
来源：http://zr.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jo.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://gv.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sm.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://on.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jl.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nz.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://og.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ow.colortex.cn

[P08] 处理浮点精度问题
来源：http://zf.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hy.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dg.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zj.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kg.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://og.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uj.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jy.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://br.lnxyls.cn

================================================================================
来源：http://uz.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aw.hahajie.cn

================================================================================
来源：http://py.shxzukj.cn

[Q01] 创建表
来源：http://im.lnxyls.cn

CREATE TABLE users (
来源：http://ia.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bk.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://qt.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://in.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ya.haigaiapp.cn

);
来源：http://at.hnjuh.cn

[Q02] 创建带外键的表
来源：http://he.hahajie.cn

CREATE TABLE orders (
来源：http://cw.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yk.9csxet.cn

user_id INT NOT NULL,
来源：http://nn.newstarts.cn

amount DECIMAL(10, 2),
来源：http://mi.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ym.hahajie.cn

);
来源：http://tq.asd995.cn

[Q03] 增加列
来源：http://ul.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tq.yuexingan06.cn

[Q04] 修改列类型
来源：http://ko.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kk.yuntaijiaju.cn

[Q05] 重命名列
来源：http://vw.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ty.gzmigu.cn

[Q06] 删除列
来源：http://nm.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ib.jianghongdianzi.cn

[Q07] 删除表
来源：http://li.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://kq.szsharing.cn

[Q08] 创建普通索引
来源：http://ht.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jd.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://bk.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oh.hnjuh.cn

[Q10] 插入单行
来源：http://ny.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pp.shxzukj.cn

[Q11] 一次插入多行
来源：http://lx.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nz.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://fc.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nn.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nc.gzmigu.cn

[Q13] 忽略重复插入
来源：http://ae.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://np.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://xj.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://td.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qj.lnxyls.cn

[Q15] 查询全部
来源：http://wa.szsharing.cn

SELECT * FROM users;
来源：http://yz.szxytkj.cn

[Q16] 查询指定列
来源：http://zi.yuexingan06.cn

SELECT id, name FROM users;
来源：http://iu.shtwfgs.cn

[Q17] 条件查询
来源：http://oh.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rn.shtwfgs.cn

[Q18] 模糊匹配
来源：http://sq.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://va.huixinmuqiang.cn

[Q19] 范围查询
来源：http://hn.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lp.colortex.cn

[Q20] IN 列表
来源：http://ur.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qd.jctech888.com.cn

[Q21] 空值判断
来源：http://ak.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ff.huanxung.cn

[Q22] 排序
来源：http://yb.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ak.chemitech.net.cn

[Q23] 分页
来源：http://tn.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hn.shxzskj.cn

[Q24] 去重
来源：http://ep.521024.cn

SELECT DISTINCT city FROM users;
来源：http://go.521024.cn

[Q25] 只取前 N 条
来源：http://vw.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ir.asd995.cn

[Q26] 计数
来源：http://kc.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://ny.szsharing.cn

[Q27] 条件计数
来源：http://cm.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://py.muxihuayi.cn

[Q28] 求和与平均
来源：http://oo.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pz.asd995.cn

[Q29] 最大最小值
来源：http://he.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jt.bookmarksfly.cn

[Q30] 分组统计
来源：http://rs.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hn.chemitech.net.cn

[Q31] 分组后过滤
来源：http://vy.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ou.newstarts.cn

[Q32] 分组拼接字符串
来源：http://co.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yw.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wr.lnxyls.cn

[Q33] 多列分组
来源：http://mc.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fx.muxihuayi.cn

[Q34] 每组取第一条
来源：http://ir.bjjhwx.cn

SELECT * FROM (
来源：http://wf.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vy.newstarts.cn

) t WHERE rn = 1;
来源：http://xw.jctech888.com.cn

[Q35] 内连接
来源：http://gk.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ah.colortex.cn

[Q36] 左连接
来源：http://sl.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qr.jctech888.com.cn

[Q37] 右连接
来源：http://of.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fh.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://po.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yy.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://op.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zo.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yc.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rv.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ad.yuntaijiaju.cn

[Q41] 多表连接
来源：http://lr.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bv.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://pw.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://qm.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://rx.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://lo.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://de.asd995.cn

[Q43] 标量子查询
来源：http://il.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cd.521024.cn

[Q44] IN 子查询
来源：http://av.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lg.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ce.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gc.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yv.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rp.panjiajie.cn

[Q47] 与平均值比较
来源：http://xo.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mz.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://ed.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yk.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ds.hnjuh.cn

[Q49] 更新单行
来源：http://bt.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hs.yuntaijiaju.cn

[Q50] 批量更新
来源：http://iv.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qy.bjjhwx.cn

[Q51] 用子查询更新
来源：http://xg.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wj.nszjky.cn

[Q52] 删除指定行
来源：http://aw.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://io.szxytkj.cn

[Q53] 按条件删除
来源：http://dl.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yc.bjjhwx.cn

[Q54] 清空表
来源：http://hv.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://ci.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://oh.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bs.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://ek.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wz.hahajie.cn

[Q57] 行号
来源：http://zk.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vl.bookmarksfly.cn

[Q58] 累计求和
来源：http://wh.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lr.shxzskj.cn

[Q59] 分组内累计
来源：http://qd.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sm.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://sn.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vo.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mq.newstarts.cn

[Q61] 移动平均
来源：http://ns.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hs.yuntaijiaju.cn

[Q62] 分组占比
来源：http://bw.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lr.shxzukj.cn

[Q63] 开启事务
来源：http://ny.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yt.yuntaijiaju.cn

[Q64] 提交事务
来源：http://lw.yuntaijiaju.cn

COMMIT;
来源：http://hb.newstarts.cn

[Q65] 回滚事务
来源：http://ll.chemitech.net.cn

ROLLBACK;
来源：http://tf.bjjhwx.cn

[Q66] 行锁查询
来源：http://uk.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ri.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://cj.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lg.huanxung.cn

[Q68] 保存点
来源：http://dh.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://cl.521024.cn

ROLLBACK TO sp1;
来源：http://ey.shxzskj.cn

[Q69] 查看执行计划
来源：http://jh.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zm.521024.cn

[Q70] 更新统计信息
来源：http://fe.bjjhwx.cn

ANALYZE TABLE users;
来源：http://kk.asd995.cn

[Q71] 查看建表语句
来源：http://dh.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uz.asd995.cn

[Q72] 查看索引
来源：http://ni.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://ry.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://cn.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ao.colortex.cn

[Q74] 强制使用索引
来源：http://ed.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kk.haigaiapp.cn

[Q75] 日期格式化
来源：http://ty.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ka.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ig.jianghongdianzi.cn

[Q76] 按天统计
来源：http://qf.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sy.yuntaijiaju.cn

[Q77] 时间加减
来源：http://fu.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bo.szxytkj.cn

[Q78] 当前时间
来源：http://lm.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lv.newstarts.cn

[Q79] 字符串拼接
来源：http://sw.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gc.nicolike.cn

[Q80] 字符串截取
来源：http://qa.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mt.asd995.cn

[Q81] 字符串替换
来源：http://yw.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ed.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://vf.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jr.wgjwhj.cn

[Q83] 大小写转换
来源：http://tl.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mw.szsharing.cn

[Q84] 去除首尾空格
来源：http://gh.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://gi.nicolike.cn

[Q85] 数值取整
来源：http://ok.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ls.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://fz.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nl.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://oj.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rd.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://cl.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://my.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wd.newstarts.cn

[Q89] 判断表是否存在
来源：http://tc.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zo.chemitech.net.cn

[Q90] 生成序号列
来源：http://dw.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://um.shtwfgs.cn

================================================================================
来源：http://ro.haigaiapp.cn

R. Bash 专题
来源：http://yh.521024.cn

================================================================================
来源：http://zq.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://no.haigaiapp.cn

#!/usr/bin/env bash
来源：http://lw.szxytkj.cn

set -euo pipefail
来源：http://zy.newstarts.cn

[R02] 变量赋值与使用
来源：http://op.lnxyls.cn

name="Tom"; echo "$name"
来源：http://bq.shxzukj.cn

[R03] 只读变量
来源：http://av.shtwfgs.cn

readonly PI=3.14
来源：http://jy.szsharing.cn

[R04] 位置参数
来源：http://ke.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mb.wgjwhj.cn

[R05] 参数默认值
来源：http://jz.huixinmuqiang.cn

name="${1:-default}"
来源：http://gw.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://ap.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nf.huixinmuqiang.cn

[R07] if 判断文件
来源：http://pd.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dj.9csxet.cn

[R08] 数值比较
来源：http://vl.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://co.panjiajie.cn

[R09] 字符串比较
来源：http://rd.huanxung.cn


<!-- 参考信息 -->
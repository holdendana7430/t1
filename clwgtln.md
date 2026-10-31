代发 wailian999

TS:   crypto.randomUUID()
来源：http://wj.521024.cn

Java: UUID.randomUUID().toString()
来源：http://bq.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://su.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://yz.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://bd.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://dr.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ux.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vo.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fm.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lp.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ww.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gu.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jr.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ds.panjiajie.cn

[P03] 生成短随机字符串
来源：http://kf.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tc.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jn.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wu.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zl.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ot.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iu.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mm.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lk.bookmarksfly.cn

[P04] 求长度
来源：http://xk.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ha.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://no.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ik.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pp.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://qe.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://pu.newstarts.cn

Ruby: x.length;  x.size
来源：http://wb.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wp.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://oz.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://il.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://li.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uz.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://px.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ic.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pn.hnjuh.cn

Ruby: a == b
来源：http://go.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tt.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bd.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wm.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://yj.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kt.panjiajie.cn

TS:   if (x == null) {}
来源：http://td.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ju.asd995.cn

Go:   if x == nil {}
来源：http://eu.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wp.bjjhwx.cn

C#:   if (x is null) {}
来源：http://mt.nicolike.cn

[P07] 防抖与节流
来源：http://iz.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hs.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://fz.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ts.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ct.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ol.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rz.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ee.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eu.newstarts.cn

[P08] 处理浮点精度问题
来源：http://ui.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hr.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ns.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eo.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pi.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pq.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kf.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ej.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vq.nszjky.cn

================================================================================
来源：http://ji.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://il.huixiangedu.cn

================================================================================
来源：http://kp.shxzukj.cn

[Q01] 创建表
来源：http://hc.asd995.cn

CREATE TABLE users (
来源：http://pb.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uk.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://au.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://yf.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cn.lnxyls.cn

);
来源：http://sl.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://mf.wgjwhj.cn

CREATE TABLE orders (
来源：http://za.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sl.9csxet.cn

user_id INT NOT NULL,
来源：http://or.521024.cn

amount DECIMAL(10, 2),
来源：http://mx.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ve.jianghongdianzi.cn

);
来源：http://jl.nicolike.cn

[Q03] 增加列
来源：http://hs.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gi.shxzskj.cn

[Q04] 修改列类型
来源：http://ye.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vn.szxytkj.cn

[Q05] 重命名列
来源：http://dh.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wn.nicolike.cn

[Q06] 删除列
来源：http://tl.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wd.521024.cn

[Q07] 删除表
来源：http://bw.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://cj.jctech888.com.cn

[Q08] 创建普通索引
来源：http://do.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ti.lnxyls.cn

[Q09] 创建唯一索引
来源：http://oa.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ex.haigaiapp.cn

[Q10] 插入单行
来源：http://tp.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lk.bjjhwx.cn

[Q11] 一次插入多行
来源：http://oi.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ep.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://ww.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nw.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ab.szxytkj.cn

[Q13] 忽略重复插入
来源：http://gr.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://th.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://dq.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://co.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wh.521024.cn

[Q15] 查询全部
来源：http://jb.hahajie.cn

SELECT * FROM users;
来源：http://jj.gzmigu.cn

[Q16] 查询指定列
来源：http://aa.shxzskj.cn

SELECT id, name FROM users;
来源：http://lo.newstarts.cn

[Q17] 条件查询
来源：http://of.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bb.muxihuayi.cn

[Q18] 模糊匹配
来源：http://xf.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oa.panjiajie.cn

[Q19] 范围查询
来源：http://nh.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dt.asd995.cn

[Q20] IN 列表
来源：http://lr.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lw.szxytkj.cn

[Q21] 空值判断
来源：http://uk.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pe.szsharing.cn

[Q22] 排序
来源：http://dx.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xy.newstarts.cn

[Q23] 分页
来源：http://fx.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://te.szsharing.cn

[Q24] 去重
来源：http://vp.521024.cn

SELECT DISTINCT city FROM users;
来源：http://vh.521024.cn

[Q25] 只取前 N 条
来源：http://nh.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fd.hnjuh.cn

[Q26] 计数
来源：http://ac.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://ea.haigaiapp.cn

[Q27] 条件计数
来源：http://ew.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oe.lnxyls.cn

[Q28] 求和与平均
来源：http://gh.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rl.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://gl.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tp.lnxyls.cn

[Q30] 分组统计
来源：http://po.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tj.bjjhwx.cn

[Q31] 分组后过滤
来源：http://na.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ja.asd995.cn

[Q32] 分组拼接字符串
来源：http://ab.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wa.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dm.nszjky.cn

[Q33] 多列分组
来源：http://tk.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ev.asd995.cn

[Q34] 每组取第一条
来源：http://rf.huixiangedu.cn

SELECT * FROM (
来源：http://pi.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yx.newstarts.cn

) t WHERE rn = 1;
来源：http://ar.nicolike.cn

[Q35] 内连接
来源：http://xl.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ej.szsharing.cn

[Q36] 左连接
来源：http://vx.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sm.gzmigu.cn

[Q37] 右连接
来源：http://mw.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mn.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dk.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://du.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://tt.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tj.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ka.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oa.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mn.huixinmuqiang.cn

[Q41] 多表连接
来源：http://oa.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pa.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://ou.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://ju.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://pr.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://fq.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kk.shxzskj.cn

[Q43] 标量子查询
来源：http://si.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://es.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://wp.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hf.521024.cn

[Q45] EXISTS 判断存在
来源：http://jf.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ke.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ii.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jg.panjiajie.cn

[Q47] 与平均值比较
来源：http://va.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kd.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://ot.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fm.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://vm.asd995.cn

[Q49] 更新单行
来源：http://gf.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eo.asd995.cn

[Q50] 批量更新
来源：http://wz.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eh.yuexingan06.cn

[Q51] 用子查询更新
来源：http://bv.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ye.lnxyls.cn

[Q52] 删除指定行
来源：http://jk.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://lf.haigaiapp.cn

[Q53] 按条件删除
来源：http://dd.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jd.chemitech.net.cn

[Q54] 清空表
来源：http://un.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://ho.nszjky.cn

[Q55] 排名（并列占位）
来源：http://cj.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zm.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://tf.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pj.muxihuayi.cn

[Q57] 行号
来源：http://sg.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kb.yuntaijiaju.cn

[Q58] 累计求和
来源：http://ba.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gk.9csxet.cn

[Q59] 分组内累计
来源：http://jp.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tb.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://gl.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pc.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vt.jianghongdianzi.cn

[Q61] 移动平均
来源：http://bq.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bm.haigaiapp.cn

[Q62] 分组占比
来源：http://ch.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ae.hahajie.cn

[Q63] 开启事务
来源：http://go.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ei.yuntaijiaju.cn

[Q64] 提交事务
来源：http://bg.szxytkj.cn

COMMIT;
来源：http://er.szsharing.cn

[Q65] 回滚事务
来源：http://bs.jianghongdianzi.cn

ROLLBACK;
来源：http://qd.nszjky.cn

[Q66] 行锁查询
来源：http://hc.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ra.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://xw.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qp.newstarts.cn

[Q68] 保存点
来源：http://vz.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://hq.lnxyls.cn

ROLLBACK TO sp1;
来源：http://zn.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://bc.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hn.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://zv.shxzukj.cn

ANALYZE TABLE users;
来源：http://dq.wgjwhj.cn

[Q71] 查看建表语句
来源：http://sx.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ws.shtwfgs.cn

[Q72] 查看索引
来源：http://si.lnxyls.cn

SHOW INDEX FROM users;
来源：http://rh.colortex.cn

[Q73] 查看表状态
来源：http://dx.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mm.chemitech.net.cn

[Q74] 强制使用索引
来源：http://kk.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dq.hnjuh.cn

[Q75] 日期格式化
来源：http://pb.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zl.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tf.newstarts.cn

[Q76] 按天统计
来源：http://ir.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bv.hahajie.cn

[Q77] 时间加减
来源：http://sh.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ou.hahajie.cn

[Q78] 当前时间
来源：http://fs.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ry.shxzukj.cn

[Q79] 字符串拼接
来源：http://ii.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vo.shxzskj.cn

[Q80] 字符串截取
来源：http://qj.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sy.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://hg.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://es.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://ih.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fl.szsharing.cn

[Q83] 大小写转换
来源：http://mm.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rx.colortex.cn

[Q84] 去除首尾空格
来源：http://zj.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://wb.colortex.cn

[Q85] 数值取整
来源：http://lv.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vg.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://bu.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qy.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://tp.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vy.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://dq.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jl.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ze.9csxet.cn

[Q89] 判断表是否存在
来源：http://ed.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ol.nicolike.cn

[Q90] 生成序号列
来源：http://pc.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ak.hnjuh.cn

================================================================================
来源：http://oa.asd995.cn

R. Bash 专题
来源：http://xb.newstarts.cn

================================================================================
来源：http://qa.nszjky.cn

[R01] shebang 与严格模式
来源：http://ob.yuexingan06.cn

#!/usr/bin/env bash
来源：http://sz.nicolike.cn

set -euo pipefail
来源：http://ba.nicolike.cn

[R02] 变量赋值与使用
来源：http://bo.szxytkj.cn

name="Tom"; echo "$name"
来源：http://ak.hnjuh.cn

[R03] 只读变量
来源：http://xk.yuexingan06.cn

readonly PI=3.14
来源：http://ku.szsharing.cn

[R04] 位置参数
来源：http://la.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://at.huanxung.cn

[R05] 参数默认值
来源：http://rk.lnxyls.cn

name="${1:-default}"
来源：http://di.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://uw.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aq.szsharing.cn

[R07] if 判断文件
来源：http://gu.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mj.9csxet.cn

[R08] 数值比较
来源：http://oo.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sc.chemitech.net.cn

[R09] 字符串比较
来源：http://sy.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://za.shxzskj.cn

[R10] 正则匹配
来源：http://py.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tr.shxzskj.cn

[R11] case 多分支
来源：http://zh.haigaiapp.cn


<!-- 参考信息 -->
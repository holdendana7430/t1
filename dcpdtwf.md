代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://os.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://wh.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gr.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sq.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rm.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dv.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rx.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pa.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oq.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mt.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://vc.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://js.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://re.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vs.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://re.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bl.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xq.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ri.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ve.nicolike.cn

[P04] 求长度
来源：http://im.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ex.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pi.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yc.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vm.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://gd.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://ts.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://if.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://te.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://ss.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kj.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lj.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bm.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ro.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fh.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://de.9csxet.cn

Ruby: a == b
来源：http://kx.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mh.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wh.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fa.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://gz.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uk.gzmigu.cn

TS:   if (x == null) {}
来源：http://it.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qu.huanxung.cn

Go:   if x == nil {}
来源：http://xx.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cm.9csxet.cn

C#:   if (x is null) {}
来源：http://bt.shxzskj.cn

[P07] 防抖与节流
来源：http://hm.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sk.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://gy.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gl.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://le.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pa.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uh.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ht.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://me.szsharing.cn

[P08] 处理浮点精度问题
来源：http://mr.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rf.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fi.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ms.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cm.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gr.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yq.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://of.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://za.newstarts.cn

================================================================================
来源：http://vw.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dh.szxytkj.cn

================================================================================
来源：http://fj.szsharing.cn

[Q01] 创建表
来源：http://ig.nszjky.cn

CREATE TABLE users (
来源：http://tq.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sa.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://jm.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://hw.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ur.bjjhwx.cn

);
来源：http://xu.nicolike.cn

[Q02] 创建带外键的表
来源：http://mb.huanxung.cn

CREATE TABLE orders (
来源：http://om.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uo.wgjwhj.cn

user_id INT NOT NULL,
来源：http://fp.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://le.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pi.lnxyls.cn

);
来源：http://ia.hahajie.cn

[Q03] 增加列
来源：http://xv.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hp.yuexingan06.cn

[Q04] 修改列类型
来源：http://le.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yp.szsharing.cn

[Q05] 重命名列
来源：http://pe.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kg.newstarts.cn

[Q06] 删除列
来源：http://dg.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mb.yuexingan06.cn

[Q07] 删除表
来源：http://qa.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://io.wgjwhj.cn

[Q08] 创建普通索引
来源：http://xs.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rr.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://fe.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ri.szsharing.cn

[Q10] 插入单行
来源：http://vk.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yz.huanxung.cn

[Q11] 一次插入多行
来源：http://xs.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://io.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://mj.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ec.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zh.newstarts.cn

[Q13] 忽略重复插入
来源：http://ox.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dn.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://tx.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eg.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zz.newstarts.cn

[Q15] 查询全部
来源：http://ww.yuntaijiaju.cn

SELECT * FROM users;
来源：http://aq.szxytkj.cn

[Q16] 查询指定列
来源：http://ft.jctech888.com.cn

SELECT id, name FROM users;
来源：http://rl.jctech888.com.cn

[Q17] 条件查询
来源：http://wj.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yn.szsharing.cn

[Q18] 模糊匹配
来源：http://it.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rq.huixiangedu.cn

[Q19] 范围查询
来源：http://uo.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zm.bookmarksfly.cn

[Q20] IN 列表
来源：http://st.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://je.panjiajie.cn

[Q21] 空值判断
来源：http://uu.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qk.jianghongdianzi.cn

[Q22] 排序
来源：http://nj.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ht.jianghongdianzi.cn

[Q23] 分页
来源：http://ax.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zb.muxihuayi.cn

[Q24] 去重
来源：http://qj.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://tc.521024.cn

[Q25] 只取前 N 条
来源：http://pb.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eb.jctech888.com.cn

[Q26] 计数
来源：http://zj.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://sl.jianghongdianzi.cn

[Q27] 条件计数
来源：http://xw.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jg.yuexingan06.cn

[Q28] 求和与平均
来源：http://er.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://je.huixiangedu.cn

[Q29] 最大最小值
来源：http://yh.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yu.jianghongdianzi.cn

[Q30] 分组统计
来源：http://jd.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zs.hnjuh.cn

[Q31] 分组后过滤
来源：http://na.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://au.nszjky.cn

[Q32] 分组拼接字符串
来源：http://kq.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gj.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dq.nszjky.cn

[Q33] 多列分组
来源：http://mb.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ah.jctech888.com.cn

[Q34] 每组取第一条
来源：http://mr.shtwfgs.cn

SELECT * FROM (
来源：http://ln.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pe.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://mx.asd995.cn

[Q35] 内连接
来源：http://sr.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uw.9csxet.cn

[Q36] 左连接
来源：http://xg.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://st.newstarts.cn

[Q37] 右连接
来源：http://az.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bx.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sz.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qa.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://dt.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yf.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://el.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qg.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ot.yuexingan06.cn

[Q41] 多表连接
来源：http://ci.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ip.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://sn.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://bi.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://jr.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://uy.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://df.nicolike.cn

[Q43] 标量子查询
来源：http://wr.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ea.huanxung.cn

[Q44] IN 子查询
来源：http://zd.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://la.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://pi.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qo.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kh.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jr.shxzskj.cn

[Q47] 与平均值比较
来源：http://iq.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jm.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://uz.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kg.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://rl.shxzskj.cn

[Q49] 更新单行
来源：http://uu.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rt.colortex.cn

[Q50] 批量更新
来源：http://pm.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://og.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://js.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jh.wgjwhj.cn

[Q52] 删除指定行
来源：http://yi.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://mx.gzmigu.cn

[Q53] 按条件删除
来源：http://hd.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://es.huixinmuqiang.cn

[Q54] 清空表
来源：http://nb.521024.cn

TRUNCATE TABLE logs;
来源：http://tu.hahajie.cn

[Q55] 排名（并列占位）
来源：http://mq.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gz.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://mw.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gq.szxytkj.cn

[Q57] 行号
来源：http://qq.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rf.hahajie.cn

[Q58] 累计求和
来源：http://ar.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ny.bjjhwx.cn

[Q59] 分组内累计
来源：http://bi.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eb.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://ez.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://um.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wf.newstarts.cn

[Q61] 移动平均
来源：http://cq.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tg.haigaiapp.cn

[Q62] 分组占比
来源：http://ix.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kf.bjjhwx.cn

[Q63] 开启事务
来源：http://ar.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rh.colortex.cn

[Q64] 提交事务
来源：http://rr.wgjwhj.cn

COMMIT;
来源：http://ab.nszjky.cn

[Q65] 回滚事务
来源：http://wb.asd995.cn

ROLLBACK;
来源：http://di.lnxyls.cn

[Q66] 行锁查询
来源：http://ry.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ge.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://js.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://in.hnjuh.cn

[Q68] 保存点
来源：http://lr.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ss.shxzskj.cn

ROLLBACK TO sp1;
来源：http://cy.chemitech.net.cn

[Q69] 查看执行计划
来源：http://ou.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ve.9csxet.cn

[Q70] 更新统计信息
来源：http://np.nszjky.cn

ANALYZE TABLE users;
来源：http://se.lnxyls.cn

[Q71] 查看建表语句
来源：http://db.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ay.haigaiapp.cn

[Q72] 查看索引
来源：http://jt.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://bb.9csxet.cn

[Q73] 查看表状态
来源：http://ps.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lg.hahajie.cn

[Q74] 强制使用索引
来源：http://wy.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kb.hahajie.cn

[Q75] 日期格式化
来源：http://jv.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ha.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ru.newstarts.cn

[Q76] 按天统计
来源：http://cj.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xr.shtwfgs.cn

[Q77] 时间加减
来源：http://pm.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sr.panjiajie.cn

[Q78] 当前时间
来源：http://li.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ph.asd995.cn

[Q79] 字符串拼接
来源：http://vx.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://np.hahajie.cn

[Q80] 字符串截取
来源：http://tq.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ew.lnxyls.cn

[Q81] 字符串替换
来源：http://iv.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mi.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://tg.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://na.haigaiapp.cn

[Q83] 大小写转换
来源：http://cw.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fu.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://zr.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://ha.yuexingan06.cn

[Q85] 数值取整
来源：http://qh.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://re.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://pl.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gd.colortex.cn

[Q87] JSON 字段做条件
来源：http://wb.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tk.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://kt.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uu.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cq.colortex.cn

[Q89] 判断表是否存在
来源：http://td.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wx.bookmarksfly.cn

[Q90] 生成序号列
来源：http://qr.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tp.huixinmuqiang.cn

================================================================================
来源：http://cm.szsharing.cn

R. Bash 专题
来源：http://pt.colortex.cn

================================================================================
来源：http://er.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://va.nszjky.cn

#!/usr/bin/env bash
来源：http://hw.gzmigu.cn

set -euo pipefail
来源：http://tf.newstarts.cn

[R02] 变量赋值与使用
来源：http://ul.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://yr.jctech888.com.cn

[R03] 只读变量
来源：http://dz.gzmigu.cn

readonly PI=3.14
来源：http://tq.szxytkj.cn

[R04] 位置参数
来源：http://lx.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mw.gzmigu.cn

[R05] 参数默认值
来源：http://wy.nicolike.cn

name="${1:-default}"
来源：http://re.colortex.cn

[R06] 判断命令是否存在
来源：http://xg.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pf.yuexingan06.cn

[R07] if 判断文件
来源：http://fm.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hw.haigaiapp.cn

[R08] 数值比较
来源：http://vy.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ru.muxihuayi.cn

[R09] 字符串比较
来源：http://vk.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gd.shtwfgs.cn

[R10] 正则匹配
来源：http://bx.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dz.newstarts.cn

[R11] case 多分支
来源：http://mi.jianghongdianzi.cn

case "$1" in
来源：http://mp.nicolike.cn

start) echo "启动" ;;
来源：http://gi.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://iz.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://ph.nicolike.cn


<!-- 参考信息 -->
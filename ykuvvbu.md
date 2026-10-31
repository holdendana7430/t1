代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://jv.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://sx.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dl.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xb.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gw.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ww.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zi.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://la.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://co.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zm.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://jj.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xn.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vd.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://al.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dj.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wy.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ao.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ea.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nr.yuexingan06.cn

[P04] 求长度
来源：http://fe.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nm.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ja.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ni.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cm.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://lv.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://rt.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://lv.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jb.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://ga.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qi.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cn.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ph.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jk.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nd.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qq.colortex.cn

Ruby: a == b
来源：http://ta.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fl.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nb.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mq.asd995.cn

PHP:  if (empty($x)) {}
来源：http://lz.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kh.nszjky.cn

TS:   if (x == null) {}
来源：http://fu.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xz.shxzukj.cn

Go:   if x == nil {}
来源：http://jq.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://da.huixiangedu.cn

C#:   if (x is null) {}
来源：http://re.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://ul.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tc.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://nn.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xn.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ni.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kp.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ut.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ho.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nw.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://qb.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mx.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://av.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wb.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fi.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lq.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jw.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fl.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tn.wgjwhj.cn

================================================================================
来源：http://nb.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ns.shtwfgs.cn

================================================================================
来源：http://ez.haigaiapp.cn

[Q01] 创建表
来源：http://ia.nszjky.cn

CREATE TABLE users (
来源：http://bl.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vr.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://yu.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://di.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hb.huixiangedu.cn

);
来源：http://bb.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://bo.shtwfgs.cn

CREATE TABLE orders (
来源：http://cn.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hi.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://ft.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://pi.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ai.9csxet.cn

);
来源：http://gx.521024.cn

[Q03] 增加列
来源：http://ey.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://az.huixiangedu.cn

[Q04] 修改列类型
来源：http://fp.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lp.panjiajie.cn

[Q05] 重命名列
来源：http://hy.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://di.nicolike.cn

[Q06] 删除列
来源：http://sk.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ot.lnxyls.cn

[Q07] 删除表
来源：http://ij.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://zf.nicolike.cn

[Q08] 创建普通索引
来源：http://pe.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fe.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://px.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vy.hnjuh.cn

[Q10] 插入单行
来源：http://uc.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://za.hnjuh.cn

[Q11] 一次插入多行
来源：http://pc.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mc.asd995.cn

[Q12] 插入后取自增 ID
来源：http://gg.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ps.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fl.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://dh.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mb.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://nl.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://so.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bo.shtwfgs.cn

[Q15] 查询全部
来源：http://na.bookmarksfly.cn

SELECT * FROM users;
来源：http://vv.jctech888.com.cn

[Q16] 查询指定列
来源：http://bq.521024.cn

SELECT id, name FROM users;
来源：http://aa.wgjwhj.cn

[Q17] 条件查询
来源：http://nq.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mh.521024.cn

[Q18] 模糊匹配
来源：http://vx.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lz.shtwfgs.cn

[Q19] 范围查询
来源：http://ew.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://am.shtwfgs.cn

[Q20] IN 列表
来源：http://jd.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.szsharing.cn

[Q21] 空值判断
来源：http://be.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yv.bookmarksfly.cn

[Q22] 排序
来源：http://ga.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wn.521024.cn

[Q23] 分页
来源：http://tz.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ob.shxzukj.cn

[Q24] 去重
来源：http://hb.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://re.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://eu.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rp.jianghongdianzi.cn

[Q26] 计数
来源：http://qs.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://zc.shtwfgs.cn

[Q27] 条件计数
来源：http://qw.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://se.haigaiapp.cn

[Q28] 求和与平均
来源：http://rt.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hn.shtwfgs.cn

[Q29] 最大最小值
来源：http://kf.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pr.jctech888.com.cn

[Q30] 分组统计
来源：http://jk.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ed.muxihuayi.cn

[Q31] 分组后过滤
来源：http://xf.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ne.hahajie.cn

[Q32] 分组拼接字符串
来源：http://if.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zg.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mb.bookmarksfly.cn

[Q33] 多列分组
来源：http://qx.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nd.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://uh.9csxet.cn

SELECT * FROM (
来源：http://lh.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rx.jctech888.com.cn

) t WHERE rn = 1;
来源：http://al.shxzskj.cn

[Q35] 内连接
来源：http://nk.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qd.huixiangedu.cn

[Q36] 左连接
来源：http://js.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jw.9csxet.cn

[Q37] 右连接
来源：http://fo.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pp.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ff.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ah.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://qu.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ja.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nr.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ud.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://el.lnxyls.cn

[Q41] 多表连接
来源：http://jp.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qm.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://st.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://sv.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://ci.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://bn.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yv.chemitech.net.cn

[Q43] 标量子查询
来源：http://xm.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wv.nszjky.cn

[Q44] IN 子查询
来源：http://en.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://au.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://ob.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://li.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gw.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tf.wgjwhj.cn

[Q47] 与平均值比较
来源：http://sn.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uy.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://wb.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xy.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://kq.bookmarksfly.cn

[Q49] 更新单行
来源：http://br.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://us.hnjuh.cn

[Q50] 批量更新
来源：http://mn.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zs.bjjhwx.cn

[Q51] 用子查询更新
来源：http://cz.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mb.hahajie.cn

[Q52] 删除指定行
来源：http://ip.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://tc.haigaiapp.cn

[Q53] 按条件删除
来源：http://fv.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://co.lnxyls.cn

[Q54] 清空表
来源：http://te.9csxet.cn

TRUNCATE TABLE logs;
来源：http://gy.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://ft.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fc.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://lr.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qd.bookmarksfly.cn

[Q57] 行号
来源：http://oc.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kb.yuntaijiaju.cn

[Q58] 累计求和
来源：http://wv.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xt.9csxet.cn

[Q59] 分组内累计
来源：http://gs.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://es.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://xq.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zv.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xo.huixiangedu.cn

[Q61] 移动平均
来源：http://gw.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fj.colortex.cn

[Q62] 分组占比
来源：http://ah.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zy.lnxyls.cn

[Q63] 开启事务
来源：http://ks.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zx.hnjuh.cn

[Q64] 提交事务
来源：http://cg.shtwfgs.cn

COMMIT;
来源：http://md.wgjwhj.cn

[Q65] 回滚事务
来源：http://ws.shxzukj.cn

ROLLBACK;
来源：http://kr.newstarts.cn

[Q66] 行锁查询
来源：http://wf.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mq.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://cs.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jd.muxihuayi.cn

[Q68] 保存点
来源：http://bf.colortex.cn

SAVEPOINT sp1;
来源：http://lp.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://rt.chemitech.net.cn

[Q69] 查看执行计划
来源：http://rz.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gq.shxzukj.cn

[Q70] 更新统计信息
来源：http://kz.szxytkj.cn

ANALYZE TABLE users;
来源：http://us.muxihuayi.cn

[Q71] 查看建表语句
来源：http://bv.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://px.newstarts.cn

[Q72] 查看索引
来源：http://dc.9csxet.cn

SHOW INDEX FROM users;
来源：http://nh.hahajie.cn

[Q73] 查看表状态
来源：http://cp.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ne.yuexingan06.cn

[Q74] 强制使用索引
来源：http://qz.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vo.shtwfgs.cn

[Q75] 日期格式化
来源：http://jz.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wd.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cz.huixiangedu.cn

[Q76] 按天统计
来源：http://ho.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wn.huixinmuqiang.cn

[Q77] 时间加减
来源：http://ys.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cy.bookmarksfly.cn

[Q78] 当前时间
来源：http://ps.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lo.shxzukj.cn

[Q79] 字符串拼接
来源：http://zu.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qk.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://ah.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://li.muxihuayi.cn

[Q81] 字符串替换
来源：http://zg.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qh.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://li.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ym.shxzskj.cn

[Q83] 大小写转换
来源：http://ns.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://df.gzmigu.cn

[Q84] 去除首尾空格
来源：http://wj.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://on.newstarts.cn

[Q85] 数值取整
来源：http://sm.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dj.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://hp.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jp.szsharing.cn

[Q87] JSON 字段做条件
来源：http://gr.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lg.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://wo.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lr.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jn.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://eo.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tp.bjjhwx.cn

[Q90] 生成序号列
来源：http://mj.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mp.jctech888.com.cn

================================================================================
来源：http://nb.hahajie.cn

R. Bash 专题
来源：http://lm.bookmarksfly.cn

================================================================================
来源：http://jl.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://jo.chemitech.net.cn

#!/usr/bin/env bash
来源：http://xd.shxzukj.cn

set -euo pipefail
来源：http://vw.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://wj.colortex.cn

name="Tom"; echo "$name"
来源：http://bq.lnxyls.cn

[R03] 只读变量
来源：http://xc.wgjwhj.cn

readonly PI=3.14
来源：http://ky.asd995.cn

[R04] 位置参数
来源：http://zm.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kr.huanxung.cn

[R05] 参数默认值
来源：http://mw.shxzskj.cn

name="${1:-default}"
来源：http://kh.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://qz.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fs.shxzukj.cn

[R07] if 判断文件
来源：http://uq.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kt.szsharing.cn

[R08] 数值比较
来源：http://ot.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://th.shtwfgs.cn

[R09] 字符串比较
来源：http://wx.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qa.jianghongdianzi.cn

[R10] 正则匹配
来源：http://mz.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cy.jianghongdianzi.cn

[R11] case 多分支
来源：http://oi.hahajie.cn

case "$1" in
来源：http://sg.asd995.cn

start) echo "启动" ;;
来源：http://gf.9csxet.cn

stop)  echo "停止" ;;
来源：http://js.nszjky.cn

*)     echo "未知命令" ;;
来源：http://xy.wgjwhj.cn


<!-- 参考信息 -->
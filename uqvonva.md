代发 wailian999

TS:   crypto.randomUUID()
来源：http://cw.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://yh.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://jq.asd995.cn

Ruby: SecureRandom.uuid
来源：http://em.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://hg.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://mi.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ye.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ge.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yd.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lj.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://su.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cf.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ke.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pk.szxytkj.cn

[P03] 生成短随机字符串
来源：http://fj.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vk.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aq.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fo.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uo.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ig.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aa.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://la.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://an.haigaiapp.cn

[P04] 求长度
来源：http://un.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kz.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jz.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://so.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://og.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://fw.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://fx.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://jw.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rs.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://fd.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ku.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://im.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nt.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ni.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ur.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rl.panjiajie.cn

Ruby: a == b
来源：http://wm.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cb.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yp.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qg.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://no.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ty.nicolike.cn

TS:   if (x == null) {}
来源：http://ql.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ih.newstarts.cn

Go:   if x == nil {}
来源：http://sn.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ns.asd995.cn

C#:   if (x is null) {}
来源：http://pg.jctech888.com.cn

[P07] 防抖与节流
来源：http://pz.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ji.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://ak.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ts.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qd.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ql.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mc.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ld.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kv.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://xk.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xx.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nq.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zy.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oc.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lu.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://me.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pd.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ru.jianghongdianzi.cn

================================================================================
来源：http://tz.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fu.szsharing.cn

================================================================================
来源：http://ga.shtwfgs.cn

[Q01] 创建表
来源：http://uk.bjjhwx.cn

CREATE TABLE users (
来源：http://ub.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pn.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://it.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://je.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dz.shtwfgs.cn

);
来源：http://ld.hahajie.cn

[Q02] 创建带外键的表
来源：http://qt.szsharing.cn

CREATE TABLE orders (
来源：http://ps.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vj.shtwfgs.cn

user_id INT NOT NULL,
来源：http://un.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://kh.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ph.nszjky.cn

);
来源：http://td.muxihuayi.cn

[Q03] 增加列
来源：http://tf.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://th.bjjhwx.cn

[Q04] 修改列类型
来源：http://ol.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ib.shxzskj.cn

[Q05] 重命名列
来源：http://mi.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://al.chemitech.net.cn

[Q06] 删除列
来源：http://gq.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ra.gzmigu.cn

[Q07] 删除表
来源：http://oz.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://rc.shxzukj.cn

[Q08] 创建普通索引
来源：http://dn.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ld.hnjuh.cn

[Q09] 创建唯一索引
来源：http://dd.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qr.jianghongdianzi.cn

[Q10] 插入单行
来源：http://kg.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lz.newstarts.cn

[Q11] 一次插入多行
来源：http://uk.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ds.521024.cn

[Q12] 插入后取自增 ID
来源：http://ut.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nh.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dm.hnjuh.cn

[Q13] 忽略重复插入
来源：http://eq.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://om.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://az.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yz.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rc.hnjuh.cn

[Q15] 查询全部
来源：http://cx.gzmigu.cn

SELECT * FROM users;
来源：http://mw.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://pb.gzmigu.cn

SELECT id, name FROM users;
来源：http://tm.lnxyls.cn

[Q17] 条件查询
来源：http://uk.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ci.chemitech.net.cn

[Q18] 模糊匹配
来源：http://lg.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nr.lnxyls.cn

[Q19] 范围查询
来源：http://mh.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cl.muxihuayi.cn

[Q20] IN 列表
来源：http://aa.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uj.colortex.cn

[Q21] 空值判断
来源：http://el.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://go.521024.cn

[Q22] 排序
来源：http://li.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lf.jianghongdianzi.cn

[Q23] 分页
来源：http://ta.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gv.bjjhwx.cn

[Q24] 去重
来源：http://ze.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://vt.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://ap.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tz.huanxung.cn

[Q26] 计数
来源：http://bd.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://tu.9csxet.cn

[Q27] 条件计数
来源：http://nj.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ru.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://ko.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ru.huixiangedu.cn

[Q29] 最大最小值
来源：http://bh.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fi.shxzskj.cn

[Q30] 分组统计
来源：http://tl.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wv.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://fb.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ib.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://vw.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cj.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kf.muxihuayi.cn

[Q33] 多列分组
来源：http://ci.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hu.shxzskj.cn

[Q34] 每组取第一条
来源：http://ua.hahajie.cn

SELECT * FROM (
来源：http://jc.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oi.colortex.cn

) t WHERE rn = 1;
来源：http://yg.jianghongdianzi.cn

[Q35] 内连接
来源：http://st.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rq.shtwfgs.cn

[Q36] 左连接
来源：http://fd.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ud.panjiajie.cn

[Q37] 右连接
来源：http://nl.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ko.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vi.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vb.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://md.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cf.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sx.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://px.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zf.9csxet.cn

[Q41] 多表连接
来源：http://ho.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pv.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://de.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://xu.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://zh.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://bj.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zw.szsharing.cn

[Q43] 标量子查询
来源：http://gs.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ez.bjjhwx.cn

[Q44] IN 子查询
来源：http://aw.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ud.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://rs.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ec.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mb.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ig.huanxung.cn

[Q47] 与平均值比较
来源：http://yp.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wa.asd995.cn

[Q48] CTE 公用表表达式
来源：http://vk.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tu.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://wc.hahajie.cn

[Q49] 更新单行
来源：http://un.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wj.bjjhwx.cn

[Q50] 批量更新
来源：http://hr.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vp.bjjhwx.cn

[Q51] 用子查询更新
来源：http://xg.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ag.szxytkj.cn

[Q52] 删除指定行
来源：http://ch.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://yg.chemitech.net.cn

[Q53] 按条件删除
来源：http://rg.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xl.nszjky.cn

[Q54] 清空表
来源：http://qm.huanxung.cn

TRUNCATE TABLE logs;
来源：http://bv.nicolike.cn

[Q55] 排名（并列占位）
来源：http://es.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zj.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://vn.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qq.huixiangedu.cn

[Q57] 行号
来源：http://go.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cp.szsharing.cn

[Q58] 累计求和
来源：http://rm.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jb.panjiajie.cn

[Q59] 分组内累计
来源：http://xb.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jn.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ln.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ul.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ry.huanxung.cn

[Q61] 移动平均
来源：http://zg.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pk.jianghongdianzi.cn

[Q62] 分组占比
来源：http://qg.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yn.shxzukj.cn

[Q63] 开启事务
来源：http://wu.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gd.newstarts.cn

[Q64] 提交事务
来源：http://lh.521024.cn

COMMIT;
来源：http://dc.asd995.cn

[Q65] 回滚事务
来源：http://pz.szxytkj.cn

ROLLBACK;
来源：http://ah.lnxyls.cn

[Q66] 行锁查询
来源：http://kz.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gb.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://ng.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://am.bjjhwx.cn

[Q68] 保存点
来源：http://tt.gzmigu.cn

SAVEPOINT sp1;
来源：http://di.szsharing.cn

ROLLBACK TO sp1;
来源：http://eg.panjiajie.cn

[Q69] 查看执行计划
来源：http://ea.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kq.newstarts.cn

[Q70] 更新统计信息
来源：http://if.jctech888.com.cn

ANALYZE TABLE users;
来源：http://vg.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://tj.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sg.yuntaijiaju.cn

[Q72] 查看索引
来源：http://ci.gzmigu.cn

SHOW INDEX FROM users;
来源：http://wt.newstarts.cn

[Q73] 查看表状态
来源：http://sw.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wi.hahajie.cn

[Q74] 强制使用索引
来源：http://vr.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uu.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://bk.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://st.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ua.521024.cn

[Q76] 按天统计
来源：http://vu.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vm.shxzukj.cn

[Q77] 时间加减
来源：http://qk.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hh.gzmigu.cn

[Q78] 当前时间
来源：http://aj.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qo.szxytkj.cn

[Q79] 字符串拼接
来源：http://zq.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vp.gzmigu.cn

[Q80] 字符串截取
来源：http://ze.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ou.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://vq.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lp.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://pz.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tc.nszjky.cn

[Q83] 大小写转换
来源：http://yp.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sh.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://tk.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://rm.szxytkj.cn

[Q85] 数值取整
来源：http://ri.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jf.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ud.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ed.9csxet.cn

[Q87] JSON 字段做条件
来源：http://gl.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://me.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://uw.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ri.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zt.lnxyls.cn

[Q89] 判断表是否存在
来源：http://me.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ql.lnxyls.cn

[Q90] 生成序号列
来源：http://gr.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://dn.yuntaijiaju.cn

R. Bash 专题
来源：http://yq.bookmarksfly.cn

================================================================================
来源：http://xk.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ul.jctech888.com.cn

#!/usr/bin/env bash
来源：http://ev.shtwfgs.cn

set -euo pipefail
来源：http://ks.colortex.cn

[R02] 变量赋值与使用
来源：http://xa.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://av.yuexingan06.cn

[R03] 只读变量
来源：http://ci.hnjuh.cn

readonly PI=3.14
来源：http://hs.gzmigu.cn

[R04] 位置参数
来源：http://vv.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sp.yuntaijiaju.cn

[R05] 参数默认值
来源：http://pb.chemitech.net.cn

name="${1:-default}"
来源：http://oc.lnxyls.cn

[R06] 判断命令是否存在
来源：http://gz.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wr.shxzskj.cn

[R07] if 判断文件
来源：http://qf.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fn.szsharing.cn

[R08] 数值比较
来源：http://fi.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kp.hnjuh.cn

[R09] 字符串比较
来源：http://zv.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sr.haigaiapp.cn

[R10] 正则匹配
来源：http://tc.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vz.newstarts.cn

[R11] case 多分支
来源：http://ul.panjiajie.cn


<!-- 参考信息 -->
代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://kv.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://jz.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ym.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hy.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ph.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://he.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tr.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sn.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gz.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jt.shxzskj.cn

[P03] 生成短随机字符串
来源：http://ke.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xx.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lz.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pf.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qf.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kt.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sg.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nd.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lr.wgjwhj.cn

[P04] 求长度
来源：http://pm.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://se.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://az.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tg.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mr.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://bp.nicolike.cn

Go:   len(arr);  len(m)
来源：http://ji.nszjky.cn

Ruby: x.length;  x.size
来源：http://pb.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lw.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://xs.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qy.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rr.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gf.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ar.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ti.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ww.szxytkj.cn

Ruby: a == b
来源：http://ar.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ly.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://in.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cz.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://pd.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dc.newstarts.cn

TS:   if (x == null) {}
来源：http://vy.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jp.bookmarksfly.cn

Go:   if x == nil {}
来源：http://jh.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bq.hnjuh.cn

C#:   if (x is null) {}
来源：http://il.haigaiapp.cn

[P07] 防抖与节流
来源：http://te.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kg.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://xi.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gj.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hx.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mb.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mc.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dd.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xk.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://pg.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cw.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dw.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fw.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pl.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ga.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gl.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wt.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nm.szsharing.cn

================================================================================
来源：http://xn.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://im.haigaiapp.cn

================================================================================
来源：http://tf.hnjuh.cn

[Q01] 创建表
来源：http://fm.huixiangedu.cn

CREATE TABLE users (
来源：http://lr.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kd.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://pg.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://vx.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://by.yuexingan06.cn

);
来源：http://nc.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://ax.szsharing.cn

CREATE TABLE orders (
来源：http://ow.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uj.huixiangedu.cn

user_id INT NOT NULL,
来源：http://am.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://fd.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gp.muxihuayi.cn

);
来源：http://fz.chemitech.net.cn

[Q03] 增加列
来源：http://eo.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://co.huanxung.cn

[Q04] 修改列类型
来源：http://yg.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hf.muxihuayi.cn

[Q05] 重命名列
来源：http://ih.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rm.hahajie.cn

[Q06] 删除列
来源：http://pc.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://de.panjiajie.cn

[Q07] 删除表
来源：http://jt.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://kc.hahajie.cn

[Q08] 创建普通索引
来源：http://ks.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nh.shxzskj.cn

[Q09] 创建唯一索引
来源：http://we.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fo.szsharing.cn

[Q10] 插入单行
来源：http://ik.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://be.hahajie.cn

[Q11] 一次插入多行
来源：http://ej.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zt.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://fe.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cb.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uv.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://jd.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ap.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://gh.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jy.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qr.panjiajie.cn

[Q15] 查询全部
来源：http://yy.shxzskj.cn

SELECT * FROM users;
来源：http://tj.haigaiapp.cn

[Q16] 查询指定列
来源：http://sq.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://fe.huanxung.cn

[Q17] 条件查询
来源：http://rj.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vk.gzmigu.cn

[Q18] 模糊匹配
来源：http://vf.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mj.huixiangedu.cn

[Q19] 范围查询
来源：http://os.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lj.shtwfgs.cn

[Q20] IN 列表
来源：http://vz.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xs.colortex.cn

[Q21] 空值判断
来源：http://sl.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bx.hnjuh.cn

[Q22] 排序
来源：http://hq.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mx.huixinmuqiang.cn

[Q23] 分页
来源：http://au.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fc.shxzskj.cn

[Q24] 去重
来源：http://ni.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://hv.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://ip.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kw.huanxung.cn

[Q26] 计数
来源：http://mg.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://kr.bookmarksfly.cn

[Q27] 条件计数
来源：http://ci.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://of.huanxung.cn

[Q28] 求和与平均
来源：http://uv.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vj.shtwfgs.cn

[Q29] 最大最小值
来源：http://rh.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mr.huanxung.cn

[Q30] 分组统计
来源：http://of.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hd.bjjhwx.cn

[Q31] 分组后过滤
来源：http://gd.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xf.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://ob.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pg.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bf.shtwfgs.cn

[Q33] 多列分组
来源：http://ed.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fw.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://gc.chemitech.net.cn

SELECT * FROM (
来源：http://oa.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://st.hahajie.cn

) t WHERE rn = 1;
来源：http://nm.jianghongdianzi.cn

[Q35] 内连接
来源：http://no.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ya.huixiangedu.cn

[Q36] 左连接
来源：http://as.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ml.newstarts.cn

[Q37] 右连接
来源：http://rd.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yw.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wt.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ee.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://go.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ig.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ji.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xn.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tx.shxzskj.cn

[Q41] 多表连接
来源：http://wm.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gp.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://hv.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://ab.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://wn.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://bf.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vr.lnxyls.cn

[Q43] 标量子查询
来源：http://mu.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rh.bjjhwx.cn

[Q44] IN 子查询
来源：http://mi.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ys.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://ss.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lw.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xf.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ei.szxytkj.cn

[Q47] 与平均值比较
来源：http://gq.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zr.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://sf.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kn.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://mw.szxytkj.cn

[Q49] 更新单行
来源：http://yi.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kq.haigaiapp.cn

[Q50] 批量更新
来源：http://yc.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hn.panjiajie.cn

[Q51] 用子查询更新
来源：http://mt.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ka.bookmarksfly.cn

[Q52] 删除指定行
来源：http://mg.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://xe.haigaiapp.cn

[Q53] 按条件删除
来源：http://iq.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gh.huanxung.cn

[Q54] 清空表
来源：http://qb.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://rc.9csxet.cn

[Q55] 排名（并列占位）
来源：http://cz.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cx.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://wx.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gs.huixinmuqiang.cn

[Q57] 行号
来源：http://ez.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kf.yuexingan06.cn

[Q58] 累计求和
来源：http://co.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uu.hahajie.cn

[Q59] 分组内累计
来源：http://kv.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uz.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://af.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cv.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tw.jianghongdianzi.cn

[Q61] 移动平均
来源：http://bz.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vs.shxzskj.cn

[Q62] 分组占比
来源：http://tx.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wo.huixinmuqiang.cn

[Q63] 开启事务
来源：http://dm.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lv.wgjwhj.cn

[Q64] 提交事务
来源：http://bx.huixinmuqiang.cn

COMMIT;
来源：http://hs.muxihuayi.cn

[Q65] 回滚事务
来源：http://bd.9csxet.cn

ROLLBACK;
来源：http://ns.asd995.cn

[Q66] 行锁查询
来源：http://hu.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nx.hahajie.cn

[Q67] 设置隔离级别
来源：http://zt.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yq.yuexingan06.cn

[Q68] 保存点
来源：http://mc.hnjuh.cn

SAVEPOINT sp1;
来源：http://sm.lnxyls.cn

ROLLBACK TO sp1;
来源：http://mg.asd995.cn

[Q69] 查看执行计划
来源：http://yy.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hi.colortex.cn

[Q70] 更新统计信息
来源：http://tr.bjjhwx.cn

ANALYZE TABLE users;
来源：http://di.szxytkj.cn

[Q71] 查看建表语句
来源：http://wu.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jg.huanxung.cn

[Q72] 查看索引
来源：http://bv.huanxung.cn

SHOW INDEX FROM users;
来源：http://jg.szxytkj.cn

[Q73] 查看表状态
来源：http://vn.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qo.jctech888.com.cn

[Q74] 强制使用索引
来源：http://ud.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ur.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://hp.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pr.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wo.jctech888.com.cn

[Q76] 按天统计
来源：http://rp.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kb.hahajie.cn

[Q77] 时间加减
来源：http://uv.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ts.szsharing.cn

[Q78] 当前时间
来源：http://gs.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iu.muxihuayi.cn

[Q79] 字符串拼接
来源：http://vv.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://un.gzmigu.cn

[Q80] 字符串截取
来源：http://gf.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fa.gzmigu.cn

[Q81] 字符串替换
来源：http://fe.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ms.asd995.cn

[Q82] 字符长度与字节长度
来源：http://pk.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ls.shtwfgs.cn

[Q83] 大小写转换
来源：http://ls.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qn.hahajie.cn

[Q84] 去除首尾空格
来源：http://yw.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://qo.nicolike.cn

[Q85] 数值取整
来源：http://rr.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://md.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://kp.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rz.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://rx.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://is.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://di.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zg.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kn.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://pq.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xy.wgjwhj.cn

[Q90] 生成序号列
来源：http://ud.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rq.lnxyls.cn

================================================================================
来源：http://fn.yuntaijiaju.cn

R. Bash 专题
来源：http://jh.huixiangedu.cn

================================================================================
来源：http://rw.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://th.hahajie.cn

#!/usr/bin/env bash
来源：http://qc.szsharing.cn

set -euo pipefail
来源：http://zx.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://fw.nicolike.cn

name="Tom"; echo "$name"
来源：http://vj.muxihuayi.cn

[R03] 只读变量
来源：http://kx.shxzukj.cn

readonly PI=3.14
来源：http://bc.hahajie.cn

[R04] 位置参数
来源：http://vj.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zv.9csxet.cn

[R05] 参数默认值
来源：http://kw.newstarts.cn

name="${1:-default}"
来源：http://qy.asd995.cn

[R06] 判断命令是否存在
来源：http://pt.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://em.nicolike.cn

[R07] if 判断文件
来源：http://ua.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lk.huixiangedu.cn

[R08] 数值比较
来源：http://pi.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kg.shxzukj.cn

[R09] 字符串比较
来源：http://sj.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://so.yuntaijiaju.cn

[R10] 正则匹配
来源：http://ko.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xk.shxzskj.cn

[R11] case 多分支
来源：http://ta.muxihuayi.cn

case "$1" in
来源：http://ri.szxytkj.cn

start) echo "启动" ;;
来源：http://up.nszjky.cn

stop)  echo "停止" ;;
来源：http://jd.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://hx.shxzskj.cn


<!-- 参考信息 -->
代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ku.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yb.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nk.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ir.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fg.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zy.szsharing.cn

[P03] 生成短随机字符串
来源：http://he.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vq.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xo.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mj.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qv.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://im.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yw.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zy.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nv.yuexingan06.cn

[P04] 求长度
来源：http://qx.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://du.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vn.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hr.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nu.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://oz.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ec.shxzukj.cn

Ruby: x.length;  x.size
来源：http://uz.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://po.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://gn.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ec.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vl.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://no.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qe.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dr.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zv.jctech888.com.cn

Ruby: a == b
来源：http://jg.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sl.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ui.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qy.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://or.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cc.muxihuayi.cn

TS:   if (x == null) {}
来源：http://lg.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wp.nicolike.cn

Go:   if x == nil {}
来源：http://ss.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lm.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://su.muxihuayi.cn

[P07] 防抖与节流
来源：http://gn.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xw.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://gj.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vj.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gs.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ig.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ko.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hf.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fq.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://ti.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gr.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xg.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dj.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aq.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://my.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sn.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://al.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lu.nszjky.cn

================================================================================
来源：http://pn.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qq.newstarts.cn

================================================================================
来源：http://pz.hahajie.cn

[Q01] 创建表
来源：http://lt.lnxyls.cn

CREATE TABLE users (
来源：http://hr.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zy.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://ny.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://li.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xf.lnxyls.cn

);
来源：http://ji.colortex.cn

[Q02] 创建带外键的表
来源：http://dr.szxytkj.cn

CREATE TABLE orders (
来源：http://gp.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xy.gzmigu.cn

user_id INT NOT NULL,
来源：http://mv.asd995.cn

amount DECIMAL(10, 2),
来源：http://xk.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zz.muxihuayi.cn

);
来源：http://ld.shxzskj.cn

[Q03] 增加列
来源：http://vk.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qi.9csxet.cn

[Q04] 修改列类型
来源：http://ms.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ao.yuntaijiaju.cn

[Q05] 重命名列
来源：http://et.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bv.9csxet.cn

[Q06] 删除列
来源：http://ay.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rv.jianghongdianzi.cn

[Q07] 删除表
来源：http://rk.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://vy.asd995.cn

[Q08] 创建普通索引
来源：http://az.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://is.colortex.cn

[Q09] 创建唯一索引
来源：http://om.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://si.gzmigu.cn

[Q10] 插入单行
来源：http://je.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vf.nszjky.cn

[Q11] 一次插入多行
来源：http://jb.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qq.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://us.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uq.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jd.nicolike.cn

[Q13] 忽略重复插入
来源：http://ld.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tr.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://wq.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iv.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://na.gzmigu.cn

[Q15] 查询全部
来源：http://li.bjjhwx.cn

SELECT * FROM users;
来源：http://do.bjjhwx.cn

[Q16] 查询指定列
来源：http://bs.shxzskj.cn

SELECT id, name FROM users;
来源：http://rg.hahajie.cn

[Q17] 条件查询
来源：http://pm.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mu.lnxyls.cn

[Q18] 模糊匹配
来源：http://wd.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kc.chemitech.net.cn

[Q19] 范围查询
来源：http://hk.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tt.hnjuh.cn

[Q20] IN 列表
来源：http://nl.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tr.shtwfgs.cn

[Q21] 空值判断
来源：http://lh.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zc.jianghongdianzi.cn

[Q22] 排序
来源：http://mw.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ec.nicolike.cn

[Q23] 分页
来源：http://kd.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ko.panjiajie.cn

[Q24] 去重
来源：http://fh.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://fn.szsharing.cn

[Q25] 只取前 N 条
来源：http://uw.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zr.muxihuayi.cn

[Q26] 计数
来源：http://nr.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://bb.newstarts.cn

[Q27] 条件计数
来源：http://jy.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ka.lnxyls.cn

[Q28] 求和与平均
来源：http://pn.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fz.gzmigu.cn

[Q29] 最大最小值
来源：http://dp.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sl.huixiangedu.cn

[Q30] 分组统计
来源：http://ma.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xl.jctech888.com.cn

[Q31] 分组后过滤
来源：http://gt.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ka.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://to.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wy.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://um.nicolike.cn

[Q33] 多列分组
来源：http://ij.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gs.shxzskj.cn

[Q34] 每组取第一条
来源：http://bt.jianghongdianzi.cn

SELECT * FROM (
来源：http://la.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mc.colortex.cn

) t WHERE rn = 1;
来源：http://fj.muxihuayi.cn

[Q35] 内连接
来源：http://yw.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mr.wgjwhj.cn

[Q36] 左连接
来源：http://uk.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ys.colortex.cn

[Q37] 右连接
来源：http://zl.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bo.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fo.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hc.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://pk.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tz.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nv.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cl.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pz.huixiangedu.cn

[Q41] 多表连接
来源：http://pj.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nf.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ds.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://pa.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://my.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://ap.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ed.nicolike.cn

[Q43] 标量子查询
来源：http://qy.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ow.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://fp.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sg.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://tt.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xb.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pn.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cq.shxzukj.cn

[Q47] 与平均值比较
来源：http://py.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nr.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://wl.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gq.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ua.chemitech.net.cn

[Q49] 更新单行
来源：http://ma.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ag.jianghongdianzi.cn

[Q50] 批量更新
来源：http://ew.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bg.colortex.cn

[Q51] 用子查询更新
来源：http://sw.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yt.asd995.cn

[Q52] 删除指定行
来源：http://xh.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://dj.panjiajie.cn

[Q53] 按条件删除
来源：http://fj.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zy.bjjhwx.cn

[Q54] 清空表
来源：http://dc.asd995.cn

TRUNCATE TABLE logs;
来源：http://ss.newstarts.cn

[Q55] 排名（并列占位）
来源：http://ki.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fk.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://fq.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yw.szxytkj.cn

[Q57] 行号
来源：http://uq.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iy.colortex.cn

[Q58] 累计求和
来源：http://bj.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://my.chemitech.net.cn

[Q59] 分组内累计
来源：http://fy.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rq.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://gx.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hv.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bz.asd995.cn

[Q61] 移动平均
来源：http://me.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fq.bjjhwx.cn

[Q62] 分组占比
来源：http://xl.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mh.nszjky.cn

[Q63] 开启事务
来源：http://fr.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nz.nicolike.cn

[Q64] 提交事务
来源：http://hy.huixiangedu.cn

COMMIT;
来源：http://nw.lnxyls.cn

[Q65] 回滚事务
来源：http://tp.haigaiapp.cn

ROLLBACK;
来源：http://tk.panjiajie.cn

[Q66] 行锁查询
来源：http://cy.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hl.hahajie.cn

[Q67] 设置隔离级别
来源：http://sd.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bd.wgjwhj.cn

[Q68] 保存点
来源：http://an.panjiajie.cn

SAVEPOINT sp1;
来源：http://vr.newstarts.cn

ROLLBACK TO sp1;
来源：http://pf.asd995.cn

[Q69] 查看执行计划
来源：http://kb.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ls.nszjky.cn

[Q70] 更新统计信息
来源：http://kx.nszjky.cn

ANALYZE TABLE users;
来源：http://ao.shtwfgs.cn

[Q71] 查看建表语句
来源：http://sa.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zt.huixiangedu.cn

[Q72] 查看索引
来源：http://mr.nicolike.cn

SHOW INDEX FROM users;
来源：http://vc.panjiajie.cn

[Q73] 查看表状态
来源：http://bu.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kj.shtwfgs.cn

[Q74] 强制使用索引
来源：http://du.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://si.nszjky.cn

[Q75] 日期格式化
来源：http://vi.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pu.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nicolike.cn

[Q76] 按天统计
来源：http://zc.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zo.huixiangedu.cn

[Q77] 时间加减
来源：http://kh.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hj.huanxung.cn

[Q78] 当前时间
来源：http://kb.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://na.newstarts.cn

[Q79] 字符串拼接
来源：http://hu.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qy.nicolike.cn

[Q80] 字符串截取
来源：http://cu.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://do.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://ii.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lr.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://rv.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bh.muxihuayi.cn

[Q83] 大小写转换
来源：http://ea.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ze.asd995.cn

[Q84] 去除首尾空格
来源：http://ka.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://no.hahajie.cn

[Q85] 数值取整
来源：http://is.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://us.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://fu.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xm.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://lp.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oh.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://cr.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uz.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mf.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ph.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lv.nicolike.cn

[Q90] 生成序号列
来源：http://rm.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vo.huanxung.cn

================================================================================
来源：http://wj.newstarts.cn

R. Bash 专题
来源：http://as.jianghongdianzi.cn

================================================================================
来源：http://jn.nicolike.cn

[R01] shebang 与严格模式
来源：http://sl.lnxyls.cn

#!/usr/bin/env bash
来源：http://uk.panjiajie.cn

set -euo pipefail
来源：http://nn.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://iv.nszjky.cn

name="Tom"; echo "$name"
来源：http://sk.lnxyls.cn

[R03] 只读变量
来源：http://jx.shxzskj.cn

readonly PI=3.14
来源：http://iw.bjjhwx.cn

[R04] 位置参数
来源：http://sh.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ig.hnjuh.cn

[R05] 参数默认值
来源：http://mj.jianghongdianzi.cn

name="${1:-default}"
来源：http://dp.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://wi.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://no.shtwfgs.cn

[R07] if 判断文件
来源：http://fo.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tu.szsharing.cn

[R08] 数值比较
来源：http://yv.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vv.bookmarksfly.cn

[R09] 字符串比较
来源：http://vf.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dx.gzmigu.cn

[R10] 正则匹配
来源：http://lm.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uh.huanxung.cn

[R11] case 多分支
来源：http://ub.9csxet.cn

case "$1" in
来源：http://ip.9csxet.cn

start) echo "启动" ;;
来源：http://wj.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://ux.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://cm.shtwfgs.cn

esac
来源：http://rw.muxihuayi.cn

[R12] for 遍历文件
来源：http://uv.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://au.gzmigu.cn

[R13] for 计数循环
来源：http://ou.colortex.cn


<!-- 参考信息 -->
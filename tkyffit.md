代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gz.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ju.shxzskj.cn

[P03] 生成短随机字符串
来源：http://vz.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ve.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ln.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rl.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dv.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://li.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://he.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bx.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nt.nicolike.cn

[P04] 求长度
来源：http://gp.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mv.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://za.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jw.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iz.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://qn.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ui.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://eu.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sv.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://jd.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zu.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zo.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ba.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zx.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ds.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mg.huanxung.cn

Ruby: a == b
来源：http://if.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://it.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ng.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://es.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://dd.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bp.colortex.cn

TS:   if (x == null) {}
来源：http://cy.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sx.jctech888.com.cn

Go:   if x == nil {}
来源：http://ko.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xm.nszjky.cn

C#:   if (x is null) {}
来源：http://vh.bjjhwx.cn

[P07] 防抖与节流
来源：http://it.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oj.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://jd.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lo.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yi.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oq.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rc.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zz.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cl.nicolike.cn

[P08] 处理浮点精度问题
来源：http://cj.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vz.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jm.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hg.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uq.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ay.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iz.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yj.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vz.colortex.cn

================================================================================
来源：http://sx.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vj.shxzskj.cn

================================================================================
来源：http://gh.bjjhwx.cn

[Q01] 创建表
来源：http://qd.521024.cn

CREATE TABLE users (
来源：http://mi.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uv.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://qg.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ko.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ag.szsharing.cn

);
来源：http://yj.panjiajie.cn

[Q02] 创建带外键的表
来源：http://kz.shxzukj.cn

CREATE TABLE orders (
来源：http://dw.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jr.panjiajie.cn

user_id INT NOT NULL,
来源：http://qc.huanxung.cn

amount DECIMAL(10, 2),
来源：http://mt.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qv.wgjwhj.cn

);
来源：http://oc.newstarts.cn

[Q03] 增加列
来源：http://pe.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cl.9csxet.cn

[Q04] 修改列类型
来源：http://vn.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://si.hnjuh.cn

[Q05] 重命名列
来源：http://zu.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pq.haigaiapp.cn

[Q06] 删除列
来源：http://md.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rp.lnxyls.cn

[Q07] 删除表
来源：http://ex.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://eb.nicolike.cn

[Q08] 创建普通索引
来源：http://se.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://if.521024.cn

[Q09] 创建唯一索引
来源：http://hs.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mf.haigaiapp.cn

[Q10] 插入单行
来源：http://ou.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gh.bjjhwx.cn

[Q11] 一次插入多行
来源：http://wu.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ab.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://ln.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://at.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://je.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://qw.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bt.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://ik.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iw.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cv.yuntaijiaju.cn

[Q15] 查询全部
来源：http://mn.jctech888.com.cn

SELECT * FROM users;
来源：http://ex.szsharing.cn

[Q16] 查询指定列
来源：http://ya.yuexingan06.cn

SELECT id, name FROM users;
来源：http://dk.jianghongdianzi.cn

[Q17] 条件查询
来源：http://iz.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tx.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://ny.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://er.colortex.cn

[Q19] 范围查询
来源：http://jt.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gi.shxzukj.cn

[Q20] IN 列表
来源：http://ws.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ze.asd995.cn

[Q21] 空值判断
来源：http://yh.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lt.colortex.cn

[Q22] 排序
来源：http://gr.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hj.jianghongdianzi.cn

[Q23] 分页
来源：http://xi.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vn.hahajie.cn

[Q24] 去重
来源：http://fy.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://yr.hnjuh.cn

[Q25] 只取前 N 条
来源：http://kq.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://il.lnxyls.cn

[Q26] 计数
来源：http://ys.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://pq.nszjky.cn

[Q27] 条件计数
来源：http://jj.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ds.lnxyls.cn

[Q28] 求和与平均
来源：http://de.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wv.huixiangedu.cn

[Q29] 最大最小值
来源：http://bh.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xv.yuexingan06.cn

[Q30] 分组统计
来源：http://qz.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ha.521024.cn

[Q31] 分组后过滤
来源：http://ep.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tf.szsharing.cn

[Q32] 分组拼接字符串
来源：http://hq.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sk.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gy.szsharing.cn

[Q33] 多列分组
来源：http://ii.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sf.muxihuayi.cn

[Q34] 每组取第一条
来源：http://mw.yuexingan06.cn

SELECT * FROM (
来源：http://kb.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ho.jctech888.com.cn

) t WHERE rn = 1;
来源：http://wo.chemitech.net.cn

[Q35] 内连接
来源：http://ul.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vb.panjiajie.cn

[Q36] 左连接
来源：http://st.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yw.newstarts.cn

[Q37] 右连接
来源：http://fv.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rv.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fv.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sa.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ir.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rt.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://is.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dy.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lk.wgjwhj.cn

[Q41] 多表连接
来源：http://ar.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://em.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://xu.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://td.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://xp.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://vk.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xs.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://fo.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ld.panjiajie.cn

[Q44] IN 子查询
来源：http://ji.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ma.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://zy.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://og.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zq.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://am.521024.cn

[Q47] 与平均值比较
来源：http://gs.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tk.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://lj.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ps.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://jk.colortex.cn

[Q49] 更新单行
来源：http://lk.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qs.chemitech.net.cn

[Q50] 批量更新
来源：http://oq.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xg.hahajie.cn

[Q51] 用子查询更新
来源：http://vj.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rw.asd995.cn

[Q52] 删除指定行
来源：http://kn.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://qd.bjjhwx.cn

[Q53] 按条件删除
来源：http://jq.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qy.yuntaijiaju.cn

[Q54] 清空表
来源：http://wg.newstarts.cn

TRUNCATE TABLE logs;
来源：http://sk.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://yv.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sk.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://ta.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ty.lnxyls.cn

[Q57] 行号
来源：http://ot.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rt.9csxet.cn

[Q58] 累计求和
来源：http://mh.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qq.hnjuh.cn

[Q59] 分组内累计
来源：http://jy.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uu.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://qk.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://me.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bk.shxzskj.cn

[Q61] 移动平均
来源：http://am.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uq.huanxung.cn

[Q62] 分组占比
来源：http://xt.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wu.9csxet.cn

[Q63] 开启事务
来源：http://ah.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xs.hahajie.cn

[Q64] 提交事务
来源：http://tg.lnxyls.cn

COMMIT;
来源：http://as.chemitech.net.cn

[Q65] 回滚事务
来源：http://mb.szxytkj.cn

ROLLBACK;
来源：http://vr.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://yq.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tn.nicolike.cn

[Q67] 设置隔离级别
来源：http://jr.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fo.panjiajie.cn

[Q68] 保存点
来源：http://sp.lnxyls.cn

SAVEPOINT sp1;
来源：http://cy.521024.cn

ROLLBACK TO sp1;
来源：http://fu.521024.cn

[Q69] 查看执行计划
来源：http://op.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zk.szsharing.cn

[Q70] 更新统计信息
来源：http://ci.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://uk.yuexingan06.cn

[Q71] 查看建表语句
来源：http://py.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jk.nszjky.cn

[Q72] 查看索引
来源：http://as.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://dk.hahajie.cn

[Q73] 查看表状态
来源：http://we.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fz.bjjhwx.cn

[Q74] 强制使用索引
来源：http://ps.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ro.9csxet.cn

[Q75] 日期格式化
来源：http://wj.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ew.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aq.colortex.cn

[Q76] 按天统计
来源：http://de.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nv.asd995.cn

[Q77] 时间加减
来源：http://pk.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gv.panjiajie.cn

[Q78] 当前时间
来源：http://fq.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ga.panjiajie.cn

[Q79] 字符串拼接
来源：http://yy.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gu.asd995.cn

[Q80] 字符串截取
来源：http://ij.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ij.huanxung.cn

[Q81] 字符串替换
来源：http://sy.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pw.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://wj.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jq.asd995.cn

[Q83] 大小写转换
来源：http://vh.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rt.asd995.cn

[Q84] 去除首尾空格
来源：http://jv.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://dw.yuntaijiaju.cn

[Q85] 数值取整
来源：http://rw.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gy.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://lf.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gx.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://xr.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jq.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://ux.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gb.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rp.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://oi.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ca.wgjwhj.cn

[Q90] 生成序号列
来源：http://re.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yl.huanxung.cn

================================================================================
来源：http://rj.hnjuh.cn

R. Bash 专题
来源：http://jx.szsharing.cn

================================================================================
来源：http://jd.szxytkj.cn

[R01] shebang 与严格模式
来源：http://tu.hahajie.cn

#!/usr/bin/env bash
来源：http://is.jianghongdianzi.cn

set -euo pipefail
来源：http://jz.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://zl.hahajie.cn

name="Tom"; echo "$name"
来源：http://gv.shxzukj.cn

[R03] 只读变量
来源：http://cu.asd995.cn

readonly PI=3.14
来源：http://fw.szxytkj.cn

[R04] 位置参数
来源：http://vy.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mw.nszjky.cn

[R05] 参数默认值
来源：http://iz.bjjhwx.cn

name="${1:-default}"
来源：http://nc.521024.cn

[R06] 判断命令是否存在
来源：http://le.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mc.bookmarksfly.cn

[R07] if 判断文件
来源：http://at.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wi.jctech888.com.cn

[R08] 数值比较
来源：http://xc.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tp.szsharing.cn

[R09] 字符串比较
来源：http://cb.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vb.9csxet.cn

[R10] 正则匹配
来源：http://dy.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ol.szxytkj.cn

[R11] case 多分支
来源：http://jg.colortex.cn

case "$1" in
来源：http://xz.asd995.cn

start) echo "启动" ;;
来源：http://pp.asd995.cn

stop)  echo "停止" ;;
来源：http://ie.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://fo.hahajie.cn

esac
来源：http://oj.newstarts.cn

[R12] for 遍历文件
来源：http://fz.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://fi.huixinmuqiang.cn

[R13] for 计数循环
来源：http://py.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://kz.nszjky.cn

[R14] C 风格 for
来源：http://og.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nx.shtwfgs.cn

[R15] while 逐行读文件
来源：http://dq.hahajie.cn


<!-- 参考信息 -->